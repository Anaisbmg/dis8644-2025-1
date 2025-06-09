# sesion-03a

## Apuntes
>
> ### Voltaje y resistencia en tipos de circuitos
>
> ${\color{Red}Vcc}$ = Voltaje Corriente Continua (el positivo)
>
> * Resistencia en serie = **${\color{#ffe4a8}R}$${\color{#ffe4a8}Total}$** = R1 + R2 + R2 + R4
> * [Resistencias en paralelo](https://youtu.be/5uyJezQNSHw?si=-xhBxAEVZoKuAEOg&t=576) = 1/**${\color{#ffe4a8}R}$${\color{#ffe4a8}T}$** = 1/R1 + 1/R2 + 1/R2 + 1/R4
>
>> 1k + 1k = 500 ohm (por eso al conectar una segunda resistencia en paralelo, el LED brilla más)

### Prefijos notación científica

![alt-text](https://th.bing.com/th/id/R.a8057d46a9fe796121af98f1a3dd02f3?rik=AAD%2fVV2eYzustQ&riu=http%3a%2f%2ftutordelectronica.weebly.com%2fuploads%2f2%2f4%2f4%2f1%2f24418880%2f239438.jpg%3f623&ehk=s40UHD9u%2ffetT%2bD8Yr1tyAEp6rkjAxeDieXO5BjA7ys%3d&risl=&pid=ImgRaw&r=0)

Son simbolos que se colocan antes de las unidades de medida, para cambiar su valor y expresar cantidades más grandes o pequeñas de forma más corta (resumida) y comprensible.

Una forma en que se podría pensar sobre esto es con las unidades de medida del sistema métrico (ej: "g" y "kg") pero en lugar de tener 500 mil distintas unidades de medida distintas para medir lo mismo, le añadimos un apellido para denotar la cantidad de ceros.

### [Capacitores1/](https://youtu.be/X4EUwTwZ110?si=W06CjwpOs9OW3rEu)[Condensadores2](https://www.youtube.com/watch?v=rbCXKhhzBN0)

![alt-text](./archivos/CapacitorChargeDischarge.gif)

Similares a una bateria en que atrapan y liberan electrones
>> (carga/corriente), pero difieren en que estos se cargan
>> mucho más rapidamente, tienen una capacidad muchisimo
>> más limitada y no permiten el flujo de corriente a travez de
>> ellos.
>> Se suelen utilizar para estabilizar señales (pulsación como
>> metralleta -> pulsación estable, al evitar un on-off de golpe
>> al descargarse el capacitor)
>>
>> #### Simbologia

![alt-text](./archivos/CapacitorSymbology.png)

#### Ceramic & electrolytic

![alt-text](https://www.majju.pk/assets/uploads/2018/06/470UF-35V-ALUMINIUM-ELECTROLYTIC-POLAR-CAPACITOR-1200x684.jpg)

Los ${\color{orange}capacitores \space cerámicos}$ no tienen una polaridad predefinida, por lo que no importa que "pata" del capacitor es conectada al positivo o negativo.

![alt-text](https://th.bing.com/th/id/OIP.fZ6K37RHqWd1_SyJEgwiYgAAAA?rs=1&pid=ImgDetMain)

Estos capacitores tienen su capacidad escrita en un código de 3 dígitos: XXY, donde los primeros 2 dígitos (XX) son los primeros digitos del valor, al los cuales se le agrega (Y) cantidad de 0s. Ej: 474 = 470.000 F (Farads) ${\color{#3d3d44}[same \space as \space SMD \space resistors]}$

Los ${\color{#6462fe}capacitores \space electrolíticos}$, a diferencia de los cerámicos, si tienen una polaridad definida. Aparte de eso, almacenan más electrones y tienen su  capacitancia y voltaje escritos.

:warning: Si se conectan al revés hay una alta probabilidad que exploten :warning:

### [555 Timer](https://youtu.be/iwbGccGU4io?si=_w-Vn72tDD2A57a5)

Es una IC (Integrated Circuit), es decir, un circuito que alguien ya diseñó y que solo tenemos que conectarlo y usarlo.

En el caso del NE555, este es una IC que se emplea para producir *time delays* y oscilaciones precisas.

> El 555 puede operar en los siguientes modos:
>
> * ${\color{white}Bistable}$: We can make it output 0 or 1
> * ${\color{white}Monostable}$: We can make it output 0 or 1, but it will return to it's set default state (auto-reset)
> * ${\color{white}Astable}$: It will oscillate between 0 and 1

### Pinout and datasheet

![alt-text](./archivos/555Pinout.jpg)

[NE555 datasheet](https://github.com/disenoUDP/dis8644-2025-1/blob/main/00-docentes/sesion-03a/archivos/lm555-datasheet.pdf): Una *datasheet* es como un manual, en ella está (o debería estar) toda la información relevante  en cuanto al uso y operaciones de un componente o módulo electrónico, como lo son:
>
> * Operational Voltaje range
> * Current rating
> * Power consumption (Watts)
> * Pinout diagrams
> * Etc.

#### Circuito astable

![alt-text](./archivos/555Circuit1D.jpg)

![alt-text](./archivos/555Circuit1.jpg)

Armamos un circuito que prende y apaga un LED continuamente.

![alt-text](./archivos/555Circuit1a.jpg)

Cambiando el valor del ${\color{#6462fe}capacitor \space C}$${\color{#6462fe}1}$ (conectado al pin 2) y ${\color{#ffe4a8}resistencia \space R}$${\color{#ffe4a8}2}$ (conectada al pin 2, pin 6 y pin 7) aprendimos que mientras menor su capacitancia y menor su resistencia, mayor es la ${\color{White}frecuencia}$ de la oscilación.
>>
>>
>>
>>
>>
>>
>
>
-----------------------------------------------------------------------------------------------------------

## encargo-06

### Einstürzende Neubauten

Escuché el album ${\color{lightGray}"Five \space on \space the \space open-Ended \space Richter \space Scale"}$ , me sorprendió lo caoticos que eran los sonidos de las canciones, a diferencia del 90% de la música que tienen partes definidas que suelen repetirse o mantrenerse constantes.

 Al escucharlos me daba una sensación... como si no tuviesen una estructura, como si estuviesen jugando con los sonidos, haciendo ruido para ver como suena, sin un orden o ritmo definido.

También están los sonidos que se escuchan además de algún que otro instrumento tradicional. Sonidos metálicos, motores, algo que sonaba como un pistón hidraulico... me da la sensación como si estuviesen en un taller mecanico o en una obra en construcción haciendo sonidos golpeando cosas con una llave inglesa o tirando un barril bajo las escaleras.

Tras investigar un poco y ver algunas entrevistas a Blixa, puedo decir que no me esperaba que de verdad tocasen golpeando, raspando, doblando y haciendo quien sabe qué con basura o chatarra que sacaron de un deshuesadero, a pesar que al inicio ello era por necesidad, al no poder costear instumentos.

Aunque supongo que tras ver la filosofia creativa de Blixa tiene sentido, ya que la imprevisibilidad de la vida les dio esos instrumentos, que según menciona Blixa, no podían llevar con sigo en sus giras, por lo que se veian forzados a ir a basurales en busca de nuevos instrumentos para cada performance.

 Lo cual también explica el aparente caos y falta de orden en sus canciones, al preferir los patrones aleatorios y/o accidentales que se producen al no tener tanto control del proceso creativo.
>
-----------------------------------------------------------------------------------------------------------

## Encargo 07

### Understanding the 555

The 555 on the inside:

![alt-text](./archivos/555HowWorks.jpg)

In a nutshell:

> * If voltage on ${\color{white}(Threshold)pin6}$ > ${\color{red}2/3 \space Vcc}$ -> ${\color{#6462fe}capacitor}$ is allowed to discharge and ${\color{white}(Output)pin3}$ = ${\color{white}0}$
> * If voltage on ${\color{white}(Trigger)pin2}$ < ${\color{red}1/3 \space Vcc}$ -> ${\color{#6462fe}capacitor}$ is not allowed to discharge and ${\color{white}(Output)pin3}$ = ${\color{white}1}$
> * If ${\color{white}(Reset)pin4}$ is ${\color{white}grounded \space (GND)}$ -> flip flop resets -> ${\color{#6462fe}capacitor}$ is allowed to discharge and ${\color{white}(Output)pin3}$ = ${\color{white}0}$

#### **Messing with the thing**

![alt-text](./archivos/test1.png)

(Bistable) Pin8 is connected to ${\color{red}Vcc}$, pin1 is connected to ${\color{white}GND}$, Pin3 is connected to an LED, Pin6 is connected to ${\color{red}Vcc}$ through a switch, Pin2 is connected to ${\color{white}GND}$ through a switch and Pin4 is connected to ${\color{red}Vcc}$ through a switch.
>
> When current is allowed to go into Pin6, **Comparator1** receives ${\color{red}9V}$, which is more than the ${\color{white}6V \space (2/3 \space Vcc)}$ its getting from Pin8, therefore it outputs ${\color{white}HIGH}$ or ${\color{white}1}$.
> Pin2 is floating, so **Comparator2** is comparing ${\color{red}3V \space (1/3 \space Vcc)}$ against ${\color{white}0V}$, autputing ${\color{white}HIGH}$ or ${\color{white}1}$.
> In the flip-flop, ${\color{white}R \space == \space 1}$ and ${\color{white}S \space == \space 1}$, which is ${\color{white}invalid}$, but in
> the simulation it did what I wanted, turn off the
> LED. IRL not so much.
>
> To turn the LED back on, we would ${\color{white}ground}$ Pin2 by pressing the button, causing **Comp2** to output ${\color{white}1}$, and with **Comp1** outputing ${\color{white}0}$ (after releasing it's button) we would have: ${\color{white}R \space == \space 0}$ and ${\color{white}S \space == \space 1}$, turning on the LED.
>
> And to turn it off again we could olso ${\color{white}ground}$ pin4, reseting the flip-flop.

![alt-text](./archivos/Test2.png)

En este segundo intento, intentando hacer que al presionar y soltar un botón, un pin pase de estar conectado a ${\color{white}tierra \space (GND)}$ a ${\color{red}Vcc}$ y viendo lo **errático** que era el circuito al tener el pin2 **flotando** (tras haber conectado el pin4 a tierra y haberlo desconectado), me llevó a descubrir el concepto de ***"pull down"*** y ***"pull up resistors"***, lo cual puede que me equivoque, pero parece que hacen justo lo que intentaba hacer.

Also, all of the 555 imputs except pin5 doesn't have internal pull ups (aka, don´t leave them floating)

![alt-text](./archivos/Test2a.png)

Según entiendo, al estar **abierto** el circuito (botón sin apretar), el Pin está conectado a ${\color{white}GND}$ o ${\color{red}Vcc}$, por lo que está reciviendo el voltaje que conlleva estar conectado a ${\color{white}GND}$ o ${\color{red}Vcc}$, pero sin haber **corriente**.

Al presionar el botón, se **cierra** el circuito "interruptor" y el flujo de corriente somete al pin al voltaje de la conección opuesta (de alguna forma, tampoco entiendo pq sin la resistencia no funciona)

![alt-text](./archivos/Test2b.png)

Anyways, al presionar el botón1 (superior), el pin6 que se encuentra conectado a ${\color{white}GND}$ recive ${\color{red}9V}$ al cerrarse el circuito, making **Comp1** = ${\color{white}1}$. Y debido a que el Pin2 esta conectado a ${\color{red}Vcc}$, **Comp2** = ${\color{white}0}$. ${\color{white}R \space == \space 1}$ y ${\color{white}S \space == \space 0}$ = LED apagada.

Y al presionar el botón2 (inferior), el pin2 pasa a recivir ${\color{white}0V}$ al cerrarse el circuito, making **comp2** = ${\color{white}1}$. Y al tener al pin6 conectado a ${\color{white}GND}$, **Comp1** = ${\color{white}0}$. ${\color{white}R \space == \space 0}$ y ${\color{white}S \space == \space 1}$ = LED encendida.

![alt-text](./archivos/Test3.png)

En este circuito monoestable, el LED está apagado, ya que pin 2 está reciviendo cerca de ${\color{red}9V}$, haciendo que **Comp2** = ${\color{white}0}$.
> Pin6 está conectado a un ${\color{#6462fe}capacitor}$ (recordar que corriente no pasa a travez de ellos), a pin7 y a ${\color{red}Vcc}$, por lo que está reciviendo cerca de ${\color{red}9V}$, haciendo que **Comp1** = ${\color{white}1}$.
> ${\color{white}R \space == \space 1}$ y ${\color{white}S \space == \space 0}$ = LED apagada y ${\color{#6462fe}capacitor}$ descargado (pin7 y pin6 conectados a ${\color{white}GND}$ y **Comp1** = ${\color{white}0}$.
> ${\color{white}R \space == \space 0}$ y ${\color{white}S \space == \space 0}$ = flip-flop mantiene estado anterior.

![alt-text](./archivos/Test3a.png)

Al presionar el botón, Pin2 es conectado a ${\color{white}GND}$, **Comp2** = ${\color{white}1}$.
> ${\color{white}R \space == \space 0}$ y ${\color{white}S \space == \space 1}$ = LED encendida, Pin7 desconectado de ${\color{white}GND}$ y ${\color{#6462fe}capacitor}$ se carga y Pin6 recive ${\color{red}Voltaje}$.
>
> Al soltar el botón, Pin2 es receive a ${\color{red}Voltaje}$ y **Comp2** = ${\color{white}0}$.
> ${\color{white}R \space == \space 1}$ y ${\color{white}S \space == \space 0}$ = ${\color{#6462fe}capacitor}$ se descarga, LED apagado (circuito regresa al estado predeterminado).

![alt-text](./archivos/555Circuit1t.png)

El circuito astable se mantiene oscilando por:

Al darle corriente, pin2 está conectado a ${\color{red}Vcc}$ a travez de una **resistencia de 10K y una resistencia variable** ${\color{red}(<1/3Vcc)}$, por lo que **Comp2** = ${\color{white}1}$.
> Pin2 está conectado a pin6 ${\color{red}(<2/3Vcc)}$, por lo que **Comp1** = 0. ${\color{white}R \space == \space 0}$ y ${\color{white}S \space == \space 1}$ = LED encendida y pin7 abierto.
> Tras X milisegundos, el ${\color{#6462fe}capacitor}$ conectado a pin2 y pin6 se carga ${\color{red}(voltaje \space aumenta)}$ y **Comp2** = ${\color{white}0}$ y **Comp1** = ${\color{white}1}$. ${\color{white}R \space == \space 1}$ y ${\color{white}S \space == \space 0}$ = LED apagada y pin7 conectado a ${\color{white}GND}$.
> El ${\color{#6462fe}capacitor}$ se descarga a travez de las **resistencias (10K + Variable)** y pin7.
> El voltaje se reduce, **Comp2** = ${\color{white}1}$ y **Comp2** = ${\color{white}0}$.
> ${\color{white}R \space == \space 0}$ y ${\color{white}S \space == \space 1}$ = LED encendida y pin7 abierto. El ciclo se repite.
> El valor de la **resistencia 10K** afecta el tiempo de carga del ${\color{#6462fe}capacitor}$ | El valor de la **resistencia Variable** afecta el tiempo de carga y descarga del ${\color{#6462fe}capacitor}$ | La capacitancia del ${\color{#6462fe}capacitor}$ afecta el tiempo que tarda en "llenarse" y "vaciarse".
