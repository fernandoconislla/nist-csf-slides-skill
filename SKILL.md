---
name: nist-csf-slides
description: Diseñar y auditar diapositivas del curso NIST CSF 2.0 siguiendo una plantilla nativa de Google Slides, la identidad visual acordada y prompts de ilustraciones consistentes.
---

# NIST CSF 2.0 — Skill de diapositivas

## Regla de imágenes oficiales en panoramas de componentes (2026-11-14)

Cuando una slide panorámica presenta **componentes identificables de un marco oficial** y existen representaciones oficiales pertinentes, debe incluir una imagen institucional auténtica de **cada componente**, incluso en formato pequeño. No sustituir recursos reales por numeraciones circulares, iconos genéricos o dibujos IA por comodidad de maquetación. Aplicar las mismas exigencias de origen, proporción, etiquetas, color, espacio útil y legibilidad que a las figuras grandes. La apertura puede sumar nombre y propósito breve de cada componente. En NIST 4.4, la slide 02 exige tres imágenes oficiales pequeñas (Núcleo, Perfiles, Tiers); ver `proposals/class-4.4-componentes-del-marco-v4.md`. Esta regla no desplaza la imagen propia de la portada ni fuerza tres recursos cuando no existe imagen oficial auténtica adecuada.

## Regla transversal 2026-11-14

Leer `references/editorial-redundancy-svg.md` junto con `references/visual-composition.md`. Una apertura panorámica puede resumir finalidad de conceptos desarrollados después: es repetición pedagógica funcional, no defecto automático. Auditar solapamientos con evidencia y alcance interclases. Tras narración auditada, texto en pantalla y storyboard, mostrar **maquetas SVG 16:9 visibles** antes de aprobación editorial y construcción de Slides. Las maquetas no equivalen a figuras oficiales ni a aprobación visual final; contrastar en vivo `PROJECT_STATE.md`, Sheets y Slides.


## Regla obligatoria: diseño preventivo antes de construir (2026-11-14)

Leer `references/visual-composition.md` antes de diseñar cada clase. Aplicar tres puertas, en este orden: **A) planificación preventiva** con función de cada elemento, jerarquía, layout y geometría; **B) construcción controlada** con comprobación de transformaciones y reequilibrio tras cambios; **C) auditoría estructural y visual real + regresión**. La inspección posterior no sustituye el diseño preventivo. No crear ni modificar Google Slides antes de la aprobación editorial explícita de la clase; una corrección autorizada se limita a su alcance.

## Ciclo obligatorio de optimización y auditoría (regla transversal)

- No limitarse a detectar defectos: ejecutar **inspección → optimización efectiva → auditoría → corrección → auditoría de regresión**, iterando mientras existan problemas materiales solucionables.
- Evaluar **redundancia intra-clase e inter-clases**, progresión, cobertura, precisión normativa, proporcionalidad de contenidos y límites entre módulos. Comparar los puntos detallados del temario, no solo los títulos.
- Para cada cambio, documentar **antes → después, motivo, fuente, efecto sobre identificadores/cobertura, gravedad y estado**. Preservar decisiones aprobadas y cambios manuales; no eliminar contenido normativo ni alterar el archivo maestro sin autorización.
- Las repetición pedagógica solo se admite cuando cambia la función: introducción, explicación, práctica o evaluación con un aprendizaje distinto. No presentar teoría repetida como aplicación.
- Verificar de nuevo tras cada iteración que no existan omisiones, contradicciones ni nuevos solapamientos; la **auditoría de regresión es obligatoria**, no opcional.
- La salida debe distinguir **corregido y verificado**, **pendiente de validar** y **no aprobado**. Bloquear aprobación ante errores técnicos graves o pérdida de cobertura; evitar puntuaciones complacientes.
- Responsabilidades: `course-curriculum-builder` controla redundancias y cobertura del curso completo; `course-lesson-builder` controla narración y pantalla por clase; `course-slide-builder` controla organización visual y propósito pedagógico de cada diapositiva; `course-class-producer` coordina las puertas de calidad y no aprueba entregas incompletas.

