
<center>

# Mis series favoritas


</center>

***Nombre:*** Bryan Garcia
***Curso:*** 2º de Ciclo Superior de Administración de Sistemas Informáticos en Red.

### ÍNDICE

+ [Introducción](#id1)
+ [Objetivos](#id2)
+ [Material empleado](#id3)
+ [Desarrollo](#id4)
+ [Conclusiones](#id5)


#### ***Introducción***. <a name="id1"></a>

Realizaremos una pagina con un servidor nginx y docker

#### ***Objetivos***. <a name="id2"></a>

 Crear una página web que nos enlace a tus 5 series favoritas. Realizaremos este proceso de dos formas: en la máquina de producción y en docker

#### ***Material empleado***. <a name="id3"></a>
Maquina de produccion 

-Debian
-Docker instalado
-Nginx instalado

#### ***Desarrollo***. <a name="id4"></a>

Primero verificaremos que esten instalado el docker y el nginx.

Luego crearemos nuestra pagina en html y la colocaremos en la ruta /var/www/html/series

![](img/001.png)


colocamos en el fichero /etc/hosts la ip de la maquina servidor nginx para que pueda conectarse con  bryan/series/


![](img/004.png)

![](img/006.png)



#### ***Conclusiones***. <a name="id5"></a>

En esta practia hemos aprendido a montar nuetro propio servidor web a la hora de subir sitios a la red.