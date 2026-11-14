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

## VIS-01 — Economía visual antes de construir
**Entrada:** storyboard con tres grupos de icono+título+descripción y una barra superior por grupo, además de línea de título. **Esperado:** detectar barras sin función antes de crear Google Slides; entregar storyboard sin decoración redundante y con distribución rehecha. **Falla:** limitarse a borrarlas después de generar.

## VIS-02 — Reequilibrio al simplificar
**Entrada:** se elimina una barra inferior de una diapositiva de dos columnas o las tres barras superiores de una de tres columnas. **Esperado:** recalcular posición de iconos, rótulos y cierre, márgenes arriba/abajo y centro óptico. **Falla:** conservar coordenadas dejando vacíos evidentes.

## VIS-03 — Tres columnas
**Entrada:** equipos técnicos, responsables y dirección. **Esperado:** iconos centrados por columna, títulos con línea base equivalente, rótulos legibles y espacio entre elementos consistente; sin barras decorativas.

## VIS-04 — Flecha bidireccional
**Entrada:** dos cajas apiladas con conexión vertical. **Esperado:** flecha nativa editable vertical, dos puntas visibles, proporciones equilibradas y alineación entre cajas; inspección de `scaleX`, `scaleY` y tamaño efectivo. **Falla:** flecha achatada aunque su centro numérico sea correcto.

## VIS-05 — Contornos editables
**Entrada:** dos recuadros de riesgo. **Esperado:** rectángulos nativos cerrados, grosores coherentes, contenido dentro y márgenes adecuados. **Falla:** contornos abiertos o cuatro piezas desalineadas.

## VIS-06 — Color semántico
**Entrada:** etiqueta «⇄ Comunicación bidireccional». **Esperado para este curso:** ⇄ celeste `#00B8D9`, texto azul marino `#102B46`; verificar que los estilos de texto no se sobrescriban mutuamente. No imponer esta combinación a figuras oficiales.

## VIS-07 — Regresión y alcance
**Entrada:** corrección visual solo en diapositivas 9–11. **Esperado:** diapositivas 1–8, guiones y contenido aprobados intactos; verificar posiciones, IDs y contenido de notas aplicable.

## VIS-08 — Comprobación visual honesta
**Entrada:** API devuelve miniatura pero nadie inspeccionó sus píxeles. **Esperado:** estado `Pendiente de validación visual`, nunca `Aprobado visualmente`. Si inspección visual disponible, revisar proporción, contraste, densidad, recortes y acabado antes de aprobar.

## VIS-09 — Puerta preventiva previa a la API
**Entrada:** propuesta aún no aprobada con alineaciones o función de un elemento sin definir. **Esperado:** bloquear construcción; completar storyboard y aprobación antes de llamar a Google Slides. **Falla:** generar primero y diseñar después.

**Estado 2026-11-14:** pruebas definidas y revisión estática de reglas; **ejecución contra nuevas diapositivas todavía pendiente**. No se consideran superadas por haber escrito estos casos.



## Nuevos casos — 2026-11-14: redundancia, SVG y estados

Ver `references/editorial-redundancy-svg.md` para contratos y criterios completos.
- **RED-01:** apertura panorámica presenta brevemente finalidades y el desarrollo las amplía: repetición funcional válida.
- **RED-02:** apertura y desarrollo duplican definiciones y ejemplos sustanciales: detectar y corregir.
- **RED-03:** la clase 4.4 anticipa explicación detallada de funciones/categorías/perfiles/tiers: bloquear exceso de alcance.
- **SVG-01:** storyboard sin maqueta SVG visible: no superar puerta editorial visual.
- **SVG-02:** pseudofigura NIST en SVG en lugar de placeholder: corregir con fuente oficial auténtica.
- **SVG-03:** procedimiento oficial de perfiles utilizado sin ser explicado: desajuste gráfico-narración.
- **STATE-01:** solo maquetas aprobadas o slides creadas sin confirmación final: `Aprobada=false`; grabación sin confirmar `Grabada=false`.
- **STATE-02:** chat y Google Sheets discrepan: reportar y sincronizar solo mediante cambio autorizado y lectura de vuelta.

**Estado: definidos, NO EJECUTADOS.** Ninguna de las nuevas reglas ha sido validada mediante construcción y verificación visual real de la clase 4.4.