## Portada frente a explicación: regla de diseño instruccional

- Una **diapositiva de portada** presenta la clase y admite solo una apertura narrada breve: tema, relevancia y ruta. **No desarrollar definiciones, fechas, marcos conceptuales ni explicaciones técnicas extensas sobre la portada**.
- Si la clase exige definir su tema, crear a continuación una diapositiva específica (por ejemplo: «¿Qué es NIST CSF 2.0?») con narración completa y texto visible derivado.
- La cantidad de diapositivas responde a las **funciones pedagógicas diferenciadas**, no a una cifra predeterminada ni a un punto por diapositiva. Se permite eliminar cierres redundantes y narrar la conclusión sobre la última diapositiva cuando resulte claro.
- Portada ≠ definición ≠ evolución ≠ propósito ≠ aplicación: cada unidad debe aportar información nueva y evitar repetición encubierta.
- Orden de producción: **puntos vigentes → narración completa → auditoría y corrección → texto en pantalla → storyboard → auditoría de redundancia → presentación editable y verificación visual**. No crear diapositivas antes de comprobar cobertura narrativa.

## Criterios de aceptación derivados de la clase 4.1 aprobada (2026-11-13)

Esta clase es un **caso de regresión aprobado**, no una plantilla universal de contenido. Distinguir reglas reutilizables de decisiones visuales locales:
- **No sobrescribir aprobaciones:** conservar la versión vigente del Google Slides y las ediciones manuales aprobadas. Una nueva auditoría no revoca automáticamente la aprobación; registrar hallazgos y solicitar cambio solo ante defecto material comprobado o petición explícita.
- **Identidad real, no inferida:** inspeccionar y heredar los valores exactos del deck maestro. En el curso NIST CSF 2.0, principal `#102B46`, secundario `#00B8D9`, blanco `#FFFFFF`, fuente Inter; no introducir tonos intermedios o grises como nuevos colores de marca. Los recursos oficiales conservan su cromática.
- **Portada de clase:** mantener íntegra la composición aprobada y su recurso protagonista. En este curso, texto derecho en **dos líneas semánticas**, primera línea «Introducción al» en blanco y segunda «NIST CSF 2.0» completa en celeste; no separar «2.0» ni recolorear solo parte de la segunda línea. Para otras clases, ajustar la división por unidades conceptuales sin imponer estos textos literales.
- **Composición:** controlar posiciones dentro del área útil real; títulos sobre blanco arriba alineados a la izquierda y barra celeste de la plantilla; contenido visual equilibrado y centrado dentro de su zona, sin exigir alinear el propio título al centro. Verificar bordes, distribución, saltos de línea, no solapamientos, relación texto/imagen y legibilidad a escala.
- **Recursos específicos:** en desarrollo, para un marco, entidad, producto o norma reconocible, priorizar representación institucional/documental oficial y verificable frente a símbolos genéricos generados. Excepción: la portada usa la identidad gráfica del curso. No adelantar el contenido técnico de una figura oficial sin explicarlo: cuando sea prematuro, emplear un recurso oficial de carácter introductorio o posponer la figura.
- **Diagrama de evolución:** línea de tiempo horizontal nativa editable cuando se explica una secuencia histórica, con hitos y textos vinculados a la narración. **Propósitos no secuenciales:** cuatro bloques equivalentes con iconos, sin numeración o flechas que sugieran pasos obligatorios.
- **Narración sincronizada:** tras cada regeneración, sustituir por completo los segmentos de notas de presentador (`deleteText ALL` seguido de `insertText`), releer los cuatro segmentos o tantos como existan, y comparar literalmente contra el guion vigente. Detectar concatenaciones de versiones pasadas y repeticiones entre notas. Nunca dar por concluida la clase con notas desactualizadas.
- **QA y formatos:** inspeccionar todas las slides con el medio disponible, incluida lectura nativa y vista renderizada; distinguir verificación estructural de evaluación visual efectiva. El entregable del curso es **Google Slides editable**. No generar ni ofrecer archivos PDF, PPTX ni derivados salvo que el usuario lo solicite expresamente; si una herramienta necesita un formato temporal para QA interno, no convertirlo en entregable ni presentarlo al usuario.
- **Criterios de auditoría obligatorios:** cobertura de puntos, precisión NIST, progresión, pantalla↔narración, ausencia de redundancia (puntuación independiente 1–10), fidelidad de imágenes oficiales, paleta/plantilla, centrado y distribución, legibilidad y ausencia de texto cortado, integridad literal de notas, preservación de ediciones y estatus de aprobación. Documentar evidencia y severidad; no puntuar como comprobado lo que no se ha visto.

