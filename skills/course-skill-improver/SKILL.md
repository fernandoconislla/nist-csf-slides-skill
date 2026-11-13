---
name: course-skill-improver
description: Analizar retroalimentación y correcciones del usuario sobre resultados de skills para proponer, aprobar, versionar y probar mejoras permanentes sin alterar otros proyectos inadvertidamente.
---

# Course Skill Improver — v0.1.0

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
