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

## OFF — Miniaturas oficiales y portada

**OFF-01:** maqueta 4.4 slide 02 usa círculos con números en lugar de tres imágenes oficiales disponibles → fallo. **OFF-02:** rueda, plantilla NIST Perfiles y figura Tiers pequeñas pero deformadas, recortadas arbitrariamente o ilegibles → fallo. **OFF-03:** portada aprobada sustituida por figura oficial → fallo. **OFF-04:** activos oficiales pequeños, nítidos, proporciones intactas, centrados con etiqueta/función y fuente documentada → conforme solo tras inspección real. **Casos definidos, NO ejecutados.**

## RETRY + FOCUS — 2026-11-14
- **RETRY-01**: conector funciona pero solicitud read falla por máscara de campos inválida → corregir campo y continuar, no declarar desconexión. **Ejecutado y superado 2026-11-14**: error `slides.pageElements.shape.text` corregido con lectura completa de presentación, revisión disponible.
- **RETRY-02**: batch Slides falla por `outline.solidFill` desconocido → cambiar a `outline.outlineFill.solidFill`, refrescar revisión, verificar sin duplicados. **Precedente ejecutado en 4.6**.
- **RETRY-03**: escritura tuvo éxito pero respuesta falla/desaparece → leer IDs/revisión antes de reintentar; falla si duplica objeto.
- **FOCUS-01**: contorno fino cian en cuadro amarillo y sin etiqueta → **fallo** de foco visual a zoom de presentación.
- **FOCUS-02**: objetivo oficial sin alterar, doble marco marino+cian, chip descriptivo sin tapar letras, verificado en PDF final → **superado para clase 4.6 slides 27–31, 2026-11-14**.
- **FOCUS-03**: chip o contorno se sobrepone a contenido esencial o apunta a otra fila → **fallo**.
- **FOCUS-04**: resumen de contacto parece válido pero ampliación individual detecta mala alineación → corregir y renderizar otra vez. **Regla**, no una prueba ejecutada en todos los casos.

## OCCLUSION — regresión de oclusión de códigos (2026-11-14)
- **OCC-01**: marco marino/cian de alto contraste intersecta cualquier carácter de `GV.RM-01` aunque se vea moderno → **NO conforme**.
- **OCC-02**: contornos de `PR.DS-02` y `PR.DS-10` intersectan la tinta del código o texto del resultado → **NO conforme**.
- **OCC-03**: barras laterales marino/cian externas a la línea + chip fuerte, texto original sin oclusión en render exportado → **Conforme en slides 29–31, 2026-11-14**.
- **RETRY-04**: requiredRevisionId obsoleto causa error de API y ninguna mutación → refrescar revisión, comprobar inexistencia de efectos parciales, repetir solicitud segura. **Ejecutado y superado 2026-11-14:** revisión desactualizada `QtyPp6rt-svPiQ`; relectura `JAyvmxVwXNw1Vw`; actualización correcta `IF8N21sT4INjEw`.

## DIAGRAM / TIERS — regresión clase 4.7 (2026-11-14)
- **GRAPH-01**: slide Perfil Actual/Objetivo protagonizada solo por párrafo NIST recortado → falla; diagrama comparativo editable → conforme.
- **GRAPH-02**: slide Perfil Comunitario como recorte teórico sin representación de línea base → falla; diagrama comunitario con casos reales verificados en NIST y distinción con Perfil Objetivo → conforme.
- **TIER-01**: panorama de 4 Tiers define individualmente todas sus características y otra slide repite las mismas → redundancia, falla.
- **TIER-02**: panorama con figura 4 íntegra; 4 slides con figura 4 íntegra y foco externo diferente, dos dimensiones normativas de cada Tier → conforme en 4.7 V3.
- **TIER-03**: marcador gráfico cubre texto NIST, interpreta la barra como nivel de certificación u obliga llegar a Nivel 4 → falla.
- **TIER-04**: panel de descripción recorta las últimas líneas a zoom final → falla; reajustar panel, volver a exportar y revisar. Se ejecutó ajuste en slides 36–39 V3.

## ACEPTACIÓN 4.7 — cierre de pendientes (2026-11-14)
- **APP-47**: usuario dice «aprobado» respecto a 4.7 → actualizar G17 TRUE, H17 permanece FALSE; verificar lectura de Sheets. **EJECUTADO** 2026-11-14.
- **GRAPH-03**: imagen recortada de un párrafo doctrinal se utiliza como único gráfico explicativo → fallo; reemplazar por diagrama editable basado en NIST sin atribuir oficialidad.
- **GRAPH-04**: perfil comunitario presentado como tercera variante interna del Perfil Organizacional → fallo; mostrar línea base compartida separada.
- **TIER-05**: slide general desarrolla rasgos de cada Tier y cuatro individuales los repiten → fallo; panorama = nombres y concepto; individuales = dos dimensiones de tabla 2.
- **TIER-06**: foco «Nivel n» y barra al pie de la imagen sin relación perceptual exacta con el escalón señalado → exige inspección visual individual antes de dar conformidad; no basta con validar existencia estructural del marcador.
- **STATE-03**: registro histórico dice G15 FALSE pero Sheet actual G15 TRUE y H15 TRUE → preservar valores actuales y registrar discrepancia, no corregir por suposición. **VERIFICACIÓN DE ESTADO EJECUTADA** en la lectura anterior a aprobación de 4.7.
- Estas reglas escritas son pruebas de regresión **definidas**; solo las marcadas EJECUTADO tienen evidencia de ejecución. No inventar ejecución automatizada.

## Regresión del estándar de producción — 2026-11-18

- **STD-01 · Acción reconocible.** PR.AA-02, -03 y -04 deben distinguir comprobación contextual y vínculo, autenticación y verificación de una afirmación. Una firma manuscrita falla al representar una firma criptográfica. Una credencial digital dibujada como carné físico requiere rediseño.
- **STD-02 · Una versión.** Revelar versiones con y sin rótulos como entregables falla. La prueba sin rótulos es interna; mostrar solo la versión elegida y justificar cualquier contenedor que permanezca.
- **STD-03 · Umbral por criterio.** Promedio 9,5 y acabado premium o claridad 9,0 activa corrección y nueva auditoría. Una puntuación sobre una maqueta solo acredita esa fase.
- **STD-04 · Marco y paleta.** Tarjeta izquierda 395 × 281 en (74, 173), gráfico 320 × 240 en (542, 193), tolerancia ±1 px. ID en azul `#4CAED8` y tonos suaves, GV en oro y PR en violeta. La 126 debe caber con margen.
- **STD-05 · Apertura de función.** Usar 87–89 como referencia. La 118 destaca Proteger en la rueda auténtica; la 119 muestra los cinco códigos, encabezados, orientación y fuente.
- **STD-06 · Despliegue.** Un SVG maestro editable y un PNG transparente por gráfico. La presentación mantiene el texto nativo. Verificar el marco y el dibujo visible.
- **STD-07 · Lectura acotada.** Para la 7.3 basta el extracto PR.AT, los puntos vigentes y la clase activa. Abrir el PDF para un activo oficial nuevo o detalle visual. Una lectura del deck completo para mover un gráfico falla.
- **STD-08 · Aprobación.** Aprobado ejecuta el siguiente paso anunciado. Cierre de clase verifica Sheets y GitHub; la casilla Grabada requiere su propia confirmación.
