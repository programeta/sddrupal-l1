# Requisitos de CI

El pipeline debe incluir:

- composer install
- PHPCS
- PHPCBF
- lint de PHP
- tests (si están disponibles)

## Regla de despliegue

Si el host del repo es detectable, el agente debe avisar antes de hacerlo y generar solo la configuración correspondiente a GitHub Actions o GitLab CI. Detecta GitHub por `.github/workflows/` o por un remoto `github.com`, y GitLab por `.gitlab-ci.yml` o por un remoto `gitlab.com`. Si el proyecto todavía no tiene repo o el host no es claro, debe preguntar qué host se va a usar antes de generar la CI.