## Flujo obligatorio de propuesta, aprobación y presentación acumulativa (2026-11-13)

**Regla de precedencia:** esta secuencia prevalece sobre cualquier instrucción anterior que autorice generar Google Slides directamente al recibir «genera la clase». La aprobación de una clase anterior NO autoriza producir automáticamente la siguiente.

**Fase A — propuesta editorial, sin escribir diapositivas:** identificar la clase y sus puntos vigentes en Google Sheets; preparar narración COMPLETA por diapositiva, texto EN PANTALLA y especificación gráfica/layout de cada diapositiva; explicar la cobertura y los límites respecto a clases vecinas; optimizar y auditar la propuesta; **presentarla al usuario para revisión**. Sin aprobación explícita, no crear, copiar, añadir, eliminar ni modificar diapositivas en Google Slides. Si hay ajustes, regenerar la propuesta hasta su aprobación. El texto «genera ahora [clase]» solicita inicialmente esta propuesta, no la construcción del archivo, salvo que la autorización de ejecución esté ya expresamente concedida para esa propuesta.

**Fase B — construcción tras aprobación:** una vez que el usuario **apruebe la propuesta concreta**, construir las nuevas diapositivas de esa clase **dentro de la presentación acumulativa del curso ya existente**, AL FINAL y en el orden aprobado, sin abrir una presentación por clase ni sustituir la anterior. Usar la plantilla/identidad como referencia de estilos, y la presentación acumulativa como destino de edición. Conservar intactas todas las clases aprobadas anteriores y el archivo maestro de plantilla. No confundir «plantilla maestra» (fuente inmutable) con «presentación acumulativa» (destino editable).

**Fase C — control y aprobación visual:** sincronizar y releer notas del presentador íntegramente, verificar todas las diapositivas recién incorporadas en su contexto dentro del deck acumulativo, ejecutar auditoría de regresión y mostrar al usuario el enlace a la presentación actualizada. Las correcciones de producción sobre una propuesta aprobada se auditan y presentan para aceptación visual, sin alterar otras clases.

**Archivo acumulativo actual de NIST CSF 2.0:** `https://docs.google.com/presentation/d/1h8BqC56ud8_4xKm_Aco9V-XcMdfVlaLwNedodUMgOvE/edit` contiene la clase 4.1 aprobada y es el destino para añadir 4.2 y las posteriores al aprobarlas. **No utilizar** la copia separada no aprobada de 4.2 (`1WKV9iJHHn1E47Ubn9c6-GRBa-Zbx1gcHIVIrCo_ydJQ`) como nueva fuente de verdad ni agregarla sin revisión y autorización.

## Regla transversal obligatoria: honestidad, evaluación crítica y alertas graves

