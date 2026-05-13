# Estándar de DDEV

## Requisitos
- Docker
- DDEV >= 1.23

## Configuración base
- PHP 8.5 en greenfield
- PHP igual a la versión detectada en brownfield
- nginx-fpm
- MariaDB 10.6

## Regla
Todos los proyectos deben arrancar con:
ddev start
