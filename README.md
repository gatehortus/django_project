# Registro de Usuarios - Django + Docker

Este proyecto es una aplicación básica en Django para registrar usuarios, utilizando Docker y PostgreSQL.

---

## Tecnologías usadas

- Python 3.11
- Django
- PostgreSQL
- Docker
- Docker Compose

---

## Requisitos

Antes de ejecutar el proyecto debes tener instalado:

- Docker Desktop
- Docker Compose
- Git

---

## Cómo ejecutar el proyecto

### 1. Clonar el repositorio

```bash
git clone https://github.com/gatehortus/django_project.git
cd django_project

## archivo .env 

```bash
POSTGRES_DB=usuarios_db
POSTGRES_USER=postgres
POSTGRES_PASSWORD=postgres
POSTGRES_HOST=db
POSTGRES_PORT=5432

### contruir y levantar contenedores

```bash
POSTGRES_DB=usuarios_db
POSTGRES_USER=postgres
POSTGRES_PASSWORD=postgres
POSTGRES_HOST=db
POSTGRES_PORT=5432

### ejecutar migraciones 

docker-compose exec web python manage.py migrate

### acceder a la aplicación

```bash
http://localhost:8000

## acceso a la base de datos
```bash
docker-compose exec db psql -U postgres -d usuarios_db





