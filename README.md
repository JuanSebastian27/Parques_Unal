# Parques_Unal
Parques creado en Python
README.txt
Proyecto Parqués para Programadores
Descripción del Proyecto
Este proyecto es una implementación del clásico juego de Parqués orientado a programadores, desarrollado en Python utilizando la biblioteca Pygame. El juego simula la jugabilidad tradicional del parqués, en el que cuatro equipos (Rojo, Verde, Azul y Amarillo) compiten para mover sus fichas desde la cárcel, recorrer 68 casillas en el tablero externo y, finalmente, avanzar por 8 casillas del tramo “cielo” (home) para llegar a la meta.

Requisitos
Python 3.x
Pygame (para la parte gráfica)
Sistema operativo: Windows, macOS o Linux
Cómo Ejecutar el Juego
Instalación de Dependencias:

Asegúrate de tener Python 3 instalado.
Instala la biblioteca Pygame ejecutando en la terminal:
nginx
Copiar
Editar
pip install pygame
Descargar el Proyecto:

Descarga el archivo principal del juego (por ejemplo, prueba_juego17.py o la versión final que hayas integrado) y colócalo en una carpeta.
Ejecutar el Juego:

Abre una terminal (o símbolo del sistema) y navega hasta la carpeta donde se encuentra el archivo.
Ejecuta el siguiente comando:
nginx
Copiar
Editar
python prueba_juego17.py
Se te pedirá que selecciones el modo de juego:
Modo Real: Los dados se lanzan de forma aleatoria para simular una partida real.
Modo Desarrollador: Permite ingresar manualmente los valores de los dados para facilitar pruebas y ajustes.
Controles Durante el Juego:

Tecla ESPACIO: Lanza los dados y ejecuta el turno del jugador actual.
En algunos casos, si hay varias opciones de movimiento, se solicitará al jugador que ingrese mediante la consola el número de la ficha que desea mover.
La interfaz gráfica muestra el tablero con 68 casillas externas y un tramo “cielo” (home) especial para cada equipo. Las casillas especiales (salidas, seguros y home) incluyen etiquetas descriptivas.
Reglas Básicas de Jugabilidad
Inicio y Movimiento:

Todas las fichas comienzan en la cárcel.
Para sacar una ficha de la cárcel se requiere obtener un 5 (o una suma de 5 en los dados) y que la casilla de salida tenga menos de dos fichas.
Una vez en juego, cada ficha debe recorrer 68 casillas externas y luego 8 casillas del tramo “cielo” para alcanzar la meta final (76 pasos en total).
Movimiento con Dados:

Cada dado se procesa de forma independiente, lo que permite usar el resultado de cada uno en fichas diferentes.
Si una ficha está a 75 pasos (es decir, necesita 1 para ganar), se permite moverla si alguno de los dados muestra un 1.
Capturas y Bloqueos:

Si una ficha se mueve a una casilla no segura y se encuentra con una ficha enemiga, se aplican las reglas de captura.
Las fichas en las casillas de “cielo” (home) son intocables y no pueden ser capturadas.
Se permite un máximo de 2 fichas en la casilla de salida; si ya hay 2 fichas, se debe mover una ficha en juego para liberar el espacio.
Dobles y Penalizaciones:

Si se obtiene un dado doble, el mismo jugador repite turno.
Si se obtienen 3 dobles consecutivos, se penaliza enviando una ficha a la cárcel.
Finalización:

El equipo gana cuando las 4 fichas han completado el recorrido y alcanzado la meta final.
