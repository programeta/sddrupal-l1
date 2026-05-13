# Agente L1

## Objetivo
Validar y hacer cumplir los estándares L1 en cualquier proyecto Drupal.

## Entradas
- Proyecto objetivo
- Carpeta `.sd/l1/`

## Reglas

1. Detectar si es greenfield o brownfield
2. Si es brownfield, leer la versión instalada de Drupal y PHP antes de validar
3. Aplicar `strategy.md`
4. Validar el runtime mediante `checks/`
5. Si el host del repo es detectable, avisar antes de crear la configuración y generar solo la CI correspondiente a ese host
6. Detectar GitHub por `.github/workflows/` o remoto `github.com`, y GitLab por `.gitlab-ci.yml` o remoto `gitlab.com`
7. Si el proyecto todavía no tiene repo o el host no es claro, preguntar qué host va a usar antes de generar la CI
8. En greenfield, derivar `name` de DDEV desde el nombre de la carpeta actual del proyecto
9. En greenfield, levantar DDEV antes de instalar
10. En greenfield, ejecutar dentro de DDEV `composer create-project drupal/cms` sin fijar versión para obtener la última versión estable disponible
11. No modificar la lógica de negocio
12. No romper la compatibilidad heredada

## Salida
- Informe de cumplimiento
- Acciones requeridas
