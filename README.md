# Chesster
Víctor David Muñoz Ramírez - Santiago Cortés Osorio - Digitales III

<div align="center">
  <h2>Universidad de Antioquia</h2>
  <h3>Electrónica Digital 3</h3>
  <br>
  <h1>CHESSTER</h1>
  <h2>Brazo Robótico Ajedrecista Autónomo</h2>
  <br>
  <h3>Presentado por:</h3>
  <p>
    Víctor David Muñoz Ramírez<br>
    Santiago Cortés Osorio
  </p>
  <br>
  <p>
    Medellín, Colombia<br>
  </p>
</div>

<br>

## Reporte Técnico - Iteración 2

## 1. Nombre del Proyecto
**Chesster**

## 2. Descripción de la Idea Inicial
Chesster es un sistema mecatrónico autónomo diseñado como un brazo manipulador estacionario cuyo propósito es jugar ajedrez físicamente contra un oponente humano. El nombre es un juego de palabras con "Jester", el clásico bufón de la corte, actuando en este caso como un compañero robótico de entretenimiento personal.

Para cumplir con su objetivo, el sistema opera bajo una arquitectura *standalone* controlada por una Raspberry Pi Pico W. El sistema no requiere conexión a un PC durante la partida. La percepción del tablero se realiza mediante la cámara de un celular que transmite video vía WiFi a la placa. Utilizando un modelo de visión artificial YOLO (ajustado previamente mediante *Transfer Learning*), el microcontrolador mapea el tablero en una matriz de 8x8, donde las casillas y las piezas son identificadas con valores numéricos del 0 al 12. Esto le permite comparar el estado actual del tablero con el del turno anterior para validar que el movimiento del humano haya sido legal.

Una vez validada la jugada humana, el motor de ajedrez embebido decide el próximo movimiento. La ejecución física se realiza coordinando motores paso a paso para el posicionamiento preciso en los ejes X y Y, un servomotor para el descenso en el eje Z, y un electroimán capaz de sujetar, mover o capturar las piezas. El sistema interactúa constantemente con el usuario a través de una botonera HMI y una pantalla LCD, indicando tiempos, turnos y detectando errores físicos, como advertir al jugador si dejó una pieza en una "posición ambigua" entre dos casillas.

## 3. Motivación
La motivación central para desarrollar **Chesster** surge de la evolución tecnológica de nuestro equipo. Decidimos descartar nuestra propuesta inicial enfocada en la navegación móvil para concentrar todos nuestros esfuerzos en un desafío mucho más profundo y riguroso: la cinemática, el control de precisión y la visión artificial integrada.

Este proyecto nos apasiona porque llevar la teoría de los circuitos, el procesamiento de imágenes en hardware de recursos limitados (RAM limitada) y el control espacial en 3D a un escenario físico e interactivo es un reto técnico sumamente estimulante. Integrar un modelo de inteligencia artificial embebido para validar reglas y tomar decisiones autónomas nos permitirá aplicar directamente nuestras habilidades en programación de microcontroladores, manejo de periféricos (PWM, señales Step/Dir, I2C) y estructuración de datos, consolidando nuestra formación en ingeniería a través de un proyecto complejo y fuera de lo común.