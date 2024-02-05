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


#### V.2 - Gestor de permisos:

~~~
flatpak install flathub com.github.tchx84.Flatseal -y
~~~


#### V.3 - Catálogo de recomendaciones:

• Inkscape (Editor de imágenes)

~~~
flatpak install flathub org.inkscape.Inkscape -y
~~~

• OBS (Grabador de pantalla)
~~~
flatpak install flathub com.obsproject.Studio
~~~

• Steam (Plataforma de juegos)

~~~
flatpak install flathub com.valvesoftware.Steam -y
~~~

• VLC (Reproductor multimedia)

~~~
flatpak install flathub org.videolan.VLC -y
~~~


## Reemplazos optativos

> **Nota:**
> <p> <p>
>  
> La primera línea corresponde al comando para desinstalar la versión nativa; la segunda a una operación de limpieza y la última consuma el reemplazo


#### O.V.1 - Libre Office

~~~
sudo apt remove --purge libreoffice* -y
~~~

~~~
sudo apt autoremove
~~~

~~~
flatpak install flathub org.libreoffice.LibreOffice -y
~~~

#### O.V.2 - Gnome Videos

~~~
sudo apt install git wget -y
~~~

