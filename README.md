Spriterizer 7D0 es un archivo de Blender (v4.3.2) donde renderiza modelos 3D o imágenes 2D y las convierte a ASM/BIN (u otros) para que se carguen en cualquiera de las 18 siguientes plataformas:
Amiga, Macintosh 128/512K, Intellivision, NES, ZX Spectrum, Amstrad CPC, PC compatible (CGA), Commodore 64, MSX, BBC Micro, Game Boy, Master System, Oric, Mega Drive, Apple II, Amstrad PCW, Atari ST, VIC-20.
Una muestra de lo que puede hacer Spriterizer 7D0 se encuentra en esta charla de CanariasGoRetro:
https://www.youtube.com/watch?v=uKpu92lfj7c
Si quieres probarlo, te paso unos consejos básicos, ya que está todo un poco patas arriba:

1.- Por ahora, lo mejor es ejecutar el código directamente dándole al botón del Play que hay a la derecha del nombre del código (puedes cambiar entre los distintos códigos para cambiar de plataforma). ¡OJO! Muchos de los códigos tienen rutas a carpetas que se deberían cambiar por rutas de tu preferencia.

2.- En algunos códigos se puede cambiar el tamaño del sprite en las variables correspondientes, pero a veces estas variables están enlazadas con la pestaña de Render, así que puedes cambiar el tamaño directamente ahí.

3.- Después de poner bien la resolución, lo interesante es darle a F12 para hacer un primer render. Ese render seguramente no saldrá en un inicio con la configuración adecuada, ya que hay que cambiar la plataforma en la que se quiere exportar. Haciendo zoom en la ventana de nodos, hay una lista grande donde salen las plataformas y su número asociado. Entonces, si por ejemplo queremos exportar a Atari ST, tenemos que cambiar el número flotante que aparece debajo en un nodo llamado Tipo, donde escribiremos 15. Si queremos ver el render en formato Oric, pondremos 17. Y así con el resto.

4.- Una vez tenemos la plataforma adecuada tanto en la ventana render como en el código, seguramente hará falta cambiar los colores para que salgan como uno desearía. Para ello, hay que buscar en la maraña de nodos el que corresponda a la plataforma deseada. Si queremos exportar un sprite para Amstrad CPC, por ejemplo, iríamos a los nodos que están más a la izquierda, donde hay una etiqueta que pone Amstrad CPC. Ahí se ven los 27 colores del Amstrad CPC representados con sus números (negro=1, gris=2, blanco=3, etc.). En los nodos que están encima de los colores se ponen los números de los colores que queremos, y debajo se elige el rango para cada color (cambiando esos números, habrá más de un color, o menos de ese color). 

5.- El problema es que cada plataforma tiene sus nodos específicos y algunos son bastante complicados. Hay otros, en cambio, que son más sencillos, como el de Amiga o Mega Drive, porque al tener tantos colores, simplemente hay que cambiar el brillo y poco más.

6.- Una vez tenemos todo eso configurado, le damos al Play que está a la derecha del nombre del código. Si has configurado correctamente las rutas, se generarán esa carpeta uno o varios archivos. Por lo general, el código está preparado para convertir a formato TAP, Z80, PRG, EXE, COM, etc.... ya que para probar los ASM/BIN finales, se ha aprovechado también para convertir a un formato que lea la plataforma directamente y comprobar que efectivamente se ve bien. El problema con eso es que en muchos casos hay que compilar/ensamblar con algún compilador/ensamblador que yo he descargado y que tengo en mi proyecto. En tu caso, lo más seguro es que el código falle porque no encuentra el ensamblador en la ruta especificada. Puedes comentar toda esa parte, o me puedes preguntar y te digo qué ensambladores he usado. 

Tú pregúntame sin miedo, que yo te ayudo a que ésto tire p'alante.
Mi correo: panchete@gmail.com
