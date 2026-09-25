# Actividad final — Primer corte

## Sistemas Inteligentes I — Búsqueda, Minimax y poda Alfa-Beta

### Integrantes

- Paula Andrea Cano
- Vanessa Alejandra Osorio

### Descripción breve de la actividad

La actividad consiste en estudiar y resolver, mediante notebooks de Jupyter, los tres grandes bloques del curso: búsqueda no informada (BFS y DFS), búsqueda informada (costo uniforme, A* y Beam Search) y búsqueda adversarial (Minimax y poda Alfa-Beta).

Junto con los cuadernos de referencia que explican cada tema, se incluyen los talleres resueltos que aplican los algoritmos a problemas como laberintos, recipientes de agua, el 8-puzzle, una cuadrícula con obstáculos y el juego de las piedras.

### Relación de notebooks incluidos

| Notebook | Contenido |
|---|---|
| `Resolucion_Problemas_Busqueda_NoInformada.ipynb` | Material de referencia: búsqueda no informada (BFS y DFS), laberinto, recipientes y 8-puzzle. |
| `Resolucion_Problemas_Busqueda_Informada.ipynb` | Material de referencia: búsqueda informada (costo uniforme, A* y Beam Search), heurísticas y 8-puzzle. |
| `Minimax.ipynb` | Material de referencia: búsqueda adversarial — algoritmo Minimax. |
| `Poda_Alfa_Beta.ipynb` | Material de referencia: poda Alfa-Beta y su comparación con Minimax. |
| `TallerBNI.ipynb` | Taller resuelto de búsqueda no informada: laberinto (BFS/DFS), recipientes y BFS del 8-puzzle. |
| `TallerBusquedaInformada.ipynb` | Taller de búsqueda informada: base del tema y solución de la Parte 1 (cuadrícula con UCS, A* y Beam Search). |
| `TallerMinimax.ipynb` | Taller resuelto de Minimax aplicado al juego de las piedras. |

### Instrucciones mínimas para ejecutar

1. Abrir una terminal en la raíz del repositorio.
2. Activar el entorno virtual: `.\.venv\Scripts\activate` (Windows) o `source .venv/bin/activate` (Linux/macOS).
3. (Primera vez) Instalar `matplotlib` si hace falta: `.\.venv\Scripts\pip install matplotlib`
4. Iniciar Jupyter: `jupyter lab` (o `jupyter notebook`).
5. Abrir el notebook deseado y ejecutar las celdas en orden (Kernel → Restart & Run All).

### Uso de IA generativa

Se utilizó IA generativa como herramienta de apoyo para comprender los conceptos de los algoritmos y para recibir sugerencias de cambios o modificaciones sobre el código y la redacción de los notebooks. Todo el trabajo entregado fue revisado, entendido y validado por las integrantes.