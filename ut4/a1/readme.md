<center>

# TÍTULO DE LA PRÁCTICA


</center>

***Nombre:***
***Curso:*** 2º de Ciclo Superior de Administración de Sistemas Informáticos en Red.

### ÍNDICE

+ [Introducción](#id1)
+ [Objetivos](#id2)
+ [Material empleado](#id3)
+ [Desarrollo](#id4)
+ [Conclusiones](#id5)


#### ***Introducción***. <a name="id1"></a>

En esta practica haremos una instalacion de wordpres en nuestra maquina de desarrollo debian con nginx.

#### ***Objetivos***. <a name="id2"></a>

Instalar wordpres en nuestro servidor nginx

#### ***Material empleado***. <a name="id3"></a>

* Máquina debian
* MariaDB-server
* Nginx
* Wordpress

#### ***Desarrollo***. <a name="id4"></a>

Primero procederemos con la creación de la base de datos de wordpress con MariaDB

- Configuramos el usuario wpuser.
- Le damos todos los privilegios sobre la base de datos de wordpress.

![](img/001.png)


Descargamos el archivo desde la pagina de wordpress con curl -0 https://wordpress.org/lastest.zip

![](img/002.png)


Descomprimimos el zip descargado.

![](img/003.png)

 despues de haberlo descomprimido lo copiamos en /usr/share

![](img/004.png)


Ahora estableceremos los permisos necesarios para que el usuario web www-data pueda utilizar los ficheros

![](img/006.png)

Editaremos los ficheros de configuracion de la y especificaremos los datos de la siguiente manera:

- El nombre de la base de datos.
- El usuario.
- La contraseña.


En donde dice " database_name_here " , lo sustisuimos por wordpress.bryan.me 

![](img/005.png)

![](img/006.png/)

#### Acceso mediante Nginx

Crearemos un virtual host nuevo en la carptea sites-available de la siguiente manera.

~~~
sudo vi /etc/nginx/sites-available/wordpress.bryan.me
~~~~

![](img/008.png)


Hacemos un reload al nginx y nos vamos al cliente

Importante cambiar el /etc/hosts de la maquina cliente con la ip de nuestro servidor y agregar el dominio para que pueda acceder desde el navegador.


Procedemos a acceder al navegador con wordpress.bryan.me

![](img/009.png)


Escogemos idioma español y procedemos a crear el usuario por el cual accederemos.


![](img/010.png)

![](img/011.png)

Nos iremos a la parte de ajustes y seleccionaremos enlaces permanentes

![](img/012.png)

Seleccionamos el ajuste Día y nombre. Pulsamos en Guardar cambios.

![](img/013.png)

Ahora debemos indicar a Nginx que procese estas URLs:

![](img/014.png)

Recargamos la configuracion de nginx nuevamente.

Por defecto, el límite de subida de archivos para aplicaciones PHP suele ser bastante bajo, en torno a los 2MB, lo incrementaremos de la siguiente manera en nuestra maquina debian.

" Importante, en el archivo 7.2 puede cambiar de nombre dependiendo de la version de php que tengamos instalada."
~~~
 sudo vi /etc/php/7.2/fpm/php.ini
~~~

![](img/016.png)

![](img/017.png)

![](img/018.png)


Además debemos añadir esta linea en el fichero de configuración de Nginx:

![](img/019.png)



Ahora crearemos un post de prueba en el wordpress.

![](img/015.png)


#### ***Conclusiones***. <a name="id5"></a>

En conclusion, esta practica nos ayuda a montar nuestro propio wordpress para realizar una pagina web de manera sencilla.

