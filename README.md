# 🌿 PlantCare - Orquestador Docker

Este repositorio contiene los archivos necesarios para levantar de forma rápida y sencilla la API dockerizada de **PlantCare**, una API RESTful para la gestión de plantas, plagas, usuarios, cuidados y más.

---

## 🔧 Requisitos

- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)

---

## 🚀 ¿Qué incluye este orquestador?

- 🔌 Servicio de la API PlantCare desde una imagen pública en Docker Hub.
- 🛢️ Base de datos MySQL 5.7 lista con persistencia de datos.
- 🌐 Panel de administración con **phpMyAdmin**.
- ⚙️ Variables de entorno centralizadas para facilitar la configuración.

---

## ▶️ Cómo levantar el entorno

```bash
git clone https://github.com/KarenLC23/plant-care-deploy.git
cd plant-care-deploy
cp .env.example .env   # Revisa y modifica si lo necesitas
docker-compose up --build


🌍 Accesos rápidos
API: http://localhost:8100

phpMyAdmin: http://localhost:8101
(Usuario: root – Contraseña: 12345)

📦 Imagen utilizada
Este orquestador usa la imagen Docker pública ya construida con CI/CD:

🖼️ kldevops/api-plantas:latest
📦 Disponible en: DockerHub

📁 Archivos incluidos
| Archivo              | Descripción                                           |
| -------------------- | ----------------------------------------------------- |
| `docker-compose.yml` | Define los servicios: API, base de datos y phpMyAdmin |
| `.env.example`       | Variables de entorno de ejemplo                       |
| `init.sql`           | Script de base de datos inicial (opcional si existe)  |


👩‍💻 Autor
Desarrollado y orquestado por Karen Caicedo 🚀
En camino a ser DevOps Engineer con pasión por los entornos productivos y automatizados.

