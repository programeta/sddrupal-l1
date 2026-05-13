# Kit SDDrupal L1

Este repositorio define los estándares de plataforma/runtime (L1) para proyectos Drupal.

Este `L1` forma parte de una ingeniería más amplia que también contempla `L2` y `L3`, todavía definidos como `TBD`. El objetivo es dar contexto de que este kit no es un bloque aislado, sino una pieza de una arquitectura por capas.

Este L1 sirve para arrancar y validar la base técnica de un proyecto Drupal. En un `greenfield` prepara la instalación nueva, el runtime, DDEV, Composer, CI y Drush. En un `brownfield` detecta la versión real de Drupal y PHP ya existente y se alinea a esa base sin romper compatibilidad.

## Capas

- `L1`: infraestructura, runtime y CI.
- `L2`: ingeniería de la app.
- `L3`: dominio, contenido y APIs.

## Primer Uso Con Codex

Si es la primera vez que lo vas a aplicar con Codex, usa una instrucción como esta:

```text
Aplica la L1 a este repositorio.
```

Esa instrucción hace que Codex:

- detecte si es `greenfield` o `brownfield`,
- valide Drupal y PHP,
- alinee DDEV, Composer, Drush y CI,
- y genere la configuración adecuada según el host detectado.

En `greenfield`, la instalación debe usar la última versión estable de Drupal CMS y el `name` de DDEV debe derivarse del nombre de la carpeta actual del proyecto.

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
