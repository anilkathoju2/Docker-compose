🛒 E-Commerce Platform – Docker Compose Setup
This project is an e-commerce web application powered by Docker and Docker Compose. It bundles all required services (web app, database, cache, etc.) into isolated, reproducible containers — making local development simple, fast, and consistent.

🚀 Features
* Fully containerized development environment
* Single command startup
* Hot-reloading for development
* Database + cache preconfigured
* Environment variable support via .env file

for i in mongodb mysql catalogue user cart shipping payment frontend ; do cd $i; docker build -t $i:v1 . ; cd ..; done

- docker compose up -d
- docker compose down

- Stop + remove volumes (⚠️ deletes DB data):
- docker compose down -v


docker compose
===============
it is simple yaml used to up or down the services at a time, define dependencies, networks, volumes, etc.
services are dependent on each other. 