# sesion-06a

Entrega Proyecto 01

## LDA: Light Dependent Awelita

### Premisa

- Elegir Temática

- Definir Usuario

- Definir Función

## Elegir Temática

<https://www.555-timer-circuits.com>

![Foto de los ejemplos que más nos gustaron(las4 en una misma foto)](./archivos/tme-p1-esquemas.png)

Miramos los distintos ejemplos en esta página, y destacamos los que más nos llamaron la atención.

![foto bitácora](./archivos/tme-p1-bitacoraEsquema.jpeg)

![foto del cirucuito APC](./archivos/tme-p1-circuitoAtari.jpeg)

![Foto esquemático original del pryecto dark detector](./archivos/tme-p1-esquemaDarkDetector1.png)

![Foto trabajo poor discord](./archivos/tme-p1-trabajoOnline.jpeg)

![Foto circuito armadod](./archivos/tme-p1-circuitoDark.jpeg)

<https://www.555-timer-circuits.com/dark-detector.html>

Este proyecto consiste en un circuito que sensa la luz a través de un LDR. Una alarma se activa cuando el nivel de luz detectado es menor a cierta cantidad determinada por la configuración del sistema.

## Definir Usuario

![Foto user persona](./archivos/tme-p1-user.png)

USER PERSONA

- Nombre: Gloria Fernández
- Edad: 89 años
- Género: Femenino
- Estado civil: Viuda
- Ciudad: Chillán

Biografía:

Gloria vive una casa con su hijo, su nuera y sus dos nietos. Trabajó de como educadora de párvulos hasta los 72 años. Todos los días desayuna entre las 10:30 y las 12:00, almuerza entre las 13:30 y las 16:30, y toma once entre las 19:30 y las 22:00. el horario en el que realiza sus *hobbies* va desde las 14:00 hasta las 21:30.

Motivación:

Busca realizar actividades que la ayuden a distraerse y a hacer que el tiempo pase más rápido. puede pasar horas entretenida con actividades como leer, tejer, bordar, armar rompecabezas y resolver sopas de letras.

## Definir Función a Partir de la Problemática

Problemática:

Identificamos una problemática en aquella situación cuando una persona, en este caso un adulte mayor, realiza actividades que requieren concentración, durante extensos periodos. Cuando estos períodos coinciden con la puesta del sol, el usuario sigue realizando su actividad a oscuras.

Esto ocurre porque la disminución de la luz es paulatina, y sucede a una velocidad que permite que nuestro ojo se vaya acostumbrando a ella automáticamente. Por eso a veces pareciera que oscureció de golpe en la noche

![Figura 1.13 del archivo retinaAdaptTesis.pdf](./archivos/tme-p1-grafico.png)

<https://uvadoc.uva.es/handle/10324/22376>

Si bien, no hay estudios que comprueben que hacer atividades a oscuras dañe la vista, hacer actividades a oscuras requiere un mayor esfuerzo, por lo tanto te cansa más y dificulta hacerlo por períodos prolongados.

Definición Función:

![Foto luz alarma](./archivos/tme-p1-alarmaNoche.jpeg)
Imagen generada por Ia mediante chatGPT

Un objeto que cuando se oscurezca emita una alarma para alertar al usuario, y que este recuerde encender una luz para que no suene. Esta alarma sonará durante 300s y después el istema se suspenderá hasta que vuelva a detectar luz.

### Diseño

## Investigación 1: Iluminación

![foto de algo con luz ahaha](./archivos/tme-1p-fotoLuz.jpeg)

<https://pin.it/83V7VnPhr>

La luz es un fenónemo que scede como efecto secundario de la radiación electromagnética. Esta es percibida por el ojo humano dentro de un espectro visible con longitudes de onda entre 380 y 750mm.

<https://es.wikipedia.org/wiki/Luz>

La intensidad de la luz se mide en lúmenes(lx), se mide con un instrumento llamado luxómetro.

Para trabajar / leer se recomiendan entre 300-500lx

| Ejemplo de valores lux         |            |
|--------------------------------|------------|
| Luz solar                      | 40.00 lx   |
| Lugar de trabajo en la oficina | 300-500 lx |
| Sala de estar                  | 50-200 lx  |
| Noche de luna                  | 0,3 lx     |
  
## Investigación 2: ¿Cómo lograr que suceda?

Podemos seprar en 2 nuestros objetivos del funcionamiento electrónico del objeto:

- Emitir sonido cuando sense

- Que el sonido no sea permanente

Para cada uno de los objetivos que tenemos ya tenemos un circuito conocido.

Con el circuito  Dark Detector podemos hacer que el cirtuito emita una alarma cuando haya poca luz.

![Foto esquemático original del proyecto dark detector](./archivos/tme-p1-esquemaDarkDetector1.png)

Con el circuito monoestable podemos lograr que cuando se recibe un estímulo, este quede corriendo durante un tiempo y después apagarse.

