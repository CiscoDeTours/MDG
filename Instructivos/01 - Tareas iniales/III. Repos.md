# Repositorios

#### III.1 - Abrir la lista de fuentes y borrar su contenido

~~~
sudo nano /etc/apt/sources.list
~~~

Pulsar la tecla `SUPR` a fondo

~~~

~~~

#### III.2 - Cambiar las fuentes

• Introducir componentes generales:

~~~
#REPOSITORIOS
#DE DEBIAN 12 EN ADELANTE

deb http://deb.debian.org/debian trixie main contrib non-free non-free-firmware
deb http://deb.debian.org/debian-security trixie-security main contrib non-free non-free-firmware
deb http://deb.debian.org/debian trixie-updates main contrib non-free non-free-firmware
~~~

~~~
#REPOSITORIOS
#HASTA DEBIAN 11

deb http://deb.debian.org/debian DISTRO main contrib non-free
deb http://deb.debian.org/debian-security DISTRO-security main contrib non-free
deb http://deb.debian.org/debian DISTRO-updates main contrib non-free
~~~

• Guardar cambios:

Pulsar `CTRL + X` → tecla `S` → tecla `ENTER`


#### III.3 - Agregar la versión instalada de Debian

Habiendo guardado los cambios, es imperativo proceder con el reemplazo de la palabra `DISTRO` con la `versión` instalada del SO usando privilegio root.

> **Ejemplos:**
> <p> <p>
>
> 
> • Debian **12**
> ~~~
> su
> ~~~
> ~~~
> sed -i 's/DISTRO/bookworm/g' /etc/apt/sources.list
> ~~~
> ~~~
> exit
> ~~~
>
> • Debian **11**
> ~~~
> su
> ~~~
> ~~~
> sed -i 's/DISTRO/bullseye/g' /etc/apt/sources.list
> ~~~
> ~~~
> exit
> ~~~
>  
> • Debian **10**
> ~~~
> su
> ~~~
> ~~~
> sed -i 's/DISTRO/buster/g' /etc/apt/sources.list
> ~~~
> ~~~
> exit
> ~~~

#### III.4 - Añadir la arquitectura de 32 bits 

~~~
sudo dpkg --add-architecture i386
~~~


#### III.5 - Confirmar la adición de las fuentes

~~~
sudo apt update
~~~


#### III.6 - Forzar actualización del Sistema para estar al día

~~~
sudo apt upgrade
~~~

Pulsar tecla `S` → tecla `ENTER`
