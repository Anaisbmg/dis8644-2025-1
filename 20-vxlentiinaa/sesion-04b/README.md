# sesion-04b

04-04-2025

## Apuntes

* _LED_: hay difusos o brillantes
* _Eléctrico_: Pasa algo con los electrones
* _Electrónico_: La información
* _Interfaz_: Es como la piel del objeto electrónico (lo dijo Matías jaja) --> espacio donde convergen dos sistemas

![IMG_3744](https://github.com/user-attachments/assets/efade47e-dcd9-4b60-89cb-314bb4f0929b)

![IMG_3745](https://github.com/user-attachments/assets/e8db375f-37d8-45ca-85d0-c8c071771f49)

### Trabajo en clases

![IMG_3681](https://github.com/user-attachments/assets/317a758d-5f8a-46c2-ad7f-a0554320d75e)

<https://github.com/user-attachments/assets/b9f1a804-7b02-4d42-bb57-7b1b87c75ab9>

<https://github.com/user-attachments/assets/ccfbb276-75c5-49b8-a6b8-5c33fe745dab>

_**Condensador de 100 µF**_
![IMG_3737](https://github.com/user-attachments/assets/b9f54da5-9dbe-48d1-bba0-ad18d879877c)
![IMG_3736](https://github.com/user-attachments/assets/4ee532d4-f85b-4fde-9957-cf3a65042953)

<https://github.com/user-attachments/assets/16538851-90e3-417a-aaba-9ed909ea8316>

_**Condensador de 10 µF**_
![IMG_3740](https://github.com/user-attachments/assets/84043e09-1b78-4687-9bf5-8c2b5067b1c0)
![IMG_3739](https://github.com/user-attachments/assets/7a8768f3-991a-4756-a234-2cef34ffac19)

<https://github.com/user-attachments/assets/34b6f844-d047-4f35-a205-1685bb1765e7>

_**Condensador de 1 µF**_

<https://github.com/user-attachments/assets/c249e57d-856b-43fb-a75c-7cca7f56046b>

_**Condensador de 470 µF**_
![IMG_3743](https://github.com/user-attachments/assets/d5eeeda5-6fdb-47fc-9aa7-c23a063d9135)

<https://github.com/user-attachments/assets/630810e5-d6d4-4234-8087-cae7a510bb35>

### Switched On Bach Wendy Carlos

Switched on Bach es el álbum debut de la compositora estadounidense Wendy Carlos, lanzado en 1968 a través de la discografía Columbia Records. El álbum es una colección de piezas de Johann Sebastian Bach interpretadas por Carlos y Benjamin Folkman en un **sintetizador Moog**, se conoce como música experimental. [https://en.wikipedia.org/wiki/Switched-On_Bach]

Me gustó mucho la combinación de música clásica con algo de electrónica, es completamente diferente a lo que uno suele escuchar y tiene un equilibrio perfecto entre la música con sintetizadores y lo clásico, pero sin sonar demasiado sintético (como robótico?)

![Switched-On_Bach_New](https://github.com/user-attachments/assets/069dddca-3948-477b-b736-7f7615f36be1)

### Proj 1: Bajando opacidad a la caja negra

Con Sofía Cartes, Anais Marschhausen y Valentina Ruz

Nosotras elegimos el Mando de la Xbox 360

* **Contexto**: Es el principal controlador de la consola Xbox 360 de Microsoft. Cuenta con dos versiones la inalámbrica y con cable, ambos son compatibles con PC. La versión inalámbrica requiere de dos baterías AA o recargables, mientras que la versión de cable se conecta directamente a la consola (USB).
* **Diseño**: Cuenta con 11 botones digitales, 2 gatillos analógicos, 2 joysticks analógicos y d-pad digital
* **Métodos de entrada**: 2 palancas analógicas clicables (Left analog stick press - Right analog stick press) 2 gatillos analógicos (Left shoulder trigger - Right shoulder trigger) 2 botones de hombro (Left Bumper - Right Bumper) 4 botones de acción (A B X Y) 3 botones inalámbricos (Back - Start)
* **Batería**: Batería de hidruro de níquel-metal; 2 × AA; Host USB alimentado

* **¿Cómo se utiliza al aparato**: Se conecta por bluetooth o USB hacia la consola. Se utiliza con ambas manos (pulgar e índice)
* **¿Cómo me indica esa manera de uso?***: Por su contexto, ya que se usa en videojuegos y tiene una forma intuitiva
* **¿Quién es el usuario esperado? Condiciones de accesibilidad**: Personas que juegan videojuegos, sus condiciones serían que las personas tengan manos y dedos
* **¿Qué interacción ofrece desde fuera? ¿Hay botones, perillas? ¿Cuántos? ¿Qué grados de control entrega? EXHAUSTIVIDAD**: Hay botones, gatillos, d-pad digital, joysticks
* **¿De donde obtiene energía este aparato?**: Mediante pilas AA o batería recargable
* **Hay una PCB principal? ¿No hay? ¿hay varias? ¿Cómo se interconectan?  ¿Hay números, textos, dibujos? ¿versiones, números de serie?**: Hay una PCB principal, en ella hay números, componentes, letras, números de serie.
* **Realizar diagrama de flujo: ¿Qué placas requieren alimentación? ¿Dónde llegan las interacciones? Usar lenguaje simbólico propio**
![IMG_0183](https://github.com/user-attachments/assets/5c024cbd-562f-41df-be4e-841a3cfa9e66)

Bill of materials. ¿Qué y cuantas partes tiene? de manera general

| Tipo | Qty |
|-----------------|--------|
| Batería | 1 o 2 |
| PCB | 1 |
| R: Resistencia | 60 |
| TP: Transformador de potencia | 407 |
| J: Join: conectores | 9|
| C: Condensadores | 93 |
| L: Inductores | 7 |
| SW: Interruptor | 15 |
| D: Diodo | 4 |
| U: Circuitos integrados | 5 |
| Q: Triodos | 2 |
| Y: Cristal/ Cuarzo | 1 |
| Motor de vibración | 2 |
| Chip H1219 | 1 |
| Chip H1231 | 1 |
| Chip SPB2 | 1 |
| Botones | 17 |

![IMG_0182](https://github.com/user-attachments/assets/9482a2a1-1d72-4963-b2b8-ddca9542ecda)

![IMG_0181](https://github.com/user-attachments/assets/7a722fbb-e49d-4013-9950-73e1bb3e83ce)

<https://github.com/user-attachments/assets/aa920108-868f-4ebe-b115-0cbe1f928fe8>

<https://github.com/user-attachments/assets/30be88b7-f298-4074-9fc3-eb6d8147ac95>

![alt-text](https://github.com/user-attachments/assets/d56ae16d-f2eb-4dc8-9cc6-e32a10aedc9e)

![joystick1](https://github.com/user-attachments/assets/ae09650b-9134-46c1-8dbe-4ffe13be6003)

![joystick2](https://github.com/user-attachments/assets/bd7f9dd8-f0ea-4d1a-84e2-0c7753020e22)
