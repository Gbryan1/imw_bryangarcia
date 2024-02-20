<center>

# Listado de directorios


</center>

***Nombre:*** Bryan Garcia Gallego
***Curso:*** 2º de Ciclo Superior de Administración de Sistemas Informáticos en Red.

### ÍNDICE

+ [Introducción](#id1)
+ [Objetivos](#id2)
+ [Material empleado](#id3)
+ [Desarrollo](#id4)
+ [Conclusiones](#id5)


#### ***Introducción***. <a name="id1"></a>


La actividad consiste en permitir el acceso al contenido de un subdirectorio dentro de la ruta raíz de Nginx, enlazando una serie de ficheros desde ahí. Se debe realizar de dos formas en la máquina virtual y en docker.



#### ***Objetivos***. <a name="id2"></a>

Realizaremos un host web nginx y mostraremos los archivos correspondientes con enlaces publicos.



#### ***Material empleado***. <a name="id3"></a>


Maquina Debian con nginx instalado
Maquina ubuntu



#### ***Desarrollo***. <a name="id4"></a>

Primero creamos el virtual host

![](img/002.png)


Hacemos el enlace

![](img/003.png)


 Y hacemos los enlaces con los archivos en la ruta de la pagina
![](img/004.png)

Comprobamos

![](img/005.png)



#### ***Conclusiones***. <a name="id5"></a>

En conlusion aprendimos a enlazar archivos y tenerlos en otra carpeta sin necesidad de copiarlos.