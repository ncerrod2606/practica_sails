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


## Configuración de Laravel Sail

Esto generará un nuevo proyecto de Laravel con Sail preconfigurado. Una vez creado, navegamos al directorio del proyecto:
```bash
cd practica-sails
```

Y lo iniciaremos en segundo plano con el comando:
```bash
./vendor/bin/sail up -d
```

![Iniciando Sail](../doc/img/cp3.png)

## Gestión de Servicios y Contenedores

Veremos los contenedores en ejecución con:
```bash
docker ps
```
![Contenedores en ejecución](../doc/img/cp4.png)

## Ejecución de Migraciones y Pruebas

Ejecutaremos las migraciones para configurar la base de datos:

```bash
./vendor/bin/sail artisan migrate
```

![Migraciones ejecutadas](../doc/img/cp5.png)

Probaremos la aplicación accediendo a `http://localhost` en el navegador, lo que debería mostrar la página de bienvenida de Laravel.

![Página de bienvenida](../doc/img/cp6.png)

## Comandos Útiles de Mantenimiento
Para detener los contenedores:
```bash
./vendor/bin/sail stop
```
![Contenedores detenidos](../doc/img/cp7.png)

Para iniciar los contenedores nuevamente:
```bash
./vendor/bin/sail up -d
```
![Contenedores iniciados](../doc/img/cp8.png)

Para ejecutar comandos Composer dentro del contenedor:
```bash
./vendor/bin/sail composer install
```
![Composer install](../doc/img/cp9.png)

Para hacer un test de la aplicación:
```bash
./vendor/bin/sail test
```
![Tests ejecutados](../doc/img/cp10.png)




