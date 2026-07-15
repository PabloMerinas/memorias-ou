# Rellenar Documento DOCX

Herramienta web (HTML + JS, sin backend) que permite subir plantillas `.docx` con etiquetas, detectarlas automáticamente y generar el documento final con los valores introducidos.

## Cómo funciona

1. Se seleccionan uno o varios archivos `.docx`.
2. `script.js` analiza cada documento con `PizZip` + `docxtemplater` y detecta las etiquetas presentes en el texto (incluyendo encabezados y pies de página).
3. Se generan campos de formulario dinámicos para rellenar cada etiqueta detectada.
4. Al procesar, se genera el `.docx` final con `FileSaver.js`.

## Dependencias (vía CDN)

- [docxtemplater](https://docxtemplater.com/)
- [PizZip](https://github.com/open-xml-templating/pizzip)
- [JSZip](https://stuk.github.io/jszip/)
- [FileSaver.js](https://github.com/eligrey/FileSaver.js)

## Cómo ejecutarlo

Al no tener backend, basta con abrir `index.html` en el navegador.
