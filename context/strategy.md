# Estrategia L1

## Greenfield
- Drupal CMS
- PHP 8.5 como baseline de instalación nueva
- Usar la capa de recetas/distribución de Drupal CMS en su última versión estable
- Levantar DDEV con el nombre derivado de la carpeta actual del proyecto
- Instalar Drupal CMS dentro de DDEV con `composer create-project drupal/cms`

## Brownfield
- Mantener la versión existente de Drupal
- Mantener la versión existente de PHP
- No introducir Drupal CMS

## Regla
No romper nunca la compatibilidad en proyectos existentes.
