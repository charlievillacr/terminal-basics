# Introducción a Terminal y Línea de Commandos

## Clases

1. ¿Que es y para que sirve?
2. Árbol de directorios y navegación
3. Manipulación y modificación del árbol de directorios
4. Herramientas básicas
5. Variables y entorno
6. Streams
7. Procesos de terminal
8. Power Tools - Comandos poderosos de búsqueda
9. Power Tools: curl, zip y tar
10. Pipe
11. Crontab - Una herramienta para automatizat tareas de la terminal
12. Links
13. Usuarios y Permisos
14. Que sigue después de aprendar a usar la terminal

### 1. Qué es la terminal y para qué sirve

- Bienvenido al curso de terminal y línea de comandos. En este curso aprenderás una serie de tips y hacks que te van a ayudar a manejar la terminal como si no existiera una interfaz gráfica. La línea de comandos te permite hacer de todo: configuraciones, editar texto, compilar código y utilizar las herramientas que existen dentro de tu sistema operativo.

- En el curso estaremos utilizando la terminal de UNIX. Windows cada vez se acerca más a la capacidad de esta terminal, aunque todavía hay diferencias. Todos los comandos que se ejecuten aquí puedes buscarlos con el comando man y ver cuáles son los correspondientes, si estás utilizando Windows.

- Aprender a utilizar la línea de comandos te ayuda a ahorrar un montón de tiempo y memoria, pues puedes hacer más sencillo tu trabajo y hacerlo más liviano sin ningún tipo de interfaz gráfica.

- En la siguiente clase vamos a ver cómo navegar y conocer nuestro árbol de directorios desde la terminal.

### Comandos ls

- ls /usr/bin | wc -l

## 2. Árbol de directorios y navegación

### Comandos arbol de directorios

- ls

- ls -l

- pwd = presente directorio

- cd nombre-del-file = ir a ese direcrorio o file

- cd .

- cd .. = subir de directorio

- ~ = ir a home

- cd ~ = ir a home

- cd = ir a home

## 3. Manipulación y modificación del árbol de directorios

### Comandos clase 3

1. touch filename.ext = si no existe lo va crear en blanco
2. clear = limpiar pantalla
3. control + l = limpiar pantalla
4. commando + k = limpiar pantalla
5. mkdir folder-name = crear una carpeta
6. ls -lh
7. cambiar nombre = mv pruebas tests
8. mv directorio-actual directorio-nuevo-nombre
9. rm borarr de forma definitiva
10. rm -r = borrar directorios y contenidos
11. man = manual entry
12. mv file-name dir-name/
13. cp = copy
14. crp filename.ext ../\ = folder actual y el de arriba
15. ls -l .. = listar el directorio siguiente
16. cp file-name.ext ~/src/git/whatever/ = elegir dir
17. pwd = present working directory
18. pushd ~/sites/terminal-platzi/sandbox = elegir directorio local

### Notas del profe

1. mkdir: crea un directorio
2. touch: crea un archivo. Si no existe el archivo lo va a crear, y si existe - le cambia la fecha de modificación
3. mv: mueve un archivo, te ayuda a modificarlo
4. rm: elimina archivos o links, no funciona para eliminar un directorio, para esto necesitas un poco más
5. rm -rf: elimina un directorio recursivamente
6. man: es el manual de la terminal, puedes utilizarlo cuando tu quieras para entender qué hace un comando y sus banderas. Con espacio pasas una página, - con b te regresas una página y con q sales del manual.
7. cp: copia un archivo a otros directorios
pushd y popd: te permiten navegar entre dos directorios fácilmente.

## 4. Herramientas básicas

1. more: te da las primeras líneas de lo que hay en el archivo. Para ver la siguiente página hacemos lo mismo que con el man, utilizamos espacio para
2. cat: imprime todo el contenido de un archivo en pantalla.
3. tail: te muestra las últimas 10 líneas de un archivo. Puedes agregarle un número con el - y pedir más que 10 líneas.

## 5. Variables y entorno

- Cada vez que abrimos la terminal en realidad se está ejecutando un programa que se llama .bash_profile que es una serie de comandos que da de alta unas variables.

- Todos los ejecutables tienen una serie de permisos. Cada vez que tengo un nuevo programa tengo que asegurarme

### Comandos variables y entorno

- alias: ejecuta una serie de comandos que le pasas antes, funciona para crear variables.

## 6. Streams

- El diagrama que ves en pantalla consiste en un input y en un output. Nosotros pasamos unos datos que son procesados y que luego se devuelven de alguna forma. Cuando nosotros enviamos datos, eso es STDIN (standard input), después de eso se ejecuta un script y finalmente hay dos opciones de respuesta STDOUT (standard output) o STDERR (standard error). Es importante entender esto, sobre todo porque es fundamental saber cuándo estás teniendo un error dentro de un proceso.

- En el ejercicio verás cómo corre un programa en php que identifica cuáles números son y no son múltiplos del número que ingresas. Ahí verás dos tipos de salida: STDOUT que arrojará los múltiplos y STDERR que arrojará los números que no son múltiplos del número que ingreses. Cada salida se podrá enviar a un archivo diferente y se podrá concatenar con las respuestas si ingresas un número nuevo. Además veremos cómo enviar los dos tipos de salida al mismo lugar.

## 7. Procesos de terminal

- Cada vez que ejecutamos algo en nuestra computadora es un proceso que está registrado de alguna forma. El orden en que esto se ejecuta y la cercanía del procesador son muy importantes para las prioridades que se le va a dar a dicho proceso.

- En esta clase vas a aprender a revisar, manipular y matar los procesos que corren dentro de tu computadora.

### Comandos de procesos de terminal

1. top muestra todos los procesos del equipo
2. PID ID del proceso
3. O para que te ordene por una categoría
4. kill -9 mata un proceso
5. & manda un proceso a background
6. ; encadena los comandos para cuando termine el primero ejecuta el segundo
7. ps -wA te da una lista de los procesos que se están ejecutando
8. uptime te dice el tiempo que ha estado prendido

## 8. Power Tools - Comandos poderosos de búsqueda

### Commandos de búsqueda

<!-- Grep: Herramienta que nos ayuda a buscar cadenas carácteres. -->

- grep file.ext -4 Comedy

- grep file.ext -4 Comedy | wc -l = Cuantas?

- find . -name *.php -type f

- find . -name *.php -type f

- find . -name *pl

- ls *jpg

- ls -lh *php

- find . -name *php

- wc -l resultados

## 9. Power Tools: curl, zip y tar

<!-- Linx browser para terminal -->

## Curl command

- curl

- curl https://raw.githubusercontent.com/jpatokal/openflights/master/data/airports.dat

- Va internet trae el archivo, manda las cookies y solo lo imprime en pantall

- curl https://raw.githubusercontent.com/jpatokal/openflights/master/data/airports.dat > aeropuertos.csv

- Descarga el file y lo guarda como un .csv

## 10. Pipe

## 11. Crontab - Una herramienta para automatizar tareas de la terminal

## 12. Links

## 13. Usuarios y Permisos

## 14. Que sigue después de aprendar a usar la terminal