![Foto esquemático original del circuito monoestable](./archivos/tme-p1-esquemaMonoestable.png)

La idea es "fusionar" ambos circuitos para lograr que la parte del Dark Detector(A) "controle" a la parte monoestble (B)

![Foto esquemático dibujo parte A](./archivos/tme-p1-esquemaFusionA.jpeg)

![Foto esquemático dibujo parte B](./archivos/tme-p1-esquemaFusionB.jpeg)

![Foto esquemático dibujo fusión](./archivos/tme-p1-esquemaFusion.jpeg)

## Redefinición

Tras múltiples intentos no logramos

![Foto esquemático intento fallido tinker](./archivos/tme-p1-tinkerTry1.png)

![Foto esquemático otro intento fallido tinker](./archivos/tme-p1-tinkerTry2.png)

Tras no lograr llevar a cabo la idea original, decidimos optar por quedarnos con la parte que teníamos funcionando.

![Foto esquemático del circuito que tenemos realmente](./archivos/tme-p1-esquemaDarkDetector1.png)

![Foto edel cableado funcionante](./archivos/tme-p1-esquemaDark.png)

![Foto del flujo real](./archivos/tme-p1-flujoReal.png)

![Foto esquemático dibujo fusión](./archivos/tme-p1-esquemaFusion.jpeg)

![Foto del flujo que queriamos que fuera](./archivos/tme-p1-flujoIdeal.png)

### FABRICACIÓN

- Cables

- Carcasa

## Cables

![Foto avances](./archivos/tme-p1-bitacoraBoceto.jpeg)

En esta etapa tomamos medidas de los componentes, y los tuvimos en cuenta para el diseño de la carcasa

Bill of Materials

| Componente              | Valor | Unidades |
|-------------------------|-------|----------|
| Resistencia             | 10k   | 1        |
| Resistencia             | 22k   | 1        |
| Resistencia             | 100k  | 1        |
| Resistencia             | 1M    | 1        |
| Capacitor Cerámico      | 10nF  | 1        |
| Capacitor Cerámico      | 100nF | 1        |
| Capacitor Electrolítico | 10uF  | 1        |
| LDR                     |       | 1        |
| Bocina                  |       | 1        |
| 555                     |       | 1        |
| protoboard              |       | 1        |
| Cables Dupont           |       | 1        |
| Batería                 |  9V   | 1        |

## Carcasa

Hicimos un modelo 3D mediante Rhinoceros 3D

![Foto donde aparezcan varias fotos de proceso del modelado 3d](./archivos/tme-p1-modelado0.png)

![Foto del modelado 1](./archivos/tme-p1-modelado01.png)

![Foto del modelado 1](./archivos/tme-p1-modelado02.png)

![Foto del render](./archivos/tme-p1-render.png)

Impresión 3D

![Foto de la impresión comenzando](./archivos/tme-p1-imp1.jpg)

![foto de la impresión al 40%](./archivos/tme-p1-imp2.jpg)

![foto de la impresión fallando](./archivos/tme-p1-imp3.jpg)

![Foto de la impresión lista](./archivos/tme-p1-imp4.jpg)

![Foto de la los soportes sacados](./archivos/tme-p1-imp5.jpg)

### Referencias

<555-timer-circuits.com>

- <https://www.digikey.com/es/resources/conversion-calculators/conversion-calculator-resistor-color-code>

- <https://www.digikey.com/es/resources/conversion-calculators/conversion-calculator-series-and-parallel-capacitor>

- <https://www.tinkercad.com>

- <https://circuitdigest.com/calculators/capacitor-value-code-calculator>

- <https://www.youtube.com/watch?v=WeC7cR6n48M>

- <https://www.simonelectric.com/blog/niveles-de-iluminacion-recomendados-segun-cada-zona-y-actividad>

- <https://bricoprofesional.com/blog/como-nos-afecta-la-iluminacion-en-nuestra-salud/#:~:text=Baño%3A%20no%20hace%20falta%20demasiada,iluminación%20general%20de%20100%20lx.>

Para más información y más proceso, por favor consultar nuestro figma con acceso público:

<https://www.figma.com/board/2tv4jx75qGZa6Gua2UCVer/taller.maq.electr?node-id=0-1&t=aBNh63yuq9MDT4AI-1>

### enacrgo 12: kicad

Instalé kicad para windows. Versión 9.0.2. Creé una carpeta llamada kicad, dentro de mi carpeta del taller. de modo que la jerarquía es: Escritorio > todo > universidarks > 4TO-ano > taller.maq.elec > kicad. dentro de la carpeta de kicad tengo los siguientes archivos: udpudu, theypudu, 00-libsKicad-teee, etc.

ahora me gustaría cambiar la carpeta kicad desde la carpeta del taller, hacia mi carpeta diseno.diseno, en la cual guardo cosas relacionadas a lo que me gusta diseñar. en ese caso la jerarquía sería:  Escritorio > todo > diseno.diseno > kicad.
