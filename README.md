# Triki (Tic-Tac-Toe) con Minimax y Poda Alfa-Beta
Este proyecto implementa el clásico juego de Triki (Tic-Tac-Toe) utilizando el algoritmo 
Minimax con Poda Alfa-Beta para optimizar la búsqueda de la jugada óptima. También se 
incluye una versión básica del algoritmo Minimax sin optimización. El código está escrito 
en Python y simula un jugador que toma decisiones óptimas para ganar el juego.

**Características:**
- Simulación del juego Triki: El juego sigue las reglas estándar del Triki.
- Algoritmo Minimax: El jugador toma decisiones óptimas basadas en el algoritmo Minimax.
- Poda Alfa-Beta: Se usa para mejorar la eficiencia del algoritmo reduciendo el número de nodos evaluados.
- Soporte para Minimax básico: Se incluye una versión no optimizada del algoritmo Minimax.
- Detección de ganador: El juego determina si hay un ganador o si hay empate.
- Funcionalidad completa del juego: Jugador vs Computadora optimizada.

# Requisitos
- **1 -> Instalar Python**
- **2 -> Clonar el resositorio:**
```bash
git clone https://github.com/tu-usuario/nombre-repositorio.git
cd nombre-repositorio
```

- **3 -> Ejecutar el codigo:**
```bash
python triki.py
```

# Estructura del Código:
El código consta de las siguientes partes importantes:

- initial_state(): Devuelve el estado inicial del tablero vacío.
- player(board): Retorna el jugador que tiene el siguiente turno (X u O).
- actions(board): Lista todas las acciones posibles en el tablero (casillas vacías).
- result(board, action): Aplica una acción al tablero y devuelve el nuevo estado.
- winner(board): Determina si hay un ganador en el juego.
- terminal(board): Verifica si el juego ha terminado (ganador o empate).
- utility(board): Evalúa el resultado del juego: 1 si gana X, -1 si gana O, 0 si es empate.
- minimax(board): Implementación del algoritmo Minimax con Poda Alfa-Beta.
- basic_minimax(board): Versión no optimizada del algoritmo Minimax.

# Ejecución del Juego
- El tablero se representa como una matriz 3x3, donde cada casilla puede estar vacía (None), ocupada por una 'X', o ocupada por una 'O'.
- El jugador siempre juega con 'X', y la computadora toma decisiones usando Minimax con Poda Alfa-Beta.
- El juego continúa hasta que haya un ganador o un empate.

# Ejemplo de Tablero Inicial:
```bash
[[None, None, None],
 [None, None, None],
 [None, None, None]]
```

# Decisión Óptima:
El algoritmo Minimax evaluará todas las acciones posibles y retornará la mejor jugada para el jugador actual.

# Contribuciones
Si deseas contribuir, por favor, sigue estos pasos:
- Haz un fork del proyecto.
- Crea una nueva rama (git checkout -b feature-nueva-funcionalidad).
- Realiza tus cambios y haz commit (git commit -am 'Añadir nueva funcionalidad').
- Sube la rama (git push origin feature-nueva-funcionalidad).
- Abre un Pull Request.
