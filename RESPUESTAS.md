# Respuestas

Indica tu nombre a continuación: David Carvallo

Por cada etapa agrega una sección abajo y escribe las respuestas a las preguntas de cada etapa.

## ETAPA 2

¿Qué pasa si cambias el nombre del servicio de `postgres` a `db`? ¿Qué otros cambios tendrías que hacer?
R: Al cambiar el nombre del servicio de postgres a db docker creara una nueva imagen de postgres con el nombre db por lo que sera necesario cambiar tambien las variables POSTGRES_USER además de la seccion depends_on en el docker-compose.yml
