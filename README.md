# EventFlow - Taller DevOps + Arquitectura

Este repositorio acompaña el taller de arquitectura y DevOps para el sistema *EventFlow*.

## Contenido

- `index.html`: Archivo simple (intencionalmente con malas prácticas) para análisis en SonarCloud.
- `.github/workflows/ci.yml`: Pipeline básico de CI/CD que ejecuta:
  - Checkout
  - Build simulado
  - Tests simulados
  - Copia de `index.html` a la carpeta `/build`
- `main.tf`: Archivo Terraform para el módulo de IaC (opcional según el taller).

## Objetivo del Pipeline (CI)

Este pipeline demuestra:
- Automatización básica DevOps
- Ejecución automática en cada push
- Preparación para futuras tareas como despliegue automático

## Ejecución del Pipeline

Cada vez que se haga *push* a `main`:
1. GitHub Actions realiza un build simulado.
2. Corre tests simulados.
3. Copia los artefactos a la carpeta `/build`.

## Integración con SonarCloud

1. Importar el repo en SonarCloud.
2. Activar análisis automático.
3. Observar los *code smells* en `index.html`.

## Licencia
Uso educativo.
