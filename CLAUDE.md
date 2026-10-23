# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Qué es este repositorio

CV profesional de Carlos Enrique Madrigal Ramos gestionado con [RenderCV](https://rendercv.com/). No es una aplicación: la única "fuente de verdad" es un archivo YAML que RenderCV compila a PDF, HTML, Markdown, Typst y PNG.

## Comandos

```bash
# Generar todos los formatos en rendercv_output/
rendercv render cv-carlos-madrigal_CV.yaml

# Solo PDF
rendercv render cv-carlos-madrigal_CV.yaml --pdf-only
```

Requisitos: Python 3.8+ y `pip install rendercv`.

## Arquitectura

- **`cv-carlos-madrigal_CV.yaml`** — único archivo editable. Contiene tres bloques de nivel superior:
  - `cv:` — datos personales y las `sections:` (Perfil, Experiencia, Educación, Proyectos, etc.). El orden de las secciones aquí determina el orden en el documento renderizado.
  - `design:` — tema `classic`, `colors`, y `templates`. La plantilla `education_entry` está **personalizada** (`degree_column: ''` y el `degree` movido al `main_column`) para evitar que títulos largos rompan el formato de la columna de fecha; no la revierta al default sin motivo.
  - `locale:` — idioma `spanish`.
  - `rendercv_settings:` — rutas de salida (`rendercv_output\NAME_IN_SNAKE_CASE_CV.*`) y `current_date`, que fija la fecha impresa en el CV. Al actualizar el CV, ajustar `current_date`.
- **`rendercv_output/`** — artefactos generados. Está en `.gitignore`; no editar a mano ni commitear. Los `.pdf`/`.png` versionados con sufijos (`_VE`, `_3`) son variantes archivadas manualmente.
- **`README.md`** — versión en Markdown del CV mantenida a mano, redundante con el YAML. Al cambiar datos en el YAML, sincronizar el README si el cambio es visible ahí.

## Flujos de trabajo habituales

1. **Actualización de mantenimiento** — el caso más común. Agregar cursos nuevos, proyectos recientes que aún no figuran, o reflejar un cambio de cargo/empresa. Editar la sección correspondiente en el YAML, ajustar `current_date`, sincronizar `README.md` si aplica y re-renderizar.
2. **Ajuste para una oferta específica** — cuando el CV se adapta a una vacante concreta. El proceso es: analizar primero la oferta, identificar puntos de optimización para alinear el CV lo más preciso posible, destacar los puntos a favor de esa oferta, y **planear los ajustes antes de editar**. No reescribir el YAML de entrada sin este análisis previo.

## Convenciones

- Todo el contenido va en **español** con acentos correctos.
- Los iconos usan nombres simples de FontAwesome (ej. `phone`), no clases CSS.
- `custom_connections` incluye teléfonos como enlaces `wa.me`; hay entradas comentadas (números alternos) que se activan/desactivan según el país de residencia.
