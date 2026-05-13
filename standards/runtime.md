# Estándar de runtime

## Greenfield
- Drupal CMS
- PHP 8.5
- Nginx preferido
- MariaDB 10.6+ o MySQL 8+

## Brownfield
- La baseline de validación es la versión actual detectada de Drupal
- La baseline de validación es la versión actual detectada de PHP
- No subir requisitos de plataforma por encima de lo que ya existe

## PHP
- Versión: >= 8.5 en greenfield
- Versión: la existente en brownfield

## Servidor web
- Preferencia por Nginx

## Database
- MariaDB 10.6+ o MySQL 8+

## Cache
- OPcache obligatorio
- Redis recomendado

## Operación
- Drush disponible en producción
- Los entornos productivos deben poder ejecutar comandos `drush`
