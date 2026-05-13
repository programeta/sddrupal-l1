# Kit SDDrupal L1

Este repositorio define los estándares de plataforma/runtime (L1) para proyectos Drupal.

Este `L1` forma parte de una ingeniería más amplia que también contempla `L2` y `L3`, todavía definidos como `TBD`. El objetivo es dar contexto de que este kit no es un bloque aislado, sino una pieza de una arquitectura por capas.

## Capas

- `L1`: infraestructura, runtime y CI.
- `L2`: ingeniería de la app.
- `L3`: dominio, contenido y APIs.

## Uso

Clónalo dentro de cualquier proyecto:

```bash
git clone https://github.com/programeta/sddrupal-l1.git .sd/l1
```

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
