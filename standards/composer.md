# Estándar de Composer

- `composer.lock` obligatorio
- No instalar dependencias manualmente
- Greenfield: partir de Drupal CMS con `composer create-project drupal/cms` sin fijar una versión concreta para obtener la última versión estable
- Brownfield: respetar la base Composer ya existente
- `drush/drush` debe instalarse en `require`, no solo en `require-dev`
- Drush debe estar disponible en runtime y en entornos productivos
- Para proyectos Composer-managed compatibles:
  - `drupal/core-recommended`
  - `drupal/core-composer-scaffold`
