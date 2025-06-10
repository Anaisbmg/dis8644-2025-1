# sesion-09b

## Apuntes

### Modulo PAM8403

![alt text](./archivos/pam8403.jpg)

Es un módulo ${\color{#b0e6e6}amplificador}$ clase D de 2 canales (para audio ${\color{#b0e6e6}stereo}$ [${\color{#b0e6e6}L}$ and ${\color{#b0e6e6}R}$ speakers]).

#### Características

* Requiere ${\color{red}5V}$ para operar

* Eficiencia de un 90%

* Puede proveer ${\color{red}3W}$ (${\color{red}Watts}$) a cada canal (${\color{#b0e6e6}R}$ y ${\color{#b0e6e6}L}$) a un parlante de ${\color{#ffe4a8}4Ω}$ y ${\color{red}5V}$

* Circuito de cancelación de ruido integrado en el módulo

* Se apaga y enciende sin hacer ruido

* ${\color{#b0e6e6}Protección}$ contra ${\color{#b0e6e6}corto \ circuitos}$ integrada

#### Especificaciones

* Rango de voltaje de operación: ${\color{red}2.5V-5.5V}$
* Carga del parlante: ${\color{#ffe4a8}4-8Ω}$
* Tamaño: 21 X 18 X 3.4 mm (Largo X Ancho X Alto)

:warning: No conectar las terminales negativas de los canales (R y L) entre sí, o se dañará el módulo

:warning: Conectar el parlante antes de proveer de energía al módulo

### [Pulse Width Modulation (PWM)](https://youtu.be/aeE0u1J-1pg?si=sQ3Hyve-fgqd14Sa)

Ver [Sesión-04b](https://github.com/disenoUDP/dis8644-2025-1/tree/main/25-FranUDP/sesion-04b)

### Persistencia virtual

Es una ${\color{#b0e6e6}ilusión \ óptica}$ que nos permite ${\color{#b0e6e6}percibir \ movimiento}$ al ver una secuencia de ${\color{#b0e6e6}imagenes \ estáticas}$, producto de las imagenes ${\color{#b0e6e6}permaneciendo}$ en nuestra ${\color{#b0e6e6}vista}$ por un período de tiempo después de haberlas visto. En el caso de las LEDs, este fenómeno nos permite percibir un ${\color{#b0e6e6}cambio \ de \ luminocidad}$ al ver ${\color{#b0e6e6}LEDs \ parpadeando \ rápidamente}$

### Diagrama de flujo

![alt text](./archivos/flowChart.png)

Es un ${\color{#b0e6e6}diagrama \ de \ bloques}$ que divide los componentes y acciones que participan en un ${\color{#b0e6e6}circuito}$ para ${\color{#b0e6e6}facilitar}$ el ${\color{#b0e6e6}entendimiento}$ de este y su diseño

### Diodo 1N4148

![alt text](./archivos/1N4148.png)

Diodo de ${\color{#b0e6e6}alta \ velocidad}$ (4ns), con un ${\color{red}forward \ voltage \ de \ 0.7V}$ y un ${\color{darkred}voltaje \ reverso \ de \ 75V}$. Viene en un paquete ${\color{#b0e6e6}DO-35}$ (footprint)

### Voltaje y corriente en un diodo

![alt text](./archivos/diode.jpg)

### Forward  Voltage

Es la ${\color{#b0e6e6}diferencia \ de}$ ${\color{red}voltaje}$ ${\color{#b0e6e6}entre \ el}$ ${\color{red}anodo}$ ${\color{#b0e6e6}y \ el}$ ${\color{white}catodo}$ del diodo, es decir, el ${\color{red}voltaje}$ que recibe el diodo se ${\color{#b0e6e6}reduce}$ en el ${\color{red}forward \ voltage}$
El ${\color{red}forward \ voltage}$ ${\color{#b0e6e6}varía \ dependiendo \ del \ material}$ del diodo

### Threshold Voltage (Voltaje de encendido)

Este es el ${\color{red}voltaje \ mínimo}$ que requiere el diodo para ${\color{#b0e6e6}permitir \ que \ pase \ la \ corriente}$ (bajo el voltaje mínimo hay un flujo minusculo de corriente)
Desde el punto threshold, la ${\color{#b0e6e6}corriente}$ que pasa por el diodo ${\color{#b0e6e6}aumentará \ de \ forma \ exponencial}$

### Modulo relé (relay module)

![alt text](./archivos/relay.gif)

${\color{#b0e6e6}Similar}$ a un ${\color{#b0e6e6}transistor}$, en el sentido que una ${\color{#b0e6e6}señal \ pequeña}$ ${\color{white}(input)}$ ${\color{#b0e6e6}controla \ una \ señal \ más \ grande}$ ${\color{white}(output)}$, Pero ${\color{#b0e6e6}difiere}$ en que la ${\color{white}señal \ controlada \ (output)}$ está ${\color{#b0e6e6}aislada}$ del circuito del cual proviene la ${\color{white}señal \ de \ control \ (input)}$, esto permite que la ${\color{white}señal \ de \ salida}$ sea muchísimo más grande que el ${\color{white}input}$ o incluso que sea de ${\color{red}corriente \ alterna \ (AC)}$

### Other things

### gordon matta clark

![alt text](./archivos/GordonMattaClark.jpg)

Artista y arquitecto chileno-estadounidense conocido por sus intervenciones arquitectónicas, donde hacia cortes y perforaciones en estructuras

### Clases de amplificadores

* Clase D: Amplificadores ${\color{#b0e6e6}electrónicos}$ de ${\color{#b0e6e6}alta \ eficiencia \ energética}$, funcionan usando ${\color{#b0e6e6}PWM}$. Suelen tener más ${\color{#b0e6e6}distorsión}$ que las otras clases y el rápido ON y OFF del PWM puede causar ${\color{#b0e6e6}interferencias \ de \ radiofrecuencia \ (RFI)}$ si no se filtra
* Clase A: Amplificadores ${\color{#b0e6e6}lineales}$ de ${\color{#b0e6e6}alta \ fidelidad}$ (minima distorsión), tienen una ${\color{#b0e6e6}eficiencia \ muy \ baja}$ (25% aprox) y ${\color{#b0e6e6}produce \ mucho \ calor}$, por lo que requieren de enfriamiento
* Clase B: Amplificadores ${\color{#b0e6e6}lineales}$ más ${\color{#b0e6e6}eficientes}$ que la clase A (78% max), sufren de ${\color{#b0e6e6}distorciones}$, por lo que no son aptos para aplicaciones de alta fidelidad
* Clase AB: Tienen ${\color{#b0e6e6}mayor \ eficiencia}$ que la clase A y ${\color{#b0e6e6}menos \ distorsión}$ que la clase B, se suelen utilizar como amplificadored de ${\color{#b0e6e6}propósito \ general}$
* Clase C: Amplificadores ${\color{#b0e6e6}lineales}$ de ${\color{#b0e6e6}alta \ eficiencia}$ y ${\color{#b0e6e6}distorsión \ considerable}$, se suelen emplear en aplicaciones de ${\color{#b0e6e6}radiofrecuencia}$
* Clase H y G: Variaciones de la clase AB, utilizan ${\color{red}múltiples \ voltajes \ de \ entrada \ distintos}$ para ${\color{#b0e6e6}mejorar \ la \ eficiencia}$ energética (varian de menor a major voltaje dependiendo de la señal que estén procesando), la ${\color{#b0e6e6}clase \ G}$ varía entre multiples ${\color{red}voltajes}$ de entrada ${\color{red}fijos}$, mientras que la ${\color{#b0e6e6}clase \ H}$ utiliza una ${\color{red}fuente \ de \ poder \ variable}$

### Mechanical turk

![alt text](./archivos/Turk.png)

Es un ${\color{#b0e6e6}autómata}$ que aparentaba ser un una máquina que operaba por si misma, tomando deciciones por cuenta propia, sin embargo la máquina era ${\color{#b0e6e6}controlada \ por \ un \ enano}$ desde el interior. En la clase fue usada como analogía a la ${\color{#b0e6e6}caja \ negra}$ (${\color{white}inputs}$ y ${\color{white}outputs}$ de un objeto sin saber sus mecanismos de operación)

### Envolvente

![alt text](./archivos/envelope.png)

Es una ${\color{#b0e6e6}curva}$ suave que sigue los puntos más altos de la onda (${\color{#b0e6e6}amplitud}$). Misaa menció haber utilizado un programa que recivia la señal de un micrófono y extraía la envolvente de la señal

### Digital v/s Análogo

${\color{White}Inputs}$ y ${\color{White}outputs}$ ${\color{#b0e6e6}digitales}$ consisten de ${\color{White}HIGHs}$ y ${\color{White}LOWs}$, mientras que los ${\color{White}inputs}$ y ${\color{White}outputs}$ ${\color{#b0e6e6}análogos}$ tienen casi infinitos estados (ej: 1.1 / 1.00000001 / 3.14159...).

### Triodo

![alt text](./archivos/triode.jpg)

${\color{#b0e6e6}Similar \ al \ transistor}$, pero es ${\color{white}controlado}$ por la cantidad de ${\color{red}voltaje}$ y no por la cantidad de ${\color{#b0e6e6}corriente}$. El ${\color{#b0e6e6}triodo}$ es un ${\color{#b0e6e6}tubo \ de \ vacio}$ (vacuum tube), mientras que el ${\color{#b0e6e6}transistor}$ es un ${\color{#b0e6e6}semiconductor}$

## encargo-18

tomen el circuito que simulamos en tinkercad y lo traspasen a su protoboard, usando los componentes que tienen en su kit de materiales

### Circuito IRL

#### Circuito PWM usando el NE555

![alt text](./archivos/circuit1.jpg)

![alt text](./archivos/circuit1A.jpg)

![alt text](./archivos/PWM.gif)

#### Circuito relay

![alt text](./archivos/circuit2.jpg)

![alt text](./archivos/circuit2A.jpg)

![alt text](./archivos/relay.gif)

## encargo-19

estudiar la obra de laurie anderson, incluir citas y referentes usados, explicar qué y por qué les gusta o no de su trabajo

### Laurie Anderson

Escuché el álbum Big science. Inmediatamente me llamó la atención que prácticamente no "canta", sino que habla a distintas velocidades con música repetitiva acompañándola de fondo, porque la mayoría de canciones que he escuchado, cuando incluyen partes habladas, suelen interrumpir la canción y hablar por un período corto antes de retomarla. Tras ver una entrevista que tuvo en el canal 60 minutes <https://youtu.be/rydadItdnt0?si=7jIRZXng869N9_ud>, me sorprendió que ella no busca hacer canciones o temas musicales, sino contar historias de la forma más bizarra que se le ocurra. También mencionó que los sonidos repetitivos de fondo son porque tenía varios equipos que podían hacer loops, aunque no sé si es solo por eso o si hay otros factores detrás.  Aunque no considero que sus canciones sean de mi agrado, me agrada cómo juega con distintos elementos, como sonido, visuales y tecnología en sus obras
