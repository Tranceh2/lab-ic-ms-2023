# Respuestas

Indica tu nombre a continuación: 

Por cada etapa agrega una sección abajo y escribe las respuestas a las preguntas de cada etapa.

## ETAPA 1

Escribe respuestas de la etapa 1 acá

## ETAPA 2

Escribe respuestas de la etapa 2 acá

## ETAPA 3

¿Qué te llama la atención?
R: Un aspecto que podria llamar la atencion del Dockerfile seria el uso de Multi-stage Build en este, el cual en este caso permite destinar un stage para el build del desarrollo en una imagen especifica de golang, para luego utilizar el binario construido en otra imagen de tipo distroless. De esta manera se optimiza el tamaño final de la imagen.

¿Cómo se relacionan el archivo `docker-compose.yml` y el archivo `movies-api/Dockerfile`?
R: La relacion va en que el archivo docker-compose.yml en la seccion del service movies-api realiza el build de la imagen utilizando el Dockerfile presente en movies-api/Dockerfile

¿Qué crees que hace el atributo `context` debajo de `build` (está en la linea 6 del archivo `docker-compose.yml`)?
R: El atributo context lo que hace es indicar donde se encuentra el archivo Dockerfile y ademas indicar el contexto o grupo de archivos con el cual podra trabajar el Dockerfile en la construccion de la imagen.
