# ⋆₊˚⊹♡ Clase  12b - Circuitos para un proyecto ♡⊹˚₊⋆

Viernes 30/05/2025

***

## Observaciones

<!---Recordar para programar "md" (markdown): 
- https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet 
- https://www.markdownguide.org/basic-syntax/
[Demasled](https://www.demasled.cl/)
--->

Este día no quería ir. Dado que se ha vuelvo a alterar mi vida personal no tenía mucha energía para poder ir. Al final me obligué a ir, y llegué justo a tiempo.
De la información que alcancé a recapitular fue la obra ["Summer" (2013) de Olia Lialina](https://rhizome.org/editorial/2013/aug/8/olia-lialina-summer-2013/): en esta se observa que a medida que se va recargando la página web una mujer se va comulpiando. Tras ello se comenzó a hablar del artista chileno [Cristian Oyarzún](https://www.error404.cl/coyarzun.htm) y de sus obras digitales perdidas que fueron recuperadas gracias a un fondart. Otro proyecto destacado fue [Posternura Records](https://posternurarecords.cl/). Se habló de las diferencias entre sonidos digitales hechos con ["General midi"](https://es.wikipedia.org/wiki/General_MIDI) y [Virtual Studio Technology](https://en.wikipedia.org/wiki/Virtual_Studio_Technology), los eventos de [Algorave](https://en.wikipedia.org/wiki/Algorave), los softeare [Traktor](https://en.wikipedia.org/wiki/Traktor) y [Sonic Pi](https://sonic-pi.net/).
Luego se habló de las problematicas de la información y privacidad que uno posee, que permiten acceder mediante rastreo los movimientos de la página web de la bip! (lugares en el que se usó, colegio o istitucion perteneciente, etc.) o el carnet de identidad, por ello saltamos al documental [Joshua: Adolescente vs. Superpotencia (2017)](https://en.wikipedia.org/wiki/Joshua:_Teenager_vs._Superpower). Más referentes son [Twitter and tear gas](https://es.wikipedia.org/wiki/Twitter_and_tear_gas), [Anillo web / web ring](https://es.wikipedia.org/wiki/Anillo_web), [WeiweiCam](https://en.wikipedia.org/wiki/WeiweiCam), [Domestic Tension (2017)](https://wafaabilal.com/domestic-tension/), [La privamera Hacker - Chile](https://phacker.org/).

***

## Bitácora digital

### Parte 1: Partes conocidas (y desconocidas) para formar circuitos

#### Fuentes de energía

Batería de 9V, Power bank (batería portátil) y USB A o B (5V), Pantallas solares.

Esta vez me constó nuevamente estar en clases. Sentía que se hablaban de piezas para hacer una categorización de las partes que podemos usar en nuestras propuestas para el examen.
Por ello, decidí prestar más atención a lo que nos decían que a escribir, dado que más tarde podría ir a consultar dicha información al repositorio del equipo.

***
### Copia del listado de los elementos hecho por el [equipo de profesores](https://github.com/disenoUDP/dis8644-2025-1/tree/main/00-docentes/sesion-12b)

#### Fuentes de poder

* Usamos baterías de 9v, pilas AA, AAA, CR2032, entre otras. Lamentablemente son caras y contaminantes. Alternativa: Eliminador de voltaje o fuente de poder AC/DC.

* Powerbank, o más bien todo lo que usb-A o usb-B. Ojo con USB-C porque trabaja con otro estándar.

* También pueden usar pantallas solares como [éstas](https://listado.mercadolibre.cl/mini-panel-solar#D[A:mini%20panel%20solar]).
  Para cargar baterías de litio se requiere un aparato intermediario llamado [BMS](https://afel.cl/collections/cargador-balanceador).
  
Al elejir la fuente hay que considerar:

- Voltaje: hay de 4,5; 5, 7, 9, 12, 15, 18, 25 VDC, etc... ESTAS SON DC, como una batería. Debe ser IGUAL al que espero que se utilice.

- Polaridad: Si el centro es positivo o negativo.

- Tamaño del conector: centro de 2.1mm o 2.5mm.

- Corriente: Recordar esta analogía: el voltaje se entrega, la corriente se pide. Siempre usar una fuente de poder de corriente MAYOR a la que quiero utilizar.

#### Iluminación

* LEDS. Se queman al no tener resistencia.

* Ampolletas domésticas (220V), son peligrosas, hay que tener cuidado. Para controlarlas, usamos RELÉS.

* LEDS de alta potencia. Requieren resistencias también de alta potencia.

* Cintas LEDS son controlables vía PWM y transitor acorde.

Al elejir las luces hay que considerar:

- Muy probablemente requerirán transistores.

- Muy interesante considerar aspectos aditivos de la luz [EJEMPLO](https://lorre-mill.com/spectrabloom).

#### Motores

* Motores DC de 6V. Si le llega electricidad, giran tan rápido como pueden.

* Para que giren más lento hay que usar [motorreductores](https://afel.cl/collections/motorreductores).

* Servomotor: Se suele utilizar con Arduino. Sabe donde está, es preciso, y puede ser rápido. Es a veces inestable.

* [Bomba de agua o de aire](https://afel.cl/products/mini-bomba-de-agua-sumergible-120l-h?_pos=1&_sid=1ab36901a&_ss=r)

#### Transistores

- Se usan como amplificador, como switch, como inversor, o como compuerta lógica

- Hay principalmente dos tipos: BIPOLARES y FET

- Ejemplo bipolar: 2n2222

- Ejemplo MOSFET: IRFZ44n

- Ejemplo transistor modo inversor: <https://es.wikipedia.org/wiki/Puerta_NOT>

#### Sonido

- Parlantes activos y/o pasivos.

- Buzzers. Son parlantes muy básicos, principalmente usados como señal de alarma o aviso. Pueden sonar MUY fuerte

- Micrófonos. Convierte sonido (mecánica) en electricidad. Inverso a un parlante.

- Micrófono piezoeléctrico. Convierte vibración mecánica (sobre materiales) en electricidad.

- Sintetizadores. Generan sonido a partir de señales eléctricas creadas dentro del mismo aparato.

***

### Encargo 24: Descripción de proyectos personales

1. "CONTENEDOR" (CONTENCIÓN) SENSORIAL DE RELAJACIÓN PARA CASOS DE ALERTA EMOCIONAL.

Cómo primera idea se me ocurrió un objeto de dimenciones pequeñas (que no sobrepase el tamaño de un control de mano) que permita a una persona el recibir vibraciones que les puedan relajar en momentos de estrés o ansiedad. Al sentir emociones tan abrumadoras se pierden los sentidos de forma momentánea. Empiezan los dolores, la sudoración excesiva, la sensación de la boca seca, respiración acelerada, el pesar en el pecho, y muchos síntomas que nos generan angustia. Para ello, pensaba en poder generar un aparato que pueda ayudar a calmar a una persona en estos momentos. Me gustaría que se tratase de un objeto que posea varias funciones en uno mismo: que cuente con una pantalla que permita entregar mensajes positivos (Lo haces lo mejor que puedes, Un paso a la vez, etc), que pueda generar vibraciones armoniosas que ayuden a salir del transe frente a la tensión, que permita funcionar con un sensor de frecuencia cardiaca (es más sencillo el saber cuándo uno se encuentra acelerado por el corazón). Considero que también sería interesante el poseer leds que puedan informar el momento de uso, es decir que cuándo se encuentre activo pueda dar una señal que luego se vaya apagando a medida que se relaja.

![image](https://github.com/user-attachments/assets/bc6d79c3-1434-4591-97e6-ecf1c515856d)

▼ Sensor Pulso Cardiaco Corazón. Recuperado de: <https://afel.cl/products/sensor-pulso-cardiaco-corazon?variant=45125252087960>

2 SINTETIZADOR VERDE: MÚSICA DESDE LAS RAICES

Otra ideda que me gustaría realizar sería un sintetizador más complejo que trabaje con plantas para crear pistas de música. Para ello me interesa el poder grabar sonidos base que sean producidos por las frecuencias de energía de cada planta. La idea es poder hacer una mezcla del Atari Punk console y el circuito PWM más complejo, que no sólo trabaje en vivo con un "ser vegetal", sino que pueda hacer pequeñas piezas sonoras que queden registradas. Esta idea se inspira en todos los sintetizadores que hemos visto y que han traído, pero con la inspiración de conectar lo digital con lo natural. Esta idea se inspira en el [Google Doodle de Oskar Fischinger’s de 2017](https://www.google.com/logos/doodles/2017/fischinger/fischinger17.9.html?hl=es-419), el cuál muestra que componer pequeñas piezas de sonido puede ser divertido. Un video que muestra en funcionamiento: <https://www.youtube.com/watch?v=izFtLmpxEMc&ab_channel=CharlesDWright>. La idea necesita aclararse más.

![image](https://github.com/user-attachments/assets/9f77d402-d8ff-4ead-b9ab-722fbd15b071)
▼ Captura del Doodle en función.

***

### Encargo 25: Diagramas, flujos y especulaciones a considerar

***

### Posdata

Estos días mantego la mente en blanco. Busco no sobrepensar como de costumbre, pero aunque no lo quiera a veces se asoman estas ideas y reabren viejas heridas. Siento que no me estoy esforzando lo suficiente para lograr las cosas que quiero. Siento que no me deberían afectar tan a largo plazo la muerte o la perdida de un empleo. A su vez, mi visión se nubla y siento amenazas donde antes no las había. Me da pena ir a clases y sentir que me es complejo interactuar y sentirme parte de un espacio, sobretodo si no me estoy esforzando por estar al tanto con los contenidos y los circuitos fallan constantemente. ૮ ◞ ﻌ ◟ ა
Creo que al igual que muchos, quiero un lugar al que pertenecer y sentirme valorada.
Reflexiones de madrugada mientras pienso en los proyectos.

***

°˖✧◝(⁰▿⁰)◜✧˖°
