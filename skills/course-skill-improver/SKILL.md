---
name: course-skill-improver
description: Analizar retroalimentación y correcciones del usuario sobre resultados de skills para proponer, aprobar, versionar y probar mejoras permanentes sin alterar otros proyectos inadvertidamente.
---

# Course Skill Improver — v0.1.0


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
Convertir correcciones, ejemplos aprobados/rechazados y comentarios del usuario en mejoras **controladas, comprobables y persistentes** de las skills del repositorio. No se trata de reentrenar el modelo: son cambios versionados a instrucciones, referencias, ejemplos y pruebas que el agente debe cargar en futuras ejecuciones.

## Entrada
Se acepta cualquiera de:
- Nombre/ruta de la skill objetivo y un comentario («los títulos son genéricos»).
- Resultado original más versión corregida (Google Sheets, Slides, Docs, texto, imagen de referencia).
- Comparación entre un resultado aprobado y uno rechazado, con o sin explicación.
- Auditoría o incidencia observada durante el uso.
Opcionales: prioridad, alcance del cambio (esta clase/curso o todos los cursos), enlaces, caso de uso y criterios de aceptación.

**No exigir un formulario.** Si falta una entrada imprescindible, pedir únicamente lo indispensable. Antes de comparar, leer la versión vigente y los archivos citados; al tratar archivos externos, preservar los permisos y no asumir que una URL implica autorización para editarla.

## Clasificación de la retroalimentación
Clasificar cada observación como:
1. **Corrección local del entregable**: solo modifica el temario, texto o diapositiva objeto de revisión.
2. **Preferencia contextual**: válida para un curso, temática o público determinados, no regla universal.
3. **Regla permanente de skill**: comportamiento reusable que mejora futuros resultados, sujeto a aprobación explícita.
4. **Error técnico / factual**: corregir con evidencia y evaluar si demanda una regla de validación.
5. **Conflicto o incertidumbre**: explicitar compensaciones y requerir decisión antes de cambiar instrucciones.

Nunca interpretar todas las ediciones manuales como una preferencia universal. No extrapolar una corrección aislada sin justificar su generalización; pueden proponerse reglas condicionales.

## Procedimiento obligatorio
1. **Captura:** registrar fecha, skill objetivo, versión/commit, artefacto original, artefacto corregido y comentario (enlaces o referencias, sin copiar datos sensibles al repo).
2. **Comparación:** analizar diferencias textuales, curriculares y/o visuales. Describir qué cambió con citas a ubicaciones reales (filas, celdas, diapositivas, fragmentos).
3. **Diagnóstico:** determinar causa probable: instrucción ausente, ambigua, contradictoria, insuficiencia de fuentes, fallo de ejecución o preferencia local. No declarar causa probada sin evidencia.
4. **Propuesta:** redactar una o más reglas breves, operativas y verificables. Indicar alcance, ubicación de archivo, ejemplos positivos y negativos, posibles conflictos y criterio de aceptación.
5. **Aprobación explícita:** presentar el diff propuesto en lenguaje comprensible. **No modificar permanentemente SKILL.md ni archivos de reglas sin autorización del usuario para esa propuesta concreta.** Una aprobación genérica de mejorar una skill no autoriza cualquier cambio futuro.
6. **Implementación:** con aprobación, volver a leer archivos y SHA actuales; aplicar edición mínima, versionar, registrar en `CHANGELOG.md` y `FEEDBACK.md`. Conservar instrucciones existentes salvo incompatibilidad aprobada.
7. **Pruebas:** ejecutar casos del archivo `tests/cases.md` y, cuando sea posible, una regeneración real con el mismo input. Comparar antes/después; detectar regresiones.
8. **Auditoría final:** informar criterios cumplidos, incumplidos o no verificables, evidencia, cambios aplicados y riesgos restantes. No declarar una mejora probada si solo se cambió texto de la skill.
9. **Verificación:** confirmar que los archivos están disponibles en la rama/commit esperados. Entregar enlaces a la regla, registro de feedback y pruebas.

## Prioridades de instrucciones y alcance
- Respetar instrucciones superiores, seguridad, documentación oficial, decisiones editoriales aprobadas y restricciones explícitas del usuario.
- Una mejora de persuasión, brevedad o diseño **no puede** reducir cobertura técnica obligatoria o introducir falsedades.
- Diferenciar instrucciones normativas de ejemplos de estilo.
- Preferir reglas condicionales para temas, públicos o modalidades distintos.
- Si una regla contradice otra, identificar ambas y proponer resolver la contradicción explícitamente.
- No modificar documentos o spreadsheets originales al analizar versiones, salvo solicitud explícita.

## Contrato de salida en fase de propuesta
Mostrar:
- Resumen de observación + evidencia rastreable.
- Comparación `Antes → Después`.
- Causa posible y grado de confianza.
- Tipo de cambio: local, contextual o permanente.
- Regla propuesta con texto exacto, archivo y sección de destino.
- Impacto esperado, posibles regresiones y prueba de aceptación.
- Solicitud de aprobación de la propuesta.

## Contrato de salida tras aprobación
- Diff o resumen exacto de cambios ejecutados.
- Commit/versiones y vínculos verificados.
- Resultado de pruebas: **Ejecutada y conforme / Ejecutada con fallos / No ejecutada**, según evidencia.
- Hallazgos pendientes, especialmente regresiones.
- Próximo ejemplo de validación si faltan datos.

## Auditoría obligatoria de la mejora
1. **Fidelidad al feedback**: regla aborda exactamente la insatisfacción.
2. **Evidencia**: diferencia sustentada en originales y correcciones realmente disponibles.
3. **Generalización**: evita convertir casos puntuales en restricciones universales.
4. **Claridad operativa**: condición, acción y resultado esperado verificables.
5. **Compatibilidad**: no contradice reglas existentes o resuelve explícitamente el conflicto.
6. **Seguridad y confidencialidad**: no publica datos, claves, enlaces privados ni contenidos sensibles en GitHub.
7. **No regresión**: casos aprobados previamente siguen cumpliéndose.
8. **Efectividad**: la nueva ejecución corrige el fallo original cuando se ha podido probar.
9. **Trazabilidad**: registro con versión, fecha, archivos y decisiones.
10. **Control de aprobación**: nunca aplica una regla permanente sin consentimiento explícito.

Estados: `Cumple`, `Requiere ajuste`, `No verificable`. Identificar gravedad y aportar evidencia; no inventar porcentajes o mejoras cuantificadas.

## Archivos de apoyo
- `FEEDBACK.md`: historial de solicitudes, decisiones y cambios.
- `references/feedback-record.md`: formato de captura y propuesta.
- `tests/cases.md`: conjunto inicial de pruebas y protocolo de regresión.
- `CHANGELOG.md` en la raíz: hitos de versión, sin reemplazar el historial detallado.

## Modo de funcionamiento
Esta skill **no vigila Google Sheets ni GitHub en segundo plano**. Se ejecuta al solicitar comparación, revisión, aprendizaje o actualización. Si se desea detectar ediciones nuevas automáticamente, se necesita un flujo de automatización explícito y autorizado. Cambiar el contenido de una skill no garantiza por sí solo que el modelo mejore: se debe cargar la nueva versión al ejecutarla y comprobar resultados.
