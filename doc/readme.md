# Practica Laravel con Sails

<p align="left">
<img src="https://img.shields.io/badge/STATUS-FINALIZADO-blue">
</p>

## Índice

1. [Creación del Scaffolding del Proyecto](#creación-del-scaffolding-del-proyecto)
2. [Configuración de Laravel Sail](#configuración-de-laravel-sail)
3. [Gestión de Servicios y Contenedores](#gestión-de-servicios-y-contenedores)
4. [Ejecución de Migraciones y Pruebas](#ejecución-de-migraciones-y-pruebas)
5. [Comandos Útiles de Mantenimiento](#comandos-útiles-de-mantenimiento)
6. [Si lo haces con podman en lugar de docker](#si-lo-haces-con-podman-en-lugar-de-docker)
---

## Creación del Scaffolding del Proyecto

Procederemos a crear el proyecto con el comando:
```bash
curl -s "https://laravel.build/practica-sails" | bash
```

![Creación del proyecto](../doc/img/cp1.png)

![Creación del proyecto](../doc/img/cp2.png)


Esto generará un nuevo proyecto de Laravel con Sail preconfigurado. Una vez creado, navegamos al directorio del proyecto:
```bash
cd practica-sails
```