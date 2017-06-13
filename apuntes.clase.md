# Apuntes de clase

**Esto pretende ser un repositorio sobre las cosas que vamos viendo en clase y material extra al respecto**

## 1 - Comandos básicos de consola Cygwin

La consola Cygwin es un emulador de la consola de Linux en Windows."Se encarga de que instrucciones para sistemas Unix funcionen en un entorno Windows." Más información sobre Cygwin e instalación [aquí](https://fuubar.wordpress.com/2014/01/14/cygwin-creyendome-un-chico-linux-en-windows-parte-i./). Para profundizar más en los comandos de Linux, mirar [este índice](http://ss64.com/bash/).
<ul>
  <li>
  <code>$</code>Indica que somos usuarios normales.
  </li>
  
  <li>
  <code>#</code> Indica que somos administradores.
  </li>
  
  <li>
  <code>pwd </code>Print Working directory. Te dice el punto de partida en la estructura de ficheros.
  </li>
  
  <li>
  <code>ls</code> Te da información sobre los ficheros que hay en un directorio.
  </li>
  
  <li>
  <code>cd </code>Change Directory. Te traslada a otro directorio. cd / nos lleva a la raíz del sistema.
  </li>
  <li>
  <code>mv </code>cambiar nombre de directorio o fichero. El comando "mv mitexto.txt mitextoNuevo.txt" Cambiara el nombre del fichero mitexto por el otro.
  </li>
  
  <li>
  <code>mkdir nuevaCarpeta</code> Crea una nueva carpeta.
  </li>
  
  <li>
  <code>touch nuevoFichero</code> Crea un fichero.
  </li>
  
  <li>
  <code>file nuevoFichero</code> Te da la metadata de nuevoFichero.
  </li>
   <li>
  <code>echo "Empieza el Readme" > Readme.md</code> Crea un readme con las palabras que están entre comillas.
  </li>
  <li>
  <code>echo "Continua el Readme" >> Readme.md</code> Continua el readme anterior con las palabras que están entre comillas.
  </li>
  <li>
  <code>rm -rf nombreCarpeta</code> Borra una carpeta del sistema. -r quiere decir que se borre todo el contenido de la carpeta. -f quiere decir que se borre absolutamente del sistema.
  </li>
  <li>
  <code>more nombreFichero</code> Ver contenido del fichero
  </li>
  <li>
  <code>unzip nombreZip</code> Descomprimir zip
  </li>
   <li>
  <code>unzip -l nombreZip</code> Te dice lo que contiene el zip. Previene de virus
  </li>
  <li>
  <code>mv nombreDirectorio/ otroDirectorio/</code>mover nombreDirectorio a otroDirectorio
  </li>
   <li>
  <code>mv file.*/ otroDirectorio/</code>mover TODOS los tipos de fichero que lleven el nombre file, a otro directorio
  </li>
   <li>
  <code>mc nombreZip</code> copiar zip
  </li>
  <li>
  <code>cd</code> Volver a la raíz
  </li>
  <li>
  <code>./tabula.exe</code> Abrir Tabula / ejecutar tabula.exe desde consola
  </li>
  <li>
  <code>clear</code> Despejar la consola
  </li>
  <li>
  <code>find . -name Readme.md</code> Encuentra todos los archivos que se llamen Readme.md, empieza en el directorio y se proyecta hacia abajo en la estructura árbol
  </li>
  <li>
  <code>find . -size +300M</code> Encuentra todo lo mayor de 300 megas
  </li>
  <li>
  <code>tail file.js</code> las diez ultimas lineas del js.
  </li>
  <li>
  <code>head file.js</code> las diez  lineas del js.
  </li>
  <li>
  <code>du file.txt</code> lo que ocupa el fichero
  </li>
   <li>
  <code>head -45 file.csv | tail -5 </code> encadenamiento de head y tail
  </li>
   <li>
  <code>mkdir carpeta &amp;&amp; cd carpeta &amp;&amp; pwd </code> concatenamiento de sentencias con &amp;
  </li>
  <li>
  <code>wc -l cabinasCabitelRadio.1921550.xml</code> contar los registros de un dataset
  </li>
  <li>
  <code>grep -rn 28935 cabinasCabitelRadio.1921550.xml | wc -l</code> buscar recursivamente sobre directorio cuantos registros contienen ese codigo postal en el fichero de daros y contarlos
  </li>
  <li>
  <code>curl url</code> descargar url
  </li>
</ul>



### 1.1 - El archivo .bash_history
corresponde a un archivo de registro o logs que guarda los comandos ejecutados en bash por un usuario en particular, cuando un usuario ingresa vía ssh a un sistema por ejemplo, ejecuta los típicos comandos “dir, cd, ls” y estos quedan registrados. [Más información](https://blog.zerial.org/seguridad/cosas-que-encontramos-en-los-archivos-bash_history/).

### 1.2 - Cambiar la ruta absoluta en Cygwin
De la carpeta de instalación a windows. Se hace de la siguiente manera: llendo al archivo de configuración con Emacs (/etc/nsswitch.conf), o navegando a través del interfaz del sistema operativo. Después se abre este archivo (nsswitch.conf) con Emacs o con otro editor de texto y se pone windows en la variable db_home. Dejando comentado lo demás.

## 2 - Atajos en Emacs
Emacs es un editor de texto con una gran cantidad de funciones, muy popular entre programadores y usuarios técnicos. [Mas info](https://es.wikipedia.org/wiki/Emacs).

*<code>ctrl x + ctrl w: guardar archivo</code>
*<code>ctrl + y: pegar</code>
*<code>ctrl x + b: modelo de varios buffers</code>
*<code>ctrl x + 1: salir</code>
*<code>ctrl - x ctrl - f: te lleva a ruta de fichero para abrir</code>
 <code>alt x: cargar un paquete, abrir consola de comandos si le añades term</code>
 <code>ctrl x k:  kill buffer (pantalla)</code>
 <code>packages-install-packages:  instalar</code>

## 3 - Instalando git a través de Cygwin
<ol>
  <li>bajarse el setup de cygwin e inicializarlo</li>
  <li>En select package, elegir <strong>git distributed version control system</strong></li>
  <li>Otros programas que también nos hemos descargado: git teaseratct, imagemagic xpdf</li>
</ol>

## 4 - Pasos en Github
1. <code>echo "Descripcion del fichero" >> Readme.md</code> crear un fichero Readme con una descripción.
1. <code>git init</code> iniciar un repositorio git local en tu máquina.
2. <code>git add README.md</code> vincular al repositorio git el Readme.
3. <code>git commit -m "first commit"</code> realizar un primer commit.
4. <code>git remote add origin https://github.com/Antonio-HR/gds.git</code> añadir al repositorio git remoto, el origen.
5. <code>git push -u origin master</code> subir al repositorio "origin". En la rama master.

### 4.1 - Publicar en la web a través de Github
Si lo que hemos subido es un fichero html, se puede redenrizar en el navegador y por lo tanto, publicar en la web. Github ofrece las ramas <a href="https://pages.github.com/">github-pages</a> para ello. Más información, <a href="https://github.com/flowsta/github#publicación-web">aquí</a>.
## 5 - Open Refine
Open Refine ofrece un lenguaje de programación llamado General Refine Expresions Languages (GREL) muy sencillo y útil para limpiar datos. A continuación, algunas funciones:

| Función      | Nombre        | Descripción  |
| ------------- |:-------------:| -----:|
| <code>value.replace(".","")</code>      | remplazar | remplazar el punto por nada |
| <code>value.replace().replace()</code>     | remplazar en dos pasos      |   el punto concatena |
| <code>value.toNumber()</code> | toNumber()|    convertir string a dato númerico |
|<code>value.toString()</code>| toString()| convertir dato numerico a cadena de caracteres|
||||
||||
||||
||||
||||
||||
||||
||||
||||
||||
||||
||||
||||
||||
||||
||||
||||
||||






   





