## Ejercicio 05

* HEALTHCHECK

Se encarga de indicarle al daemon de Docker cómo comprobar que el contenedor se encuentre funcionando. Esta instrucción permite que el sistema sea capaz de detectar casos de errores.

* ONBUILD

`ONBUILD` agrega a la imagen una instrucción trigger que se ejecutará cuando la imagen se use como base para otra compilación. El trigger se ejecutará en el contexto de la compilación descendente, como si se hubiera insertado inmediatamente después del `FROM` en el Dockerfile.

* VOLUME

El comando VOLUME especificará un punto de montaje en el contenedor. Este punto de montaje se asignará a una ubicación en el host que se especifica cuando se crea el contenedor o, si no se especifica, se elige automáticamente desde un directorio creado en `/var/lib/docker/volumes.`
Si el directorio elegido contiene archivos, estos archivos se copiarán en el volumen. 