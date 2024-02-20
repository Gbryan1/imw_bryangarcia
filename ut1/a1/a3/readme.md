
<center>

# Trabajo con virtual hosts


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

La actividad consiste en configurar 4 sitios web (virtual hosts) en nuestro servidor web Nginx.

#### ***Objetivos***. <a name="id2"></a>

Deberemos crear 4 paginas con 4 virtual host.

#### ***Material empleado***. <a name="id3"></a>

Máquina de desarrollo debian con nginx instalado


#### ***Desarrollo***. <a name="id4"></a>

### Sitio Web1
hacemos los vinculos y los virtual host
![](img/001.png)


Y asignamos la ruta 

Y comprobamos
![](img/002.png)


Después hacemos la carpeta mec 

![](img/003.png)


![](img/004.png)

### Sitio web 2

Hacemos el mismo procedimiento creamos el virtual host y comprobamos en la maquina cliente y ponemos en escucha el puerto 9000

![](img/016.png)


![](img/005.png)

### Sitio web 3

Ahora haremos el virtual host de ssl.bryan.me y prohibimos el acceso al .htpasswd

![](img/007.png)

Creamos el index con la lista de alumnos de 2asir

![](img/008.png)

![](img/009.png)

Comprobamos en la maquina cliente.


Como vemos nos pide el usuario y contraseña que establecimos

![](img/014.png)

Ingresamos con el usuario1 y clave 2asir, y ya nos sale la pagina creada.

![](img/015.png)


### Sitio web 4

creamos los virtual host respectivos

![](img/011.png)

![](img/012.png)

y descargamos el archivo initializr y lo descomprimimos en la carpeta que asignamos en el virtualhost para la ruta

![](img/013.png)

Y comprobamos las entradas desde el navegador

![](img/010.png)


#### ***Conclusiones***. <a name="id5"></a>

En conclusion la practica nos ayuda a crear varios virtual host para nuestro propio servidor web y crear nuestra pagina de una manera eficiente.