# Proxecto Docker

Arquitectura web con frontend, backend y base de datos. Incluye persistencia y montajes de código en tiempo real.

# Práctica PPS - Despliegue con Docker

## Descrición do proxecto

Este proxecto consiste nunha aplicación web simple despregada mediante Docker. Consta de tres compoñentes principais:
- Un **frontend** en HTML.
- Un **backend** en Python (Flask).
- Una base de datos **PostgreSQL** inicializada con un script SQL.


## Composición dos servizos

La arquitectura está definida en `docker-compose.yml` y se compone de:

- `frontend`: Servidor web estático que sirve el fichero HTML.
- `backend`: API REST construída con Flask.
- `db`: Contenedor de PostgreSQL con un script de inicialización (`init.sql`).


## Comandos principais para executar o proxecto

### 1. Construír e levantar os contedores:
```bash
docker-compose up --build

