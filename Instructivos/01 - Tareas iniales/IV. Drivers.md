# Drivers

Es importante aclarar que la instalación en red de Debian suele descargar el contenido aquí descrito haciendo de esta 


#### IV.1 - Tarjetas de red 

> **Nota:**
> <p> <p>
>  
> Omitir paso en **Debian 12** que los tiene acertadamente instalados por defecto 

• Intel:

~~~
sudo apt install firmware-iwlwifi -y
~~~

• Realtek:

~~~
sudo apt install firmware-realtek -y
~~~


#### IV.2 - Impresoras 

~~~
sudo apt install printer-driver-all -y
~~~


#### IV.3 - Microcódigo para CPU

> **Nota:**
> <p> <p>
>  
> **Debian 12** lo tiene incluído por defecto

• AMD:

~~~
sudo apt install amd64-microcode -y
~~~

• Intel:

~~~
sudo apt install intel-microcode -y
~~~


#### IV.4 - Nvidia 

~~~
sudo apt install printer-driver-all -y
~~~
