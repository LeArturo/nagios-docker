# Despliegue de Nagios Core en Docker

## Requisitos

- Docker
- Docker Compose
- Git

## Pasos para Construir y Ejecutar el Contenedor

### 1. Clonar el Repositorio

Clona el repositorio de GitHub en tu máquina local:
!/bin/bash
git clone https://github.com/LeArturo/nagios-docker.git
cd nagios-docker

## Dentro de tu carpeta deberian quedar todos estos archivos

├── Dockerfile
├── docker-compose.yml
├── nagios.conf
└── README.md

## Armar imagen y ejecutar nagios-core
	cd nagios-core
		docker build -t nagios .
		docker run -d -p 80:80 <imagen-ID>

## Ejecutar y armar nagios con docker-compose
	cd nagios-core
		docker-compose up -d
