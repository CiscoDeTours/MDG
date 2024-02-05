# Flatpak

> **Enfoque:**
> <p> <p>
>  
> Minimizar el problema de paquetes y dependencias rotas usando programas desacoplados del Sistema 

#### V.1 - Instalación

~~~
sudo apt install flatpak
~~~

~~~
sudo apt install gnome-software-plugin-flatpak -y
~~~

~~~
flatpak remote-add --if-not-exists flathub https://dl.flathub.org/repo/flathub.flatpakrepo
~~~

> **Advertencia:** El siguiente comando reinicia el Sistema
~~~
sudo reboot
~~~

#### V.2 - Catálogo de recomendaciones:


• Reprocuctor multimedia:

~~~
sudo apt install git wget -y
~~~

## Reemplazos optativos

> **Nota:**
> <p> <p>
>  
> La primera línea corresponde al comando para desinstalar la versión nativa; la segunda a una operación de limpieza y la última consuma el reemplazo


#### O.I.1 - Libre Office

~~~
sudo apt remove --purge libreoffice* -y
~~~

~~~
sudo apt autoremove
~~~

~~~
flatpak install flathub org.libreoffice.LibreOffice -y
~~~

#### O.I.2 - Gnome Videos

~~~
sudo apt install git wget -y
~~~

