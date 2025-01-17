# Respuestas

### Indica tu nombre a continuación: 
#### David Carvallo

## ETAPA 1

### ¿Cuál es la diferencia entre los archivos con el verbo `Create` con los archivos con el verbo `Add`?
>R: Create crea tablas o estructuras en la base de datos y Add añade entradas a la base de datos

### ¿Cómo se llama el servicio que se declara en el archivo `docker-compose.yml`?
>R: Flyway

## ETAPA 2

### ¿Qué pasa si cambias el nombre del servicio de `postgres` a `db`? ¿Qué otros cambios tendrías que hacer?
>R: Al cambiar el nombre del servicio de postgres a db docker creara una nueva imagen de postgres con el nombre db por lo que sera necesario cambiar tambien las variables POSTGRES_USER además de la seccion depends_on en el docker-compose.yml

## ETAPA 3

### ¿Qué te llama la atención?
>R: Un aspecto que podria llamar la atencion del Dockerfile seria el uso de Multi-stage Build en este, el cual en este caso permite destinar un stage para el build del desarrollo en una imagen especifica de golang, para luego utilizar el binario construido en otra imagen de tipo distroless. De esta manera se optimiza el tamaño final de la imagen.

### ¿Cómo se relacionan el archivo `docker-compose.yml` y el archivo `movies-api/Dockerfile`?
>R: La relacion va en que el archivo docker-compose.yml en la seccion del service movies-api realiza el build de la imagen utilizando el Dockerfile presente en movies-api/Dockerfile

### ¿Qué crees que hace el atributo `context` debajo de `build` (está en la linea 6 del archivo `docker-compose.yml`)?
>R: El atributo context lo que hace es indicar donde se encuentra el archivo Dockerfile y ademas indicar el contexto o grupo de archivos con el cual podra trabajar el Dockerfile en la construccion de la imagen.

## ETAPA 4

### Compara el atributo `build` del servicio `movies-api` con el de `movies-front`. 
### ¿Cuál es la diferencia?
>R: La diferencia radica en que en movies-api el contexto (En este caso la carpeta en la cual se encuentra el Dockerfile y archivos especificos para cosntruir cada servicio) se define como una clave "context" dentro de build mientras que en movies-front se define de manera directa como un string dentro de "build". Con la manera utilizada en movies-api es posible definir mas opciones como rutas alternativas al Dockerfile, argumentos adicionales para la construccion, etc.

### ¿Qué pasa si los dejas iguales?
>R: Si ambos se dejan iguales habria que estar atento de indicar de manera correcta los directorios, pero las dos maneras son equivalentes y validas.
