# Playbook greenfield

1. Verificar que existe acceso local a DDEV; si no existe, detener el flujo y avisar que no se puede avanzar
2. Tomar el nombre de la carpeta actual como nombre del proyecto para DDEV
3. Configurar DDEV con `php_version: "8.5"`, ese nombre de proyecto y `type: drupal` para seguir la última versión estable
4. Levantar el entorno con `ddev start`
5. Ejecutar dentro de DDEV `composer create-project drupal/cms` en una carpeta temporal de trabajo, sin fijar una versión concreta
6. Aplicar dentro de DDEV los `composer require` definidos por L1 para normalizar la base del proyecto:
   - `composer require drush/drush`
   - `composer require drupal/core-recommended drupal/core-composer-scaffold drupal/core-project-message`
7. Mover el resultado a la raíz del proyecto, dejando la instalación final sin carpetas extra innecesarias
8. Validar el runtime contra la baseline de greenfield
9. Confirmar que el proyecto arranca y queda instalado correctamente dentro de DDEV
