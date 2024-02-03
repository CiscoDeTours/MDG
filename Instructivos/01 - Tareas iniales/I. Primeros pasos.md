# Primeros pasos

#### I.1 - Cambiar el funcionamiento del touchpad en laptops

~~~
gsettings set org.gnome.desktop.peripherals.touchpad click-method areas
~~~

> **Advertencia:**
> <p> <p>
>  
> Para pegar este comando con la extraña configuración que en ciertos casos está habilitada por defecto debe pulsarse el touchpad con dos dedos al mismo tiempo. De persistir problemas, es recomendable usar un mouse



#### I.2 - Unificar la hora con Windows

~~~
timedatectl set-local-rtc 1 --adjust-system-clock
~~~



#### I.3 - Convertirse en usuario SUDOER

> **Nota:**
> <p> <p>
>  
> Se requiere de privilegio root para proseguir

~~~
su
~~~

> **Advertencia:**
> <p> <p>
>  
> El nombre de usuario es aquel que se encuentra a la izquierda de la arroba **usuario**@debian


    
`sudo usermod -aG sudo` + `usuario`

> **Advertencia:** El siguiente comando reinicia el Sistema
~~~
sudo reboot
~~~