- Priorizar **verdad, rigor técnico, trazabilidad y calidad** por encima de agradar, asentir o confirmar las propuestas del usuario. Nunca ser complaciente por defecto ni inventar elogios.
- **Cuestionar explícitamente** premisas incorrectas, decisiones débiles, contradicciones, duplicaciones, omisiones, riesgos, problemas pedagógicos, técnicos, visuales o de alcance, aunque la propuesta provenga del usuario o de otra skill.
- Distinguir de forma inequívoca **hechos comprobados, contenido respaldado por fuentes, hipótesis, interpretaciones y opinión editorial**. No atribuir a una norma o autor un paso, requisito o procedimiento que esa fuente no establece. Si falta una fuente o verificación, decirlo sin disfrazarlo de certeza.
- **Advertencia de gravedad obligatoria:** si se detecta un problema crítico o grave —por ejemplo, contradicción normativa, pérdida de cobertura curricular, error técnico material, daño a archivos existentes, incoherencia metodológica, imposibilidad operativa o riesgo de seguridad—, señalarlo de forma visible y directa, explicar su impacto y proponer una medida correctiva. **No ocultar ni diluir el problema en una puntuación media alta o elogios superficiales.**
- Establecer un **bloqueo de aprobación** ante problemas graves no resueltos: indicar **«NO APROBADO: problema grave pendiente»** y no etiquetar la entrega como validada, lista para publicar o técnicamente correcta. La skill puede ofrecer un borrador o una alternativa con advertencias explícitas.
- **Auditar con evidencia y criterios concretos:** indicar qué se revisó, qué no se pudo verificar, el criterio incumplido, la severidad justificada y la corrección propuesta. No fabricar defectos ni exagerar severidades solo para aparentar dureza. Las puntuaciones, si existen, deben justificarse.
- Cuando dos objetivos compitan (por ejemplo, fidelidad a fuente frente a marketing, o precisión frente a simplicidad), **declarar la tensión y la prioridad recomendada**. Una instrucción del usuario no convierte una afirmación falsa en verdadera.
- Mantener **respeto profesional y claridad directa**: críticas al trabajo y a las decisiones, nunca ataques personales. No modificar entregables aprobados silenciosamente ni sobrescribir cambios manuales sin verificar primero la versión vigente.
- Aplicar esta regla a **cada etapa y subskill**, incluida la investigación, el temario, la narración, la ilustración, el diseño, la construcción de diapositivas, la auditoría final y la mejora de skills.

## Objetivo
Crear, revisar y mejorar diapositivas pedagógicas del curso NIST CSF 2.0 manteniendo precisión técnica, claridad y consistencia visual.

## Fuente de diseño
Plantilla nativa (referencia, no modificar):
https://docs.google.com/presentation/d/1LuxRkFk9y4Bb4dDNLOP0gZWYXc90A8TFcxFi4ER-F6A/edit

- Formato 16:9.
- Familia de estilos: azul marino, celeste/cian, blanco; Inter como tipografía de referencia.
- Antes de generar nuevas diapositivas, inspeccionar los masters, layouts y ejemplos de la plantilla. Trabajar sobre una copia.

## Reglas obligatorias
1. Explicar una idea central por diapositiva, evitando sobrecarga y vacíos desproporcionados.
2. Mantener texto editable en Google Slides; no rasterizar las diapositivas completas.
3. Los elementos externos como logotipo NIST y diagramas oficiales deben conservar proporción, legibilidad y colores originales.
4. Reservar zonas apropiadas para recursos externos, preferentemente cuadradas (1:1) cuando así convenga al diseño; no deformar recursos.
5. No presentar colores de elaboración propia como convenciones oficiales NIST.
6. Separar la narración de lo visible en pantalla y evitar adelantar temas de clases posteriores.
7. Auditar cada diapositiva: exactitud NIST, ajuste al temario, jerarquía, densidad, legibilidad y coherencia de estilo.
8. Ciclo de trabajo: generar → optimizar → auditar → regenerar.

## Prompt de ilustraciones
Consultar `prompts/ilustracion-base.md` antes de generar cualquier imagen de apoyo. Es una reconstrucción inicial, NO una cita literal comprobada del prompt histórico; revisar y ajustar con el original cuando esté disponible.

## Contexto del temario
Consultar `references/seccion-03.md`. Evitar anticipar el contenido de las clases posteriores.

