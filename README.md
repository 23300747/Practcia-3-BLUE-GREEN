# Práctica 3 — Blue/Green Deployment
# Alonso Uriel Jiménez Gutiérrez  

## Descripción
Implementación de una estrategia Blue/Green Deployment utilizando Lentasos (e-commerce de lentes) con FastAPI, MongoDB, Docker y Nginx.

## Tecnologías
- FastAPI + MongoDB Atlas
- Docker + Docker Compose
- Nginx (reverse proxy)
- Bash scripts + Cron

## Estructura
- `blue/` — Versión 1 (naranja)
- `green/` — Versión 2 (azul)
- `nginx/` — Configuración del proxy
- `promote.sh` — Promoción automática a green
- `rollback.sh` — Rollback manual a blue

## Cómo ejecutar
```bash
sudo systemctl stop nginx
docker compose up -d
service cron start
```

Acceder en `http://localhost`
