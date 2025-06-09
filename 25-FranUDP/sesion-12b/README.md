# sesion-12b

## Apuntes

### SUBTITULO

### Other things

#### SUB_SUBTITULO

## Encargo 24 y 25 <!-- Describir de forma textual 3 proyectos de máquinas electrónicas que quieran hacer de forma individual, ordenar por preferencia o interés de que sea desarrollado. Dibujar diagrama de comportamiento, flujos de interacción. No específicar chips. Considerar procesos de manera especulativa. ¿Cuánto tiempo se usará? ¿Qué encendidos y apagados tiene? ¿Cómo se interactúa? -->

### Descripción ideas

### 1.- Dispensador de comida automático

Mi perrita se la pasa sola en la casa durante la mayoría del día, debido a que estamos todos ocupados fuera, todos menos mi hermano (por ahora).
Previendo la posibilidad que él deje de poder reponerle el agua y la comida a causa de la universidad, pensé en un dispensador de agua y comida automático.

Este aparato se enchufará a la pared a través de una power supply de 5V USB-C y contará con una batería interna que asegurará que se mantendrá funcionando incluso durante cortes de luz.

El dispositivo tendrá un botón de encendido y apagado, además de una perilla para determinar la cantidad de comida, otra para la cantidad de agua dispensada y otra para seleccionar el tiempo de espera antes de reponer los alimentos.

El dispensador detectará cuando le hayan acabado el agua (agua como switch) y la comida (LDR al fondo del plato), en caso de que los platos estén vacíos, el dispositivo comenzará a contar hasta que se cumpla el delay establecido antes de liberar la cantidad especificada de alimento. Este delay se debe a que si no se regula la frecuencia y las porciones que inhieren las mascotas, la salud de estas se verá afectada.

Si el dispensador está recibiendo energía del power supply mantendrá encendida un LED azul, en caso de estar funcionando en energía de emergencia este LED parpadeará; mientras la batería se esté cargando, brillará un LED rojo; Si los tanques de agua y comida de reserva están cerca de vaciarse, el dispositivo avisará parpadeando el LED rojo.

![dispensador](./archivos/1.jpg)

### 2.- Pomodoro sonoro

A quienes tenemos TDAH (ADHD) nos puede llegar a costar muchísimo sentarnos a trabajar sin inmediatamente distraernos o comenzar a soñar despiertos.

Una solución usualmente recomendada para este dilema es la técnica del pomodoro (tomate en italiano) que consiste en estudiar por aproximadamente 25 minutos con pequeños breaks entre medio, sin embargo, sin embargo, dependiendo de la capacidad de mantenerse consciente de cada uno, es posible que uno se "vuele" sin saberlo incluso empleando esta técnica.

El dispositivo recibirá energía a través de un puerto USB-A (5V).

EL aparato contará con una palanca de encendido y apagado, un botón para seleccionar si funciona o no el parlante y una perilla para variar la duración de los períodos de estudio y descanso (no son valores independientes).

Una vez el pomodoro es encendido, este comenzará a emitir un sonido (pulso) cada aproximadamente 10 segundos, esto es para que el usuario pueda mantenerse al tanto del paso del tiempo sin tener que ver un reloj, mientras esto está pasando, un LED irá brillando con una intensidad cada vez mayor, hasta que se cumpla el tiempo de estudio.

Una vez comience el período de descanso, el LED comenzará a atenuarse hasta apagarse, momento en el cual comenzará otro ciclo estudio-descanso.

![Pomodoro sonoro](./archivos/2.jpg)

### 3.- Guante sintetizador

Se me ocurrió la idea de un instrumento que emita distintos sonidos dependiendo del gesto que se haga con la mano, esto se lograría teniendo los inputs de distintos elementos sonoros en la yema de los dedos (zona metalizada) y distintos valores experimentales ubicados en las falanges y otras zonas de la mano (en caso de que este método no sea viable, se pueden usar pequeños botones de TPU esparcidos por la superficie del guante).
En otras palabras, dependiendo de que parte de la mano (incluyendo otros dedos) toques con cada dedo variará la frecuencia, el tono, la nota siendo tocada, el volumen, etc.

Este aparato funcionaría con un una batería recargable mediante USB-c.

![Guante sintetizador](./archivos/3.jpg)
