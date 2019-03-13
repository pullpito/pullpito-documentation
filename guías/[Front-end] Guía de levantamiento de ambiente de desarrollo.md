# Guía de levantamiento de ambiente de desarrollo Front-end

## Requerimientos

- [Docker](https://www.docker.com/)
- [Docker compose](https://docs.docker.com/compose/)
- [Código fuente](https://github.com/pullpito/pullpito-front)

## Stack de tecnologías

- [VueJS](https://vuejs.org/)

## Levantamiento

1. Clonar el código fuente del [repositorio](https://github.com/pullpito/pullpito-front).
1. En la raiz del directorio de front clonado ejecutar `docker-compose up -d cli`.
1. Entrar via navegador web a la url del cli: http://localhost:8000.

## Flujo de desarrollo

Si el proyecto no está creado, es posible crearlo directamente desde el CLI **dentro del directorio /app**. Ej: `/app/pullpito-front`.

Toda interacción con el proyecto (dependencias, tareas, etc) se puede realizar directamente desde el CLI. También es posible realizarlo dentro de la consola del contenedor via línea de comandos. Para ingresar a la consola del contenedor se debe ejecutar `docker-compose exec cli bash`. Cabe mencionar que entrar a la consola del contenedor es una acción de alto riesgo por el potencial cambio de configuraciones además que cualquier configuración debería existir como código y no de forma manual.

Tras reiniciar los servicios, el CLI no mostrará el proyecto en el dashboard. Para que vuelva a ser visible, basta con importarlo en la sección `Importar`.