# Kit SDDrupal L1

Este repositorio define los estándares de plataforma/runtime (L1) para proyectos Drupal.

## Uso

Clónalo dentro de cualquier proyecto:

git clone <repo> .sd/l1

## CI

La L1 debe generar una única configuración de CI para el host detectado.

- GitHub: generar GitHub Actions.
- GitLab: generar GitLab CI.
- Host no claro o sin repo: preguntar antes de crear la CI.

Los agentes deben leer:

- context/
- standards/
- playbooks/
- checks/
