# AGENTS.md

## Qué es este repo

Colección plana (sin paquetes) de notebooks Jupyter en **español** para el curso Sistemas Inteligentes I: búsqueda no informada (BFS/DFS), búsqueda informada (A*), Minimax y poda Alfa-Beta. Remoto: `origin/main` → `https://github.com/VanessaOsorioS/ActividadFinalInteligentesI.git`.

- **No hay** README, requirements, pyproject, tests, lint, CI ni `.gitattributes`. No inventes comandos de build/test/typecheck: no existen.
- Todo el contenido (markdown, comentarios, identificadores en demos) está en **español**; mantén ese idioma al editar o crear celdas/notebooks.

## Entorno

- Existe `.venv/` (Python 3.12.6) con `ipykernel`, `jupyter` client e `ipython`. Úsalo para ejecutar celdas:
  - Windows: `.\.venv\Scripts\python.exe`, `.\.venv\Scripts\jupyter.exe`
- **`matplotlib` NO está instalado** en el venv, pero ambos notebooks `Resolucion_Problemas_Busqueda_*.ipynb` lo importan. Antes de ejecutarlos: `.\.venv\Scripts\pip install matplotlib`.
- `nbconvert` tampoco está instalado → no se puede ejecutar notebooks en headless (`jupyter nbconvert --execute` fallará). Ejecuta celdas en un kernel o instala lo que falte.
- El kernelspec registrado es `python3` (a nivel de usuario, en `AppData\Roaming\Python`). El `display_name` del metadata (`SIntel` o `.venv (3.12.6.final.0)`) es cosmético.

## Gotchas de git / archivos

- **Dos notebooks están vacíos (0 bytes)** y fueron commiteados así: `TallerBusquedaInformada.ipynb`, `TallerMinimax.ipynb`. No son JSON válido; si hay que completarlos, escríbelos como nbformat 4 completo (copia la estructura/metadata de `Minimax.ipynb` o `Poda_Alfa_Beta.ipynb`).
- `TallerBNI.ipynb` también era 0 bytes en HEAD; ahora tiene contenido **sin commitear** (ejercicio TODO de `bfs_8_puzzle`).
- Hay cambios sin commitear en `Resolucion_Problemas_Busqueda_NoInformada.ipynb` y `TallerBNI.ipynb`. El diff del primero incluye una salida guardada de error (`ModuleNotFoundError: No module named 'matplotlib'`) de una ejecución fallida: **las outputs guardadas no son verdad de origen**; re-ejecuta o limpia las celdas afectadas antes de dar por bueno un resultado.
- `core.autocrlf=true` y no hay `.gitattributes`: los `.ipynb` (JSON con LF) generan ruido de CRLF en los diffs. No reformatees notebooks enteros ni cambies indentación JSON sin motivo; edita solo las celdas necesarias.
- Los `.ipynb` son UTF-8 con acentos españoles. No re-guardar en cp1252/latin-1 (la consola Windows puede mostrar mojibake aunque el archivo esté bien).

## Convenciones de notebooks

- nbformat 4, celdas con `id`, kernelspec `name: python3`.
- Estructura de contenido: encabezado `# Sistemas Inteligentes I` + subtítulo del tema, `**Autor:** Jairo I. Vélez B.`, secciones numeradas (`## 1. …`) que alternan explicación en markdown con celdas de código cortas que demuestran el concepto antes de presentar el algoritmo. Sigue ese patrón al añadir material.
