# Docker + Python 
- - -
# Creamos un contenedor sencillo de phyton

```docker run -it --rm -v "$PWD":/usr/src/myapp -w /usr/src/myapp python:3 python main.py```
 
``docker`` el comando base, es el daemon.
 
``run`` crear el contenedor.

``-it`` dos opciones que me valen para interactuar con la terminal del contenedor.

``--run`` borra el contenedor cuando finaliza la acción. 

``-v`` define el mapeo del volumen a continuación. 
 
- ``\$PWD`` el directorio donde estamos.
- ``/usr/src/myapp`` el directorio dentro del contenedor.

``w`` el directorio de trabajo (_workdir_).
 
``python:3`` la imagen de la que se creará el contenedor.

``python main.py`` es el comando para ejecutar dentro del contenedor.