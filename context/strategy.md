# Estrategia L1

## Greenfield
- Drupal CMS
- PHP 8.5 como baseline de instalación nueva
- Usar la capa de recetas/distribución de Drupal CMS en su última versión estable
- DDEV es obligatorio en local; si no hay acceso, no se puede avanzar
- Levantar DDEV con el nombre derivado de la carpeta actual del proyecto
- En DDEV, usar `type: drupal` para seguir la última versión estable de Drupal
- Instalar Drupal CMS dentro de DDEV en una carpeta temporal, aplicar los `composer require` definidos por el playbook y llevar el resultado a la raíz del proyecto

## Brownfield
- Mantener la versión existente de Drupal
- Mantener la versión existente de PHP
- No introducir Drupal CMS

## Regla
No romper nunca la compatibilidad en proyectos existentes.
