# Instalación de Packet Tracer en Debian 9 (Stretch)
El primer paso será descargarnos de la página oficial de netacad la carpeta comprimida con los archivos de instalación de Packet Tracer. Para ello tendremos que iniciar sesión en nuestra cuenta y acceder a esta página: https://www.netacad.com/group/offerings/packet-tracer/.

![img](https://github.com/smxrlxp/debian-packettracer/blob/master/installation/assets/00.jpg)

Una vez descargado, procederemos a descomprimir los archivos y volcarlos en una carpeta que hemos creado.

![img](https://github.com/smxrlxp/debian-packettracer/blob/master/installation/assets/01.jpg)

El siguiente paso será acceder a la carpeta en la que hemos volcado los archivos y ejecutar el archivo de instalación como podemos ver en la imágen. Al empezar la instalación nos pedirá que presionemos la tecla ENTER para leer la licencia y más tarde aceptar los términosde esta.

![img](https://github.com/smxrlxp/debian-packettracer/blob/master/installation/assets/02.jpg)

Seguidamente, nos preguntará si aceptamos los términos de licencia, los cuales aceptaremos si estamos de acuerdo. También pedirá que introduzcamos un lugar de instalación donde presionaremos la tecla ENTER para que lo instale en la ruta que viene por defecto. Y por último, nos preguntará si queremos que cree un link simbólico para que podamos ejecutar Packet Tracer mediante el comando `packettracer`, a lo que responderemos que sí.

![img](https://github.com/smxrlxp/debian-packettracer/blob/master/installation/assets/03.jpg)

Una vez instalado, iniciaremos Packet Tracer mediante el archivo ejecutable creado. Utilizamos el siguiente comando: `/opt/pt/bin/PacketTracer7`. En este momento aparece el primer fallo que se causa por la falta de algunas librerias.

![img](https://github.com/smxrlxp/debian-packettracer/blob/master/installation/assets/04.jpg)

Para descargar este paquete accederemos a la siguiente página de descarga en la que podremos descargar el paquete según la localización en la que nos encontremos o prefiramos.

https://packages.debian.org/jessie-backports/amd64/libssl1.0.0/download

![img](https://github.com/smxrlxp/debian-packettracer/blob/master/installation/assets/05.jpg)

Una vez descargado, procedemos a intalarlo de la forma en que vemos en la siguiente imágen.

![img](https://github.com/smxrlxp/debian-packettracer/blob/master/installation/assets/06.jpg)

A partir de ahora cuando intentamos iniciar Packet Tracer de la misma forma que anteriormente, nos aparecerán algunos fallos por la falta de otros paquetes que no deberemos descargar porque ya se encuentran en los repositorios de debian. Estos paquetes pueden ser los siguientes:

```
sudo apt-get install qtmultimedia5-dev
sudo apt-get install libqt5webkit5-dbg
sudo apt-get install libqt5script5
sudo apt-get install libqt5scripttools5
```

![img](https://github.com/smxrlxp/debian-packettracer/blob/master/installation/assets/07.jpg)

![img](https://github.com/smxrlxp/debian-packettracer/blob/master/installation/assets/08.jpg)

Una vez instalados todos los paquetes que nos pide, procederemos a iniciar de nuevo Packet Tracer pero esta vez con éxito.

![img](https://github.com/smxrlxp/debian-packettracer/blob/master/installation/assets/09.jpg)

![img](https://github.com/smxrlxp/debian-packettracer/blob/master/installation/assets/10.jpg)
