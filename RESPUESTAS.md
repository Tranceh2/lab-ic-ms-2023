# Respuestas

Indica tu nombre a continuación: 

Por cada etapa agrega una sección abajo y escribe las respuestas a las preguntas de cada etapa.

## ETAPA 1

Escribe respuestas de la etapa 1 acá

## ETAPA 2

Escribe respuestas de la etapa 2 acá

## ETAPA 3

Escribe respuestas de la etapa 2 acá

## ETAPA 4

Compara el atributo `build` del servicio `movies-api` con el de `movies-front`. 
¿Cuál es la diferencia?
R: La diferencia radica en que en movies-api el contexto (En este caso la carpeta en la cual se encuentra el Dockerfile y archivos especificos para cosntruir cada servicio) se define como una clave "context" dentro de build mientras que en movies-front se define de manera directa como un string dentro de "build". Con la manera utilizada en movies-api es posible definir mas opciones como rutas alternativas al Dockerfile, argumentos adicionales para la construccion, etc.

¿Qué pasa si los dejas iguales?
R: Si ambos se dejan iguales habria que estar atento de indicar de manera correcta los directorios, pero las dos maneras son equivalentes y validas.
