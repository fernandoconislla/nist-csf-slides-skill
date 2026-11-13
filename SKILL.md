---
name: nist-csf-slides
description: Diseñar y auditar diapositivas del curso NIST CSF 2.0 siguiendo una plantilla nativa de Google Slides, la identidad visual acordada y prompts de ilustraciones consistentes.
---

# NIST CSF 2.0 — Skill de diapositivas


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