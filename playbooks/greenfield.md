# Playbook greenfield

1. Crear el proyecto con Composer usando Drupal CMS en su última versión estable, sin fijar una versión concreta
2. Requerir PHP 8.5 como baseline del nuevo proyecto
3. Configurar DDEV con `php_version: "8.5"`
4. Validar el runtime contra la baseline de greenfield
5. Confirmar que el proyecto arranca con `ddev start`
