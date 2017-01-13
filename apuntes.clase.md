# Apuntes de clase

**Esto pretende ser un repositorio sobre las cosas que vamos viendo en clase y material extra al respecto**

## 1 - Comandos básicos de consola Cygwin

La consola Cygwin es un emulador de la consola de Linux en Windows."Se encarga de que instrucciones para sistemas Unix funcionen en un entorno Windows." Más información sobre Cygwin e instalación [aquí](https://fuubar.wordpress.com/2014/01/14/cygwin-creyendome-un-chico-linux-en-windows-parte-i./). Para profundizar más en los comandos de Linux, mirar [este índice]("http://ss64.com/bash/").

   <pre>$ Indica que somos usuarios normales.</pre>
   <pre># Indica que somos administradores.</pre>
   <pre>pwd Print Working directory. Te dice el punto de partida en la estructura de ficheros</pre>
   <pre>ls Te da información sobre los ficheros que hay en un directorio</pre>
   <pre>cd Change Directory. Te traslada a otro directorio. cd / nos lleva a la raíz del sistema.</pre>
  <pre>mv cambiar nombre de directorio o fichero. El comando "mv mitexto.txt mitextoNuevo.txt" Cambiara el nombre del fichero mitexto por el otro.</pre>
   <pre>mkdir nuevaCarpeta. Crea una nueva carpeta.</pre>
   <pre>touch nuevoFichero. Crea un fichero</pre>
   <pre>file nuevoFichero. Te da la metadata de nuevoFichero</pre>
   <pre>rm -rf nombrecarpeta. Borra una carpeta del sistema. -r quiere decir que se borre todo el contenido de la carpeta. -f quiere decir que se borre absolutamente del sistema.</pre>
   <pre>more .nombreFichero. Abrir fichero</pre>
### 1.1 - El archivo .bash_history
corresponde a un archivo de registro o logs que guarda los comandos ejecutados en bash por un usuario en particular, cuando un usuario ingresa vía ssh a un sistema por ejemplo, ejecuta los típicos comandos “dir, cd, ls” y estos quedan registrados. [Más información].("https://blog.zerial.org/seguridad/cosas-que-encontramos-en-los-archivos-bash_history/")

## 2 - Atajos en Emacs
Emacs es un editor de texto con una gran cantidad de funciones, muy popular entre programadores y usuarios técnicos. [Mas info]("https://es.wikipedia.org/wiki/Emacs").
*     ctrl x + ctrl f
en emacs: te lleva a ruta de fichero para abrir
*     ctrl x + ctrl w
en emacs: guardar archivo
*     ctrl y
pegar
*     ctrl x + b
modelo de varios buffers
*     ctrl x + 1
salir
   





