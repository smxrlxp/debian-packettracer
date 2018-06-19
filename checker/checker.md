# Completar correctamente la verificación del entorno para realizar actividades de Packet Tracer

Para realizar esta verificación debemos iniciar sesión en la plataforma de netacad y acceder a los recursos del estudiante. En el último apartado encontraremos ete verificador aunque dejo este [enlace](https://assessment.netacad.net/check/check.html) para poder acceder directamente iniciando sesión. Este verificador nos descarga un archivo con extensión `.jnlp` el cual deberemos ejecutar mediante la aplicación JAVA o en Debian: IcedTea Java Web Start. Esto permitirá que sepuedan realizar varias comprobaciones. Cuando lo intenté por primera vez me aparecía este error:

![img](https://github.com/smxrlxp/debian-packettracer/blob/master/checker/assets/00.jpg)

La solución es sencilla. Debemos modificar el fichero `/etc/environment`. Este fichero está pensado para situar las variables de entorno en su interior y así hacerlas disponibles para todo el sistema.

![img](https://github.com/smxrlxp/debian-packettracer/blob/master/checker/assets/01.jpg)

Dentro de este fichero tan solo agregaremos esta variable con su ruta:

![img](https://github.com/smxrlxp/debian-packettracer/blob/master/checker/assets/02.jpg)

Una vez modificado el archivo debemos reiniciar el ordenador obligatoriamente. De esta forma cuando volvemos a realizar la verificación, ésta termina con éxito y por lo tanto ya podremos realizar todo los tipos de tareas y exámenes que propone la plataforma.

![img](https://github.com/smxrlxp/debian-packettracer/blob/master/checker/assets/03.jpg)
