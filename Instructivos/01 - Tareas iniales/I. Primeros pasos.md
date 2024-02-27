# Primeros pasos

#### I.1 - Cambiar el funcionamiento del touchpad en laptops

~~~
gsettings set org.gnome.desktop.peripherals.touchpad click-method areas
~~~

> **Advertencia:**
> <p> <p>
>  
> Para pegar este comando con la extraña configuración que en ciertos casos está habilitada por defecto debe pulsarse el touchpad con dos dedos al mismo tiempo. De persistir problemas, es recomendable usar un mouse.



#### I.2 - Unificar la hora con Windows

~~~
timedatectl set-local-rtc 1 --adjust-system-clock
~~~



#### I.3 - Convertirse en usuario SUDOER

• Identificar nombre de usuario en la Consola:

> **Nota:**
> <p> <p>
>  
> Es aquel de color verde que se encuentra al lado izquierdo de la arroba 

**nombre**@debian:~$


• Adquirir privilegio root:

~~~
su
~~~


• Agregar usuario al grupo SUDO:
 
`sudo usermod -aG sudo` `nombre`


• Reiniciar el Sistema:

~~~
sudo reboot
~~~

