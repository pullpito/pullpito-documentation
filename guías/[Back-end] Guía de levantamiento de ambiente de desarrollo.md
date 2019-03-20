# Guía de levantamiento de ambiente de desarrollo Back-end

## Requerimientos

- [Docker](https://www.docker.com/)
- [Docker compose](https://docs.docker.com/compose/)
- [Código fuente](https://github.com/pullpito/pullpito-backend)

## Stack de tecnologías

- [Ruby on Rails](https://rubyonrails.org/)
- [PostgreSQL](https://www.postgresql.org/)

## Levantamiento

1. Clonar el código fuente del [repositorio](https://github.com/pullpito/pullpito-backend).
1. En la raiz del directorio de front clonado ejecutar `docker-compose up -d`.
1. Entrar via navegador web a la url del cli: http://localhost:3000.

## Flujo de desarrollo

La infraestructura está creada con base en la [arquitectura template para api RoR](https://github.com/josuemeza/ror-api-template) creada por [Josue Meza](https://github.com/josuemeza). Las instruccuones en la documentación del template aplican como dinámica de trabajo para esta aplicación.