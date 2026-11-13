# Pruebas de regresión de producción de clases

## Caso aprobado NIST41-01 — Portada
Entrada: título «Introducción al NIST CSF 2.0», plantilla del curso.
Esperado: se preservan gráfica y layout de portada; primera línea blanca «Introducción al» y segunda línea celeste completa «NIST CSF 2.0», sin aislar «2.0». Inspección visual real.

## NIST41-02 — Paleta
Extraer colores desde el deck maestro y compararlos por HEX con elementos nuevos. Esperado: #102B46, #00B8D9, #FFFFFF. No colores inventados de marca; excepciones legítimas en gráficos oficiales.

## NIST41-03 — Diagramas y figuras
La diapositiva que define un marco específico debe mostrar una representación institucional verificable o omitirla justificadamente. No sustituirla por un escudo IA genérico. No anticipar explicación detallada de las seis funciones cuando aún no se desarrollan.

## NIST41-04 — Composición
Verificar título superior a la izquierda, barra de acento, composición equilibrada dentro de los márgenes, ningún texto cortado, iconos de tamaño y estilo consistente. Revisión visual de todas las slides (no solo portada).

## NIST41-05 — Secuencia histórica
Diapositiva de evolución: 2014, 2018, 2024 en línea de tiempo nativa editable, cronología y etiquetas coherentes con las notas.

## NIST41-06 — Propósitos
Cuatro bloques: comprender, evaluar, priorizar, comunicar. Iconos pertinentes; no flechas ni números que los presenten como pasos obligatorios.

## NIST41-07 — Reemplazo de notas
Crear notas viejas intencionalmente; regenerar. Esperado: usar deleteText ALL + insertText para **cada** nota afectada y lectura de vuelta literal, sin residuos. Portada sólo una apertura breve.

## NIST41-08 — Conservación de aprobaciones
El usuario edita manualmente el color de un título y aprueba. Una revisión no debe modificar esa edición ni revocar la aprobación sin motivo material verificado y autorización de cambio.

## NIST41-09 — Formato
Usuario pide Google Slides. Esperado: archivo nativo editable con enlace verificado; no presentar ni entregar PDF o PPTX salvo petición expresa.

## NIST41-10 — Auditoría integral
Registrar cobertura curricular, correspondencia pantalla↔narración, notas, exactitud, redundancia independiente 1–10, identidad, legibilidad, imágenes y limitaciones, con evidencia; no otorgar 10/10 sobre aspectos no comprobados.

Estado al 2026-11-13: **casos registrados**. Las pruebas sobre una regeneración futura aún no se han ejecutado; no presentarlas como aprobadas automáticamente.
