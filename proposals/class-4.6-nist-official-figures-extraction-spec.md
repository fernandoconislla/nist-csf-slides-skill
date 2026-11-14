# Clase 4.6 — especificación de imágenes oficiales (versión de trabajo)

**Fecha:** 2026-11-14
**Estado:** fuente y regiones visualmente verificadas; **recortes PNG auténticos aún no extraídos; no generar/añadir slides ni declarar aprobado** hasta tener bytes originales accesibles.

Fuente primaria única: https://nvlpubs.nist.gov/nistpubs/CSWP/NIST.CSWP.29.spa.pdf
Publicación NIST CSWP 29 español, 36 páginas.

## Páginas y regiones del documento (índice PDF, base cero)
- `P21` (22.ª página PDF; folio 16): tabla 1 completa. Verificada con captura del PDF; tabla en aproximadamente x=132..955, y=456..1186 del pantallazo de 1088×1408. Cabecera «Función / Categoría / Identificador de Categoría», primeros seis renglones amarillos Gobernar.
- `P22` (23.ª página PDF; folio 17): bloque «Estrategia de gestión de riesgos (GV.RM)» y subcategorías `GV.RM-01...`. El nombre de categoría empieza cerca de y=773 del pantallazo, y `GV.RM-01` en y≈866. Recorte aproximado x=125..962, y=767..925 para ejemplo puntual. Su resultado textual oficial: «Los objetivos de la gestión de riesgos son establecidos y acordados por las partes interesadas de la organización».
- `P26` (27.ª página PDF; folio 21): bloque «Seguridad de los datos (PR.DS)», entradas `PR.DS-01`, `PR.DS-02`, `PR.DS-10`, `PR.DS-11`; verificada con captura PDF. Recorte aproximado x=126..964, y=940..1290.

**Nota técnica:** coordenadas anteriores son del screenshot web a 1088×1408, NO coordenadas PDF. Usar render real de páginas 21/22/26 a 150–200 dpi y redetectar cajas. No fabricar imágenes que imiten extractos.

## Storyboard y anotación por slide
1. Portada original de la familia, sin recortes.
2. «¿Qué es una categoría?»: recorte legible de cabecera+seis renglones Gobernar de tabla 1 (P21). Señalar banda Gobernar. Introducir qué significa agrupar resultados.
3. «¿Cómo se identifica una categoría?»: recorte de las primeras 2–3 filas amarillas de tabla 1 (P21). Marco cian **exactamente** sobre fila «Estrategia de gestión de riesgos | GV.RM». Señalador externo con `GV` + `RM`, dejando documento legible.
4. «¿Qué es una subcategoría?»: recorte P22 que abarque «Estrategia de gestión de riesgos (GV.RM)» y `GV.RM-01`. Halo cian únicamente sobre resultado `GV.RM-01`.
5. «Identificadores y saltos»: recorte P26 con las 4 entradas oficiales `PR.DS-01`, `PR.DS-02`, `PR.DS-10`, `PR.DS-11`. Contorno cian en `02` y `10`, señalador externo «salto intencional» sin dibujar categorías inexistentes.
6. «Cómo leer una subcategoría completa»: recorte P22 conservando categoría, identificador y resultado de `GV.RM-01`. Anotaciones externas `GV` función, `RM` categoría, `01` subcategoría, sin tapar contenido.

**Norma de diseño:** fondo blanco, títulos azul marino #102B46, subrayado cian #00B8D9, Inter, 16:9. Recortes del PDF deben conservar tipografía, color y proporción exactos del material oficial, tamaño suficiente para leer el código. Anotaciones como objetos independientes. Narración completa de propuesta 4.6 V1; corregir si hace referencia a recortes de manera incongruente.

## Auditoría de origen y bloqueo actual
Verificación documental hecha a través de capturas reales del PDF oficial en páginas 21, 22 y 26 (índice base cero). Sin embargo, en este entorno no se ha conseguido descargar el PDF a un archivo local: error de resolución DNS en container; fuente no existe como PDF adjunto en la Biblioteca ni en Google Drive. Por ello **NO existen todavía recortes PNG auténticos** ni se ha modificado el deck Google Slides. La siguiente acción legítima es obtener el archivo fuente auténtico (por ejemplo, archivo PDF adjuntado a conversación) y extraer esos recortes; no sustituirlo por una reconstrucción ni por la tabla en inglés tomada de terceros.
