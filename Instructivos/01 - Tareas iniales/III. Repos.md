# Repositorios

#### III.1 - Borrar contenido por defecto

~~~
sudo truncate -s0 /etc/apt/sources.list
~~~

#### III.2 - Cambiar las fuentes

• Introducir componentes generales:

~~~
#DEBIAN 12
deb http://deb.debian.org/debian bookworm main contrib non-free non-free-firmware
deb http://deb.debian.org/debian-security bookworm-security main contrib non-free non-free-firmware
deb http://deb.debian.org/debian bookworm-updates main contrib non-free non-free-firmware

#BACKPORTS
deb http://deb.debian.org/debian bookworm-backports main contrib non-free non-free-firmware
~~~

• Guardar cambios:

Pulsar `CTRL + X` → tecla `S` → tecla `ENTER`


#### III.3 - Agregar la versión instalada de Debian

Habiendo guardado los cambios, es imperativo proceder con el reemplazo de la palabra `DISTRO` con la `versión` instalada del SO usando privilegio root.


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
