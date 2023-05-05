# TIC-TAC-TOE-ejercicio-pw

La función Square() permite ponerle un nuevo valor a un cuadrado en el tablero de acuerdo al click que se le haga.

En la función Board() en primera instancia se define el array squares correspondiente a los 9 espacios en el tablero, iniciando en null todos los espacios. Luego, se define la función handleClick() que recibe como parámetro la posición en el tablero (array). Primero calcula si se ha ganado, para después colocar "X" u "O" en caso sea el siguiente turno de xIsNext coloca "X", sino "O".

Hay también una porción de código llamada status, la cual según lo obtenido con la función calculateWinner, si esta es verdad,m anuncia al ganador, sino muestra de quien es el turno en el juego.

Los board-row arman el tablero de 3x3, asignándole a cada uno de los cuadrados la función de handleClick en su posición con el onSquareClick y una función flecha. 

La función para calcular si el jugador ha ganado se llama calculateWinner() a la que se le pasa como parámetro el array correspondiente a los cuadrados del tablero y se definen los movimientos que determinan si se gano con lines. Recorriendo el array de lines, si hay coincidencia en el array squares en posiciones a, b y c, se determina que el jugador ganó. 
