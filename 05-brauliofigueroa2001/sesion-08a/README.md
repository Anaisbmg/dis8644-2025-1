# sesion-08a

## taller clase martes 29 de abril

### primera parte

llegué temprano, había poquita gente, en la primera media hora entre 8:30 a 9:00 aaron estuvo revisando bitácoras

apuntes sueltos:

- santi preguntó cómo se podía agregar una gráfica vectorial a la pcb
- se probó con una gráfica de un completinho, al ponerlo en la pcb el archivo no se puede insertar cuando es PNG, para poder ser colocado necesita ser un archivo SVG
- cuando el objeto está puesto se puede desagrupar y podemos manipularlo, por ejemplo, pusieron una imágen de un pretzel y este tenía puntos de relleno. Al desagruparlo se pueden ir modificando y eliminando estos puntitos, es parecido a illustrator
- la segunda forma de hacer esto que es más tediosa mediante el conversor de imágenes
- el conversor de imágenes primero al insertar nuestra imágen (un completo) lo pasará a blanco y negro
- se puede establecer en cuál capa se quiere, ej: máscara de soldadura, serigrafía frontal
- en formato de salida, puedo establecer que sea formato símbolo o huella, en este caso huella
- exportamos archivo y lo guardamos en la carpeta udpudu
- lo agrego manualmente en biblioteca de huellas
- al insertarlo, si viene con un tamaño de imágen preestablecido, quedará de esa forma. Si queremos que sea más pequeño necesitamos conseguir una versión más pequeña de la foto
- **ahora aaron hablará un poco de notas y reclamos**
- Rafael Benguria, un profe físico de aaron en la universidad, era un capo
- se habló de la malla nueva, en esta, habrá una práctica en el sexto semestre ojo
- de bitácoras hay 4 notas, se considerarán 3 y se borrará la peor
- en encargos pasa lo mismo
- cómo mandar un reclamo??? ---> puedo proponer una pull request, si quiero que aaron se haga cargo de esto lo debo asignar, esto significa que en mi modificación aaron se debe hacer cargo de esto porque es la persona a cargo
- aaron pondrá merged en nuestro pull request y de esta forma quedará cerrado
- esto se puede hacer sólo si estoy ahead y no behind
- si es que aaron no acepta mi contribución los demás no pueden ver mis cambios
- otra cosa que están enseñando paso a paso, primerovamos al original y pondremos un issue
- si es una issue para bitácora, en new issue usamos la de bitácora y si es de encargo usamos la de encargo
- al abrirlo, en número de estudiante pongo mi número y sesión ej hoy, 8a
- entonces todos los problemas, reclamos que tengamos, los pondremos en los issues
- APARECIÓ RAFITA STUDIO EN LA CLASE!!!!!!
- @madbuton en github increíble repositorio, nos dieron stickers del lab de interacción digital épico
- **ahora está hablando misaa sobre cambios que hicieron en la pcb**
- agregaron un ícono de parlante
- perforaron las esquinas con círculos
- cómo perforamos? ---> en edgecuts
- en la capa esquemático necesitamos agregar un componente que se llama mounting hole
- los mountinghole son agujeros
- perno, tuerca y golilla existen en el mundo de la fijación, la tuerca no tiene suficiente fuerza para que se salga el perno solo, para esto existe la golilla que fija el agarre. Existen las golillas de presión que giran en sentido opuesto a la tuerca entonces genera un mejor agarre
- agregamos la huella a mounting hole , buscamos m3 y aparece, en este caso es MountingHole:MountingHole_3.2mm_M3
- también existen los separadores pcb
- repaso de cómo exportar el archivo gbr, debo ver la clase otra vez para entenderlo mejor porque aun no logro desarrollar mi udpudu
- en la página de jlcpcb podemos ver las opciones de la pcb y especificaciones físicas, para ver cómo quedó y qué cosa quedó en cada lugar/capa/colores
- en order details veo todo le proceso de envío
- el aduanazo siempre llega, cobran el 6% de arancel aduanero + el 19% del iva, terrible

- ### parte 2 post break

- comenzaremos con openscad en este módulo, ahora aaron tomó el mando
- joseph prusa --- > nació en república checa, prusa3d.com, fue una gran empresa que hizo soluciones de modelos 3d, impresiones 3d
- el próximo proyecto aparte de kicad y esquemático, llevará una carcasa que puede ser en 3d
- makerworld de bambulab
- hay cartelitos con valores paramétricos, puedo cambiar valores de estos parámetros
- quena, qué es? se refería al instrumento pero está hecha mediante parámetros específicos en openscad
- escuchar la cantata santa maría de iquique
- aaron está modificando los parámetros de la quena, esto está cambiando su forma
- OSKITONE un referente que aaron nombró, realizó un proyecto apc (atari punk console) que está abierto para el público, de esta forma nosotros entremos y veamos como está hecho, de hecho aparece en github. El proyecto del APC está hecho en openscad
- existe una forma de clonar los repositorios de github para guardarlos en la nube de nuestro pc
- el antecesor de linux y mac es unix, comparten los mismos comandos
- homebrew, para instalar apps que funcionen en la terminal. Es un administrador de aplicaciones
- githubdesktop, permite administrar las apps sin sufrir
- clonar con github desktop el repositorio que tenemos en la nube y así quedará en nuestro computador
