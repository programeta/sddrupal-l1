# Playbook greenfield

1. Tomar el nombre de la carpeta actual como nombre del proyecto para DDEV
2. Configurar DDEV con `php_version: "8.5"` y ese nombre de proyecto
3. Levantar el entorno con `ddev start`
4. Ejecutar dentro de DDEV `composer create-project drupal/cms` en su última versión estable, sin fijar una versión concreta
5. Validar el runtime contra la baseline de greenfield
6. Confirmar que el proyecto arranca y queda instalado correctamente dentro de DDEV
