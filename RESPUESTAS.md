# Respuestas

Indica tu nombre a continuación: David Carvallo

Por cada etapa agrega una sección abajo y escribe las respuestas a las preguntas de cada etapa.

## ETAPA 1

¿Cuál es la diferencia entre los archivos con el verbo `Create` con los archivos con el verbo `Add`?
R: Create crea tablas o estructuras en la base de datos y Add añade entradas a la base de datos

¿Cómo se llama el servicio que se declara en el archivo `docker-compose.yml`?
R: Flyway

## ETAPA 2

¿Qué pasa si cambias el nombre del servicio de `postgres` a `db`? ¿Qué otros cambios tendrías que hacer?
R: Al cambiar el nombre del servicio de postgres a db docker creara una nueva imagen de postgres con el nombre db por lo que sera necesario cambiar tambien las variables POSTGRES_USER además de la seccion depends_on en el docker-compose.yml