## Evolución
Registrar cambios técnicos o visuales en `CHANGELOG.md`. Los prompts consolidados se versionan; no sobrescribir las versiones aprobadas sin conservar historia de Git.
## Protocolo obligatorio de resiliencia y foco documental (2026-11-14)
- Ante un fallo de conector, operación Google Slides/Sheets, exportación, imagen o GitHub: **no afirmar que la conexión se perdió sin una lectura de verificación**. Reintentar con diagnóstico: (1) relectura + corrección de argumentos/esquemas; (2) acción más pequeña / API alternativa / fuente local auténtica; (3) última ruta independiente y comprobación de estado, **hasta 3 intentos técnicos distintos cuando sean seguros**. No repetir a ciegas escrituras no idempotentes; comprobar IDs, revisión y cambios parciales antes de reintentar. Si la limitación es firme (permisos, autenticación revocada, inexistencia de herramienta, riesgo de duplicación) detener escrituras y reportar causa/evidencia.
- Resolver en el mismo turno todo lo que sea factible; nunca convertir una ejecución solicitada en nueva propuesta sin necesidad real. Declarar éxito solo tras lectura de vuelta. Si persiste bloqueo, documentar qué sí cambió, qué no y siguiente dependencia.
- Al enseñar tablas/recortes auténticos de NIST, el punto señalado debe ser evidente **a tamaño de presentación**: preferir **doble contorno marino+cian** y **etiqueta cian explícita** sobre contorno fino. Mantener el texto oficial intacto, foco/editable independiente y suficiente contraste en fondos amarillos o saturados. La geometría se determina por píxel real/render; verificar que las etiquetas no tapen contenido. El usuario define intensidad final.
- QA obligatorio: render de cada slide corregida → inspección visual → reajuste → segundo render; auditar por separado **Fuerza del foco visual** y **Ausencia de redundancia**. No marcar `Aprobada` sin aceptación explícita.

## Reglas consolidadas tras aprobación 4.7 — 2026-11-14
1. **Jerarquía de evidencia:** imagen oficial auténtica cuando su geometría explique el concepto; un párrafo recortado NO es por sí solo apoyo gráfico. Para relaciones (Actual→Objetivo, comunidad→ejemplos) usar diagrama nativo editable, basado en NIST y rotulado como elaboración editorial.
2. **Panorama y desarrollo son distintos:** introducción enumera y define; slides posteriores desarrollan particularidades. Repetición de nombres funcional permitida; rasgos duplicados, no. Puntuar por separado Ausencia de redundancia.
3. **Series:** si cada subelemento tiene contenido propio, una slide por elemento. Tiers 4.7: panorama de los cuatro con figura original; cuatro slides individuales con figura oficial íntegra + foco externo sobre el escalón correspondiente + dos dimensiones Gobernanza y Gestión de riesgos; integración final. No presentar Nivel 4 como obligatorio ni los Tiers como certificación.
4. **Foco sin oclusión:** destacar exactamente el componente sin ocultar glifos ni etiquetas; usar barras externas si no cabe un contorno. Confirmar en render individual, no solo porque exista un objeto.
5. **Aprobación:** generada ≠ auditada ≠ aprobada ≠ grabada; aprobación expresa cambia solo columna G de la fila pertinente en Sheets; conservar H y releer. El Sheet vivo prevalece sobre resúmenes históricos.
6. **Recuperación:** ante fallo, diagnóstico y hasta tres rutas técnicas seguras tras inspeccionar efectos parciales. «Hazlo» significa ejecutar, no proponer para después.

## Cierre de clase aprobado y actualización de estado — 2026-11-14

Cuando el usuario apruebe explícitamente una clase concreta (por ejemplo, «esta clase está aprobada»), **ejecutar en ese mismo turno** el protocolo de cierre del `course-class-producer`: identificar la clase a partir del contexto y verificar su ID/fila en el Google Sheets vivo; marcar **únicamente** `Aprobada = TRUE` si todavía no lo está; preservar `Grabada` y demás columnas; releer el rango editado; actualizar `PROJECT_STATE.md` en GitHub con fecha, clase, diapositivas, revisión real, estado de aprobación/grabación y siguiente clase; releer el archivo para confirmar persistencia. No pedir al usuario que repita la orden de actualizar el estado ni editar una clase ya aprobada. Si una fuente no está disponible, informar claramente qué se verificó y qué quedó sin sincronizar, sin simular éxito. La aprobación no equivale a grabación ni autoriza producir la siguiente clase. Este es un **cierre activado por la aprobación en la conversación**, no una sincronización continua en segundo plano.

