# Respuestas del simulacro RA3.1

## Tarea 3 · Conversión del fragmento antiguo

| Código antiguo | Solución en HTML5/CSS | Motivo |
|---|---|---|
| `<TABLE>` y celdas usadas para disponer el contenido | `<section class="condiciones-ofertas">` con párrafos y CSS | La tabla se reserva para datos tabulares; la sección expresa el contenido y se adapta mejor. |
| `<CENTER>` | `text-align: center` en la hoja de estilo | Separa presentación y contenido y elimina una etiqueta obsoleta. |
| `<FONT FACE/SIZE/COLOR>` | Reglas CSS para tipografía, tamaño y color | La presentación se gestiona desde una hoja de estilo reutilizable. |
| `<B>` para destacar las etiquetas | `<strong>` para «Validez», «Garantía» y «Pago» | `strong` comunica importancia semántica, además de su presentación. |
| `BGCOLOR`, `CELLPADDING`, `ALIGN` y `BORDER` | `background-color`, `padding`, `text-align` y `border` en CSS | Sustituye atributos de presentación obsoletos por estilos. |
| Imagen GIF enlazada sin texto alternativo | Enlace de texto «Contacta con nosotros» | El control se entiende con lector de pantalla y no depende de una imagen ausente. |
| `&iacute;` y `&ntilde;` | Caracteres españoles en UTF-8 | La codificación declarada permite escribir el texto de forma legible. |

## Tarea 5 · Ventajas de CSS

La variable `--color-principal` se cambió temporalmente de `#e86f00` a `#166534`. Las cabeceras, enlaces destacados, etiquetas de descuento y precios nuevos de ambas páginas cambiaron al actualizar esa única declaración. Después se restauró `#e86f00`.

Ventajas comprobadas:

1. Un único cambio propaga el color de marca por varias páginas y componentes.
2. La presentación queda separada del contenido HTML y puede reutilizarse.
3. Las reglas responsive y de impresión se mantienen centralizadas sin duplicarlas en cada página.

Las capturas antes/después de Inicio y Guías se adjuntan a la conversación. La captura de Ofertas a 375, 768 y 1280 px y la del modelo de caja de la etiqueta se adjuntan junto con las comprobaciones visuales.

## Tarea 6 · Lenguajes de marcas del sitio

| Fichero modificado | Lenguaje | Tipo | Versión o estándar | Organismo que lo define |
|---|---|---|---|---|
| `index.html` | HTML | Lenguaje de marcas | HTML Living Standard | WHATWG |
| `guias.html` | HTML | Lenguaje de marcas | HTML Living Standard | WHATWG |
| `galeria.html` | HTML | Lenguaje de marcas | HTML Living Standard | WHATWG |
| `contacto.html` | HTML | Lenguaje de marcas | HTML Living Standard | WHATWG |
| `ofertas.html` | HTML | Lenguaje de marcas | HTML Living Standard | WHATWG |
| `css/estilos.css` | CSS | Hoja de estilo | CSS (especificaciones CSS actuales) | W3C CSS Working Group |
| `noticias.xml` | XML | Lenguaje de marcas; canal RSS | XML 1.0; RSS 2.0 | W3C; RSS Advisory Board |
| `sitemap.xml` | XML | Lenguaje de marcas; protocolo Sitemap | XML 1.0; Sitemap Protocol 0.9 | W3C; sitemaps.org |
| `respuestas.md` | Markdown | Lenguaje de marcado ligero | CommonMark | CommonMark |

## Tarea 7 · Herramientas y comprobación

- Validación de `ofertas.html` y `css/estilos.css`: pendiente de capturar los resultados del validador W3C.
- Vista adaptable: comprobada visualmente en 375, 768 y 1280 px; no debe aparecer desplazamiento horizontal en 375 px.
- Inspector: pendiente la captura del modelo de caja de `.etiqueta`.
- Errores encontrados y corregidos: sustituí etiquetas y atributos de presentación antiguos, quité el estilo en línea del pie, asocié etiquetas a los controles del formulario y añadí texto accesible al enlace que antes dependía de una imagen.
