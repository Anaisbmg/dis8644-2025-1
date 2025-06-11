# sesion-10a

## Apuntes

### RGB LED

![RGB LED pinout](./archivos/rgb-led-pinout.jpg)

Fuente: <https://pijaeducation.com/tinkercad/code-blocks-for-rgb-led-interfacing-with-arduino-in-tinkercad/>

Combinan ${\color{#b0e6e6}3 \ LEDs \ de \ distintos \ colores}$ (${\color{red}rojo}$, ${\color{lightgreen}verde}$ y ${\color{blue}azul}$) en un mismo componente, cada uno de estos ${\color{#b0e6e6}LEDs \ brilla}$ con ${\color{#b0e6e6}distinta \ intensidad}$ para producir el color deseado, ya que al estar tan cerca se ${\color{#b0e6e6}mezcla \ la \ luz}$ que cada uno emite  En los LED RGB, los 3 LEDs de colores suelen venir en 2 configuraciones: cátodo y ánodo común

### Display de 7 segmentos

![Pinout del display de 7 segmentos](./archivos/7segDis.jpg)

Fuente: <https://amishajhanji.weebly.com/datasheets.html>

Similares a los LEDs RGB en que ${\color{#b0e6e6}contienen \ múltiples \ LEDs}$ de menor tamaño dentro, sin embargo estos displays emplean LEDs del mismo color en ${\color{#b0e6e6}distintas \ ubicaciones \ para \ formar \ distintos \ números \ y/o \ letras}$

### [Codificador(encoder)](https://youtu.be/NWiPVMDh7GE?si=5goLb4drnWfBChbt) y [decodificador(decoder)](https://youtu.be/HHQFI8R1iZc?si=c0AfhkyOAGCwZzmC)

En un display de 7 segmentos hay que ${\color{#b0e6e6}controlar \ 7 \ LEDs}$, pero ¿qué pasa si tenemos varios displays de 7 segmentos trabajando juntos para mostrar números más grandes o pantallas de más alta resolución? necesitaríamos una ${\color{#b0e6e6}cantidad \ enorme \ de \ pines \ GPIO}$ en nuestros microcontroladores (arduino, esp32, raspberry pi pico, etc), sin mencionar la cantidad de cables y espacio.  Es por esto que se emplean ${\color{#b0e6e6}encoders}$ y ${\color{#b0e6e6}decoders}$

* ${\color{#b0e6e6}Encoders}$: Toma ${\color{#b0e6e6}múltiples \ inputs}$ y los convierte en ${\color{#b0e6e6}pocos \ outputs}$. Ej: Un teclado con 101 teclas que se comunica mediante USB (Universal Serial Bus), el cual utiliza 2 canales llamados Data+ y Data- para comunicarse

* ${\color{#b0e6e6}Decoders}$: Toma ${\color{#b0e6e6}pocos \ inputs}$ y los convierte en ${\color{#b0e6e6}múltiples \ outputs}$. Ej: Un microcontrolador controlando un display de 60 LEDs mediante el protocolo I2C, el cual emplea 2 canales de comunicación (Serial Data [SDA] y Serial Clock [SCL])

### [RGB v/s CMYK](https://youtu.be/NnP-SRiOc4o?si=X7VKQyWvUsUm_wed)

Son ${\color{#b0e6e6}formatos \ de \ colores}$ utilizados en programas de diseño de ilustraciones, editores de imágenes, entre otros. Se emplean estos distintos formatos por el ${\color{#b0e6e6}diferente \ comportamiento \ de \ la \ luz}$ al ser emitida directamente hacia los ojos y reflejada en una superficie y luego llegar a los ojos.

![Distintas pantallas OLED (Organic LED) vista 'zoomed in'](./archivos/oled.jpg)

Fuente: <https://hk.news.yahoo.com/chinese-2015-11-27-sony-xperia-z5-premium-review.html>

RGB se utiliza para diseñar ${\color{#b0e6e6}imágenes \ que \ se \ muestran \ a \ través \ de \ pantallas}$, este formato obtiene su nombre de la misma forma que el LED RGB (${\color{red}Red}$, ${\color{lightgreen}Green}$ & ${\color{blue}Blue}$), aunque su uso no es exclusivo de pantallas OLED o microLED (emplean diminutos LEDs RGB como pixeles)

![Representación 'zoomed in' de una impresión.](./archivos/cmyk.jpg)

Fuente: <https://www.shutterstock.com/es/image-vector/seamless-pattern-consisting-starsvector-illustration-background-405815827>

CMYK es utilizado para diseñar ${\color{#b0e6e6}imágenes \ para \ impresión}$, se podría decir que a diferencia de ${\color{#b0e6e6}RGB}$ que se utiliza para ${\color{#b0e6e6}imágenes \ digitales}$, ${\color{#b0e6e6}CMYK}$ se utiliza para ${\color{#b0e6e6}imágenes \ analógicas}$. Obtiene su nombre a partir de las tintas empleadas para impresión (Cyan, Magenta, Yellow & Key [negro]

### Comparador Minecraft

El comparador cuando está operando en modo comparador (modo resta con la antorcha frontal encendida), ${\color{#b0e6e6}compara \ la \ intensidad \ de \ la \ señal}$ de redstone en sus terminales laterales y principal.  Si la señal en su ${\color{#b0e6e6}terminal \ A}$ es mayor a la intensidad de la ${\color{#b0e6e6}terminal \ B}$, el comparador dejará pasar la señal A (output) Si la señal de la ${\color{#b0e6e6}terminal \ A}$ es igual o inferior a la señal de la ${\color{#b0e6e6}terminal \ B}$, entonces no dejará que pase la señal

![MCcomp1](./archivos/MCcomp1.jpg)

![MCcomp2](./archivos/MCcomp2.jpg)

![MCcomp3](./archivos/MCcomp3.jpg)

### LM324 [Op Amp (Operational amplifier)](https://youtu.be/OSCKBmkrH_g?si=QFSQ32b00GYuRYbe)

![Pinout LM324](./archivos/LM324-pinout.jpg)

Fuente: <https://microcontrollerslab.com/lm324-op-amp-pinout-datasheet-applications-features-datasheet/>

Este Op Amp (Operational Amplifier) está compuesto por ${\color{#b0e6e6}4 \ comparadores}$ (LM741 x 4) Los comparadores de los circuitos se comportan igual que el comparador de minecraft (modo comparador), pero en lugar de comparar la intensidad de la señal de redstone, ${\color{#b0e6e6}comparan \ el \ voltaje}$ que hay en cada terminal.

<!-- Comparator -->

![Comparador símbolo completo](./archivos/compSymb1.jpg)

Fuente: <https://www.masters.com.pl/en/news/st-analog-circuits-part-two-comparators-and-current-sense-amplifiers?sectionId=1&id=10533>

![Comparador símbolo simple](./archivos/compSymb2.jpg)

Fuente: <https://es.m.wikipedia.org/wiki/Archivo:Comparator_symbol.sv>

Aquí podemos apreciar los ${\color{#b0e6e6}2 \ símbolos}$ que representan a los comparadores en los esquemas. El símbolo de la ${\color{#b0e6e6}izquierda \ es \ el \ símbolo \ completo}$, ya que el comparador requiere una conexión a una ${\color{red}fuente \ de \ poder}$, ${\color{#b0e6e6}además \ de \ las \ líneas \ que \ está \ comparando}$, para poder trabajar. Mientras que en la ${\color{#b0e6e6}derecha}$ tenemos el ${\color{#b0e6e6}símbolo \ simplificado}$, que ${\color{red}no \ muestra \ las \ conexiones \ a \ la \ fuente \ de \ poder}$.  ${\color{gray}Se \ emplea \ el \ simplificado \ cuando \ se \ quiere \ entender \ la \ lógica}$ con la que se está trabajando sin confundirse con las demás conexines, que se sabe estan allí, pero no son necesarias para entender el funcionamiento del circuito (en algunos casos).

### [Componentes activos v/s pasivos](https://youtu.be/TgXMujXoG3I?si=h1dPGlVeSPS144HP)

En el mundo de la electrónica, los ${\color{#b0e6e6}componentes \ se \ clasifican \ entre \ 2 \ grupos}$, componentes ${\color{red}activos}$, que al igual que los comparadores, requieren estár ${\color{red}conectados \ a \ una \ fuente \ de \ poder}$ para operar. A diferencia de los componentes ${\color{#ffe4a8}pasivos}$, como resistencias, LEDs, motores, etc. Que solo necesitan recibir un input para funcionar, es decir, ${\color{red}no \ requieren \ una \ conexión \ dedicada \ a \ proveer \ energía}$ al componente además de los inputs.

### [Micrófono Electret](https://youtu.be/aSXv6FdYQfM?si=nr6VB09ea1yaSGRq)

![Inside electret](./archivos/electret.jpg)

Fuente: <https://mynewmicrophone.com/the-complete-guide-to-electret-condenser-microphones/>

Es un micrófono que funciona teniendo un ${\color{#6462fe}capacitor \ integrado}$. Básicamente, tiene en su interior ${\color{#b0e6e6}2 \ placas \ conductivas \ que \ no \ se \ tocan}$ pero están suficientemente cerca como para alterarse entre sí con sus emisiones electromagnéticas (si una placa tiene su polo positivo más cerca de la otra, esta tendrá su polo negativo más cerca de la primera) de la misma forma que funciona un capacitor. Una de estas ${\color{#b0e6e6}placas}$ está ${\color{#b0e6e6}fija}$, mientras la otra está sujeta a una membrana ${\color{#b0e6e6}flexible}$ que ${\color{#b0e6e6}se \ mueve}$ en mayor o menor medida ${\color{#b0e6e6}dependiendo \ de \ las \ vibraciones}$ que reciba, esto resulta en una ${\color{red}variación \ de \ voltaje}$ al variar la distancia entra ambas placas (${\color{red}señal \ análoga}$) ${\color{#3d3d44}(los \ acelerómetros \ funcionan \ bajo \ el \ mismo \ principio)}$

### [Divisor de voltaje](https://youtu.be/fmSC0NoaG_I?si=IHEnsN_ys78Bt8Sm)

![Voltage divider](./archivos/voltageDivider.jpg)

Fuente: <https://study.com/academy/lesson/voltage-divider-circuit-rule-bias-formula.html>

Se pueden conectar ${\color{#ffe4a8}2 \ resistencias \ en \ serie}$ entre ${\color{red}Vcc}$ y ${\color{gray}GND}$ ${\color{red}para \ variar \ el \ voltaje \ (reducirlo)}$. O en nuestro caso, un ${\color{#ffe4a8}potenciómetro}$, ya que ${\color{#ffe4a8}consiste \ de \ 2 \ resistencias \ variables}$. Esto se puede emplear para darle energía a un componente o sección de un circuito que funciona con un voltaje inferior al resto del circuito

### Other things: <!-- Things to organize + random stuff -->

[Voltaje negativo](https://youtu.be/z5eB_2wjLTg?si=Ngw1xYDsibCLor0w)

![baterías conectadas en serie](./archivos/negativeVoltage.jpg)

Fuente: <https://www.build-electronic-circuits.com/what-is-negative-voltage/>

Tener un ${\color{red}voltaje \ negativo}$ significa que el ${\color{red}voltaje \ medido}$ ${\color{#b0e6e6}es \ más \ bajo \ que \ el \ punto \ de}$ ${\color{white}referencia \ (GND)}$. Por ejemplo, si conectamos la ${\color{red}terminal \ positiva}$ del ${\color{#b0e6e6}multímetro}$ a ${\color{white}GND}$ y la ${\color{white}terminal \ negativa}$ a ${\color{red}+9V}$, el ${\color{#b0e6e6}multímetro}$ leerá ${\color{white}-9V}$, porque ${\color{red}+9V}$ se ${\color{#b0e6e6}convierte}$ en el ${\color{white}punto \ de \ referencia \ (GND)}$ y ${\color{white}0V}$ es ${\color{#b0e6e6}inferior}$ a ${\color{red}+9V}$ por, valga la redundancia, ${\color{red}9V}$. Los voltajes negativos son últiles para aplicaciones como ${\color{#b0e6e6}amplificadores \ de \ audio}$, ya que el ${\color{#b0e6e6}parlante \ empuja}$ el ${\color{#b0e6e6}aire}$ en una ${\color{red}dirección \ (+V)}$ y luego tiene que moverse en ${\color{white}reversa \ (-V)}$ en lugar de quedarse quieto en el medio, cuando pudo haber desplazado más aire.
>
> ### [Buffer](https://youtu.be/VKU9ciJb5u4?si=xksuSbaQz_msCMvr)
>
> Es un circuito que nos permite ${\color{red}mantener \ el \ voltaje \ (output) \ de \ un \ circuito}$, pero ${\color{#b0e6e6}aumentando \ la \ corriente}$ de este, para que componentes y/o circuitos que requieren una mayor corriente operen según esperado.
Se puede hacer un [buffer con un comparador](https://youtu.be/PvGdRVg5QXY?si=OnEHXtQWHpUfwJ3S) al conectar su ${\color{white}output}$ a su ${\color{white}input-}$
-----------------------------------------------------------------------------------------------------------

## Encargo 20 <!-- subir fotos de su propia autoría de pantallas de siete segmentos, y otras variantes que encuentren en su vida cotidiana. les pedimos al menos 3 fotos de distintas pantallas. pueden partir de la base de las que ya subieron hoy a discord. incluir información sobre dónde y cuándo fue capturada la imagen. -->

### Displays de 7 segmentos

### 1.- Indicador de piso del ascensor de la FAAD  2.- Pantalla que indica el recorrido de la micro

![Pantalla ascensor de la FAAD](./archivos/elevator.jpg)

![Pantalla de Transantiago/Micro/Red](./archivos/micro.jpg)

### 3.- Indicador de paso y contador del semáforo  4.- Contador del microondas de mi casa

![Semáforo](./archivos/semaforo.jpg)

![Pantalla microondas](./archivos/microondas.jpg)

5.- Pantalla de la lavadora de mi casa

6.- Pantalla de reloj despertador de mi papá

![Pantalla lavadora](./archivos/lavadora.jpg)

![Pantalla reloj despertador](./archivos/watch.jpg)

7.- Pantalla de reloj digital de mi casa

8.- Pantalla que muestra la temperatura de mi cautín

![Pantalla reloj digital](./archivos/clock.jpg)

![Pantalla temperatura cautín](./archivos/iron.jpg)

## Encargo 21 <!-- simular circuitos que hemos visto en clases con chips 555 y/o circuitos comparadores usando el simulador de Falstad disponible en -->

### Simulación de circuitos en [Falstad](https://www.falstad.com/circuit/)

Comparador + divisor de voltaje:

```txt
$ 1 0.000005 10.20027730826997 66 5 43 5e-11
r 224 224 288 224 0 1000
162 288 224 320 224 2 default-led 1 0 0 0.01
g 320 224 320 256 0 0
R 0 192 0 112 0 0 40 9 0 0 0.5
403 48 80 176 144 0 0_64_0_4099_0.0000762939453125_0.00009765625_-1_2_0_3
a 112 224 208 224 9 9 0 1000000 4.945500000000001 3.3533291106226013 100000
174 0 288 80 192 1 100000 0.5495000000000001 potenciometro umbral
g 0 288 0 304 0 0
w 80 240 112 240 0
374 208 160 112 160 0 0.8317000000000001 LDR
R 592 128 592 48 0 0 40 9 0 0 0.5
R 208 160 208 112 0 0 40 9 0 0 0.5
r 112 160 48 160 0 10000
w 112 208 112 160 0
g 48 160 48 192 0 0
w 208 224 224 224 0
403 16 256 144 320 0 8_64_0_4099_5_0.00009765625_-1_2_8_3
403 192 240 320 304 0 15_64_0_4099_0.00030517578125_0.00009765625_-1_2_15_3
403 160 256 288 320 0 13_64_0_4099_10_0.00009765625_-1_2_13_3
o 8 64 0 4099 10 0.00009765625 0 6 8 3 13 0 13 3 15 0 15 3
```

NE555 astable

````txt
$ 1 0.000005 10.20027730826997 66 5 43 5e-11
R 592 128 592 48 0 0 40 9 0 0 0.5
165 80 176 272 176 6 8.992760336826649
w 144 144 208 144 0
w 208 208 208 144 0
w 176 336 176 368 0
g 176 368 176 400 0 0
162 272 240 272 336 2 default-led 1 0 0 0.01
g 272 336 272 384 0 0
r 208 240 272 240 0 1000
c 144 336 144 384 4 0.00009999999999999999 5.942592511917423 0.001 0
g 144 384 144 400 0 0
w 80 208 48 208 0
r 48 208 48 144 0 10000
w 144 144 48 144 0
w 80 272 80 304 0
w 48 272 80 272 0
209 80 304 80 384 4 0.00001 5.674993227448654 0.001 0 1
g 80 384 80 400 0 0
R 144 144 144 96 0 0 40 9 0 0 0.5
174 32 208 32 320 1 100000 0.45050000000000007 Resistance
w 32 208 48 208 0
403 -80 352 48 416 0 14_64_0_4099_10_0.0001953125_-1_2_14_3
````

NE555 monostable

````txt
$ 1 0.000005 109.66331584284586 56 5 43 5e-11
R 592 128 592 48 0 0 40 9 0 0 0.5
165 80 176 272 176 6 8.992760336826649
w 176 336 176 368 0
g 176 368 176 400 0 0
162 272 240 272 336 2 default-led 1 0 0 0.01
g 272 336 272 384 0 0
r 208 240 272 240 0 1000
c 144 336 144 384 4 0.00009999999999999999 5.99999999984605 0.001 0
g 144 384 144 400 0 0
174 -48 160 -32 240 1 10000 0.005 Resistance
w 144 144 208 144 0
w 208 144 208 208 0
r 64 208 -32 208 0 1000
R -48 160 -48 128 0 0 40 9 0 0 0.5
R 144 144 144 112 0 0 40 9 0 0 0.5
c 64 336 64 384 4 0.00047 6.181085321275481 0.001 0.1
g 64 384 64 400 0 0
R 16 272 -32 272 0 0 40 9 0 0 0.5
s 16 272 48 272 0 1 false
w 48 272 80 272 0
c -32 336 -32 384 4 0.00047 6.181219552111755 0.001 0
g -32 384 -32 400 0 0
s 0 336 32 336 0 1 false
w -32 336 0 336 0
w 64 208 80 208 0
w 64 208 64 304 0
w 64 304 80 304 0
w 64 304 64 336 0
403 -48 432 80 496 0 27_64_0_4099_10_0.00625_-1_2_27_3
w 32 336 64 336 0
````

PWM

````txt
$ 1 0.000015625 4.818269829109882 56 5 43 5e-11
R 592 128 592 48 0 0 40 9 0 0 0.5
165 80 176 272 176 6 0
R 144 144 144 112 0 0 40 9 0 0 0.5
r 208 240 288 240 0 1000
162 288 240 288 320 2 default-led 1 0 0 0.01
g 288 320 288 352 0 0
w 144 144 208 144 0
w 208 144 208 208 0
c 144 336 144 384 4 0.00047 5.99999999915942 0.001 0
g 144 384 144 400 0 0
g 176 336 176 400 0 0
r 64 144 64 208 0 1000
w 64 208 80 208 0
w 64 144 144 144 0
c 80 304 80 384 4 0.00001 4.620083443523556 0.001 0
g 80 384 80 400 0 0
174 -64 256 16 288 1 100000 0.9950000000000001 Resistance
d -64 256 -64 208 2 default
d 32 208 32 256 2 default
w -64 208 32 208 0
w 32 208 64 208 0
w -16 288 80 288 0
w 80 272 80 288 0
w 80 288 80 304 0
403 -80 128 48 192 0 19_64_0_4099_0.15625_0.00009765625_-1_2_19_3
403 -64 304 64 368 0 23_64_0_4099_10_0.00009765625_-1_2_23_3
````
