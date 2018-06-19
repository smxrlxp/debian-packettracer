# Creación de un acceso directo en el escritorio y en el menú Whisker

En la carpeta de instalación de Packet Tracer podemos encontra un archivo con extensión `.desktop` el cual copiaremos en el Escritorio y editaremos con la herramienta `nano`.

![img](https://github.com/smxrlxp/debian-packettracer/blob/master/link/assets/00.jpg)

Modificamos la línea que aparece marcada y la dejamos como aparece en la imágen.

![img](https://github.com/smxrlxp/debian-packettracer/blob/master/link/assets/01.jpg)

Procedemos a darle permisos de ejecución al archivo que hemos copiado en el escritorio mediante el comando `chmod`.

![img](https://github.com/smxrlxp/debian-packettracer/blob/master/link/assets/02.jpg)

Y por último, copiamos este mismo archivo del escritorio, ya modificado, en la carpeta `/usr/share/applications` para que nos aparezca un acceso directo en el menú Whisker.

![img](https://github.com/smxrlxp/debian-packettracer/blob/master/link/assets/03.jpg)
