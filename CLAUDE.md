# Mate-Fin-Template

Plantilla de sitio web de curso hecha con Quarto, R y GitHub Pages.

## Principio rector: replicabilidad sencilla

Este repositorio es una **plantilla**. Cualquier persona debe poder hacer
"Use this template", poner su propio contenido y que el sitio funcione, sin
saber programar y sin pasos ocultos.

Toda modificación debe respetar estas reglas:

- **Cero configuración extra.** Nada de instalar herramientas locales, crear
  secretos, tokens o servicios externos. Basta con GitHub (Actions + Pages).
- **Lo que se personaliza, en pocos lugares y a la vista.** El título y el tema
  viven en `_quarto.yml`; la bienvenida en `index.qmd`; las lecciones en
  `lecciones/`. No agregar nuevos lugares que haya que editar sin una buena razón.
- **Agregar contenido = copiar un archivo.** Una lección nueva se hace copiando
  `lecciones/_plantilla.qmd`. Los listados (`lecciones.qmd`, la barra lateral)
  deben seguir detectando archivos automáticamente, sin registrarlos a mano.
- **Nada amarrado a una persona.** Sin nombres, URLs, rutas ni datos propios del
  autor en el código; usar textos genéricos que el usuario reemplace.
- **Dependencias mínimas.** Si una lección necesita un paquete de R nuevo, se
  agrega en `.github/workflows/publish.yml` y se documenta en el README.
- **El README es la guía.** Cualquier cambio que afecte cómo se usa la plantilla
  se refleja en `README.md`, en español y paso a paso para no programadores.

Antes de dar por terminado un cambio, pregúntate: *¿alguien que acaba de copiar
el repositorio podría usarlo sin preguntarme nada?* Si la respuesta es no,
simplifica.