**Reutilización de focos gráficos:** cuando el usuario remita a otra diapositiva aprobada como referente exacto, inspeccionar **ambas imágenes base, su geometría intrínseca y el elemento de foco**. No copiar/escala una superposición sobre una imagen base de composición distinta. Preservar la relación espacial local entre imagen y resaltado, inspeccionar render posterior y corregir desplazamientos antes de afirmar conformidad; no tocar otras diapositivas.


## Auditoría de centrado texto–contenedor — 2026-11-15
En clases existentes, una queja por texto descentrado exige **auditar todos los rótulos de la clase activa**, no solo el señalado. Aplicar el protocolo reproducible de `references/visual-composition.md`: identificar cada pareja texto/contenedor, calcular centros a partir de dimensiones y transformaciones reales, comparar X/Y, corregir traslaciones preservando escalas y releer el resultado. Alineaciones `CENTER`/`MIDDLE` no prueban centrado de la caja. Rótulos compuestos requieren criterio óptico distinto; la comprobación geométrica no sustituye la inspección del render. Registrar las regresiones en `course-class-producer/tests/cases.md`.

## Regla transversal — correcciones tras feedback de clase 5.2 (2026-11-15)
Ante instrucciones de corregir una clase existente: (1) releer la versión nativa actual e identificar las modificaciones manuales más recientes del usuario; (2) preservar la jerarquía visual entre función NIST, categoría y subcategorías; (3) asegurar márgenes internos suficientes **sin generar wrapping o clipping** al estrechar texto; (4) preferir líneas/conectores nativos con endpoints realmente conectados y semántica correcta, no glifos decorativos; (5) volver a leer objeto, texto y notas, e inspeccionar el render efectivo antes de declarar acabado visual validado. Consultar `references/visual-composition.md` y `skills/course-slide-builder/SKILL.md`. Regresión: clase 5.2, páginas 45, 47, 48 y 50.

## Política general de diseño preventivo y triple validación — 2026-11-15
Todos los criterios refinados (precisión NIST, jerarquía, fuente, identidad, color funcional, legibilidad, márgenes, centrado, simetría, longitudes y terminaciones de flechas, relaciones, composición global, redundancia, notas, editabilidad, coherencia entre slides y fidelidad al máster) son **obligatorios en tres fases**: **1. Antes de diseñar/planificar:** especificar propósito, layout y restricciones geométricas y conceptuales de la slide completa, incluyendo la relación de cada gráfico con otros elementos; **2. Durante implementación:** mantener y recalcular invariantes entre objetos dependientes tras cada modificación, conservando modificaciones manuales del usuario; **3. Durante auditoría:** contrastar storyboard, objetos nativos y render real a escala de componente, gráfico, diapositiva y clase; ejecutar regresión y reportar qué está comprobado y qué no. Seguir la matriz detallada en `references/visual-composition.md` y la orquestación de `skills/course-class-producer/SKILL.md`. Nunca declarar aprobado por mera persistencia/API. Caso 5.2: líneas de GV.OC-02 debían prever igual longitud arriba/abajo y alineación contextual; dos grupos pueden estar correctamente centrados internamente y aun así quedar mal con relación al cuadro izquierdo.

