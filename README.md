# Alfrond
Victor David Muñoz Ramirez - Santiago Cortes Osorio - Digitales III

<div align="center">
  <h2>Universidad de Antioquia</h2>
  <h3>Electrónica Digital 3</h3>
  <br>
  <h1>ALFROND</h1>
  <h2>Propuesta de Proyecto de Aula</h2>
  <br>
  <h3>Presentado por:</h3>
  <p>
    Víctor David Muñoz Ramírez<br>
    Santiago Cortes Osorio
  </p>
  <br>
  <p>
    Medellín, Colombia<br>
  </p>
</div>

<br>

## Primer formato (25 de agosto) 

## 1. Nombre del Proyecto
**Alfrond**

## 2. Descripción de la Idea Inicial
Alfrond es un vehículo robótico móvil diseñado como un asistente de servicio a pequeña escala, similar a un carrito hotelero. El objetivo principal de Alfrond es desplazarse de manera autónoma desde un punto inicial, como un escritorio, hasta una estación de abastecimiento para recoger un snack (como una bolsa de papas) y llevarlo de regreso al punto de partida en este caso el escritorio.

Para cumplir con este objetivo, la navegación del robot se realizará mediante un sistema de **seguidor de línea**, utilizando sensores infrarrojos que le permitirán guiarse con precisión por una ruta predefinida en el suelo. Como medida de seguridad adicional, el vehículo contará con un **sensor de proximidad** en su parte frontal, diseñado para detener el robot inmediatamente si detecta un obstáculo inesperado en su camino, evitando así cualquier colisión.

Una vez que el robot llegue a la estación de abastecimiento, entrará en acción un **brazo robótico** de 3 grados de libertad, el cual se encargará de manipular y agarrar el snack. Para garantizar que la recolección fue exitosa, la canasta de carga del robot integrará un **sensor piezoeléctrico**. Este sensor actuará como una báscula o detector de impacto que "sentirá" la vibración o presión cuando la bolsa caiga dentro del recipiente, enviando una señal a la Raspberry Pi Pico para confirmar que la carga está asegurada antes de emprender el viaje de regreso.

## 3. Motivación
La motivación central para desarrollar **Alfrond** es la oportunidad de llevar la teoría de los circuitos y sistemas digitales a un escenario práctico, a una solucion para ciertas industrias, y salir un poco de lo comun en los proyectos que se realizan en la universidad. Este proyecto nos atrae porque sincronizar el desplazamiento de un vehículo con la manipulación física de un brazo robótico representa un desafío técnico altamente estimulante para nosotros, creemos que nos permitirá aplicar directamente nuestras habilidades de programación, manejo de registros, interrupciones y control de actuadores, entre otros que iremos aprendiendo a lo largo del curso, consolidando nuestra formación en ingeniería mediante la resolución de problemas reales de calibración e integración tecnológica.
