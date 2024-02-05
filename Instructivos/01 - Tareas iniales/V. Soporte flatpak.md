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


#### V.2 - Descarga del gestor de permisos

~~~
flatpak install flathub com.github.tchx84.Flatseal -y
~~~


#### V.3 - Catálogo de recomendaciones

• Inkscape (Editor de imágenes)
~~~
flatpak install flathub org.inkscape.Inkscape -y
~~~


• Mission center (Monitor de recursos)
~~~
flatpak install flathub io.missioncenter.MissionCenter -y
~~~


• OBS (Grabador de pantalla)
~~~
flatpak install flathub com.obsproject.Studio -y
~~~

• VLC (Reproductor multimedia)
~~~
flatpak install flathub org.videolan.VLC -y
~~~


#### V.4 - Gaming

• Steam (Plataforma de juegos)
~~~
flatpak install flathub com.valvesoftware.Steam -y
~~~

• Lutris (Lanzador para plataformas adicionales)
~~~
flatpak install flathub net.lutris.Lutris -y
~~~


## Reemplazos optativos

> **Nota:**
> <p> <p>
>  
> La primera línea corresponde al comando para desinstalar la versión nativa; la segunda a una operación de limpieza y la última consuma el cambio por la versión flatpak


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

#### O.V.2 - Cheese (Cámara)

~~~
sudo apt remove cheese -y
~~~

~~~
sudo apt autoremove
~~~

~~~
flatpak install flathub org.gnome.Cheese -y
~~~


#### O.V.2 - Gnome Videos

~~~
sudo apt install git wget -y
~~~