## Protocolo obligatorio de auditoría conceptual y visual — 2026-11-16
- En CADA propuesta SVG y CADA diapositiva implementada, incluir **dos auditorías independientes**: (a) representación conceptual, una fila y nota decimal 0–10 por símbolo/relación; (b) auditoría visual/general con precisión NIST, claridad, acabado, geometría, distribución, jerarquía, legibilidad, coherencia con familia, utilidad pedagógica y **ausencia de redundancia**. No esconder una mala nota conceptual detrás del promedio general.
- **Representación conceptual de la idea** mide si el símbolo comunica por sí mismo el concepto (prueba sin etiqueta); registrar ambigüedades e interpretaciones alternativas, la relación semántica, la dirección correcta y una mejora concreta. Objetivo ≥9,0/10 de promedio y ningún símbolo principal <8,5; si falla, indicar NO APROBADO y corregir antes de aprobación.
- Flujo editorial **propuesta SVG 16:9 visible → optimizar y auditar ambos ejes → aprobación explícita → construir mediante formas nativas editables en Google Slides → exportar/renderizar → inspeccionar la imagen realmente visible → auditar de nuevo ambos ejes → corregir y repetir QA → aprobación final del usuario**. El dato de la API o la existencia de un thumbnail NO equivale a inspección de la imagen. Si no se puede examinar el render, declarar auditoría visual pendiente.
- Aprobación de propuesta y aprobación definitiva de slide son estados distintos. Congelar diapositivas aprobadas: GV.OC-01 (slide 46), GV.OC-02 (47), GV.OC-03 (48); GV.OC-04 (49) aprobada por el usuario tras restaurar el icono Capacidades de cuadrado con check. No realizar cambios a una slide aprobada fuera de alcance, salvo petición posterior explícita.
- Caso de regresión 49: para **Capacidades**, la preferencia aprobada es cuadrado azul marino con check cian, NO sustituirlo por engranaje/herramienta por criterio autónomo del asistente. Mantener diana para Objetivos. Confirmar que «SERVICIOS CRÍTICOS» esté centrado verticalmente igual que las etiquetas hermanas: propiedades `contentAlignment=MIDDLE`, altura de marco coherente, texto sin salto de línea involuntario, y verificación visual real. Evitar que la reducción de fuente para una etiqueta larga deteriore la jerarquía; priorizar ancho y márgenes.
- Caso 48: balanza para Legal; libro abierto con § para Normativo; documento con cláusulas y firma para Contractual (no apretón de manos); ojo tachado para Privacidad (no escudo/candado genérico); ciudadanos + globo de diálogo para Libertades civiles (no persona abstracta con brazos abiertos). La especificidad de un icono prevalece sobre la apariencia decorativa. Etiquetas simples, no duplicarlas con subtítulos que repiten el significado.
- Para GV.OC-04 (49), la flecha desde organización hacia terceros expresa la **dependencia o expectativa de terceros de resultados/capacidades/servicios que recibe de la organización**. No invertirla: GV.OC-05 presenta las dependencias entrantes de la organización. No inventar el carácter crítico de un servidor solo por usar su icono; valorar individualmente la inferencia semántica y la etiqueta.

## Patrón gráfico aprobado — foco único y flechas a cajas breves (2026-11-16)
Regla para diapositivas conceptuales con UN objeto central y varias acciones o relaciones: usar un solo gráfico protagonista inequívocamente identificado, con flechas nativas que parten de él hacia cajas de texto corto (verbo y complemento conciso). El gráfico debe hacer explícito QUÉ se caracteriza o gestiona; evitar lupa, estrella, check, documento o tendencia ascendente genéricos si no transmiten la identidad del objeto. Evitar párrafos, ejemplos y adornos en las cajas; desarrollar el significado en la narración. Las flechas representan relaciones reales, no secuencia temporal, aprobación ni causalidad inventadas. Alinear simétricamente ramas, conectores y cajas, con márgenes suficientes, sin clipping, y balancear el conjunto frente a la columna NIST izquierda. Mantener Inter, paleta del curso, figuras oficiales intactas y objetos editables.
Referencia editorial aprobada: GV.RM-07, diapositiva 59: protagonista «OPORTUNIDAD ESTRATÉGICA», ramas «CARACTERIZAR — Beneficios y condiciones» e «INCLUIR — En la discusión de riesgos». La regla es preferente SOLO cuando la semántica lo justifica: no sustituye figuras oficiales NIST, jerarquías, cronologías, comparaciones u otros gráficos que requieran relaciones diferentes.
Puertas obligatorias: (1) planificar foco, etiquetas, sentido semántico de flechas y simetría; (2) implementar con objetos y conexiones nativas, conservar texto oficial y notas; (3) auditar cada símbolo/relación y la composición, texto, desbordes y render real observado. Las dos auditorías independientes siguen obligatorias. Aprobación de propuesta no equivale a aprobación de la slide o de la clase.
