# Historial de cambios

## Course Class Producer 0.1.0 — 2026-11-13
- Creada la skill orquestadora `skills/course-class-producer/SKILL.md`.
- Entrada mínima: clase por nombre/ID en el contexto de un curso existente.
- Fuente de verdad: Google Sheets vigente, incluidos cambios del usuario; secuencia obligatoria hasta Slides final.
- Puertas de control para narración completa, paleta/template/estilo aprobados, storyboard, gráficos, notas y auditoría.
- Manifiesto de estados `references/run-manifest.md` y 10 casos de prueba.
- Prohibido declarar producción completa cuando no se haya verificado la incorporación real de notas.

## Course Slide Builder 0.1.0 — 2026-11-13
- Creada `skills/course-slide-builder/SKILL.md` para transformar guion auditado en diapositivas Google Slides 16:9 editables.
- Planificador de unidades visuales: sin imponer una slide por punto curricular.
- Correspondencia obligatoria Puntos → Narración → Slides y Pantalla → Narración.
- Integración de plantillas y estilo de ilustración aprobados; uso fiel de recursos oficiales.
- Narración por diapositiva en notas del presentador, con verificación; audio reproducible es fase independiente.
- Plantilla `references/slide-plan-template.md`, ocho pruebas de regresión y auditoría integral.


## Course Image Style Builder 0.1.0 — 2026-11-13
- Nueva skill `skills/course-image-style-builder/SKILL.md`.
- Análisis exhaustivo de referencias visuales: composición, geometría, perspectiva, profundidad, iluminación, materiales, iconografía y espacios negativos.
- Integración de la paleta aprobada con precedencia sobre los colores de la imagen de referencia.
- Salida: `course-image-style.md` por curso con prompt maestro y reglas de aplicación para cada recurso.
- Aprobación obligatoria del sistema visual y verificación con dos conceptos distintos cuando exista generador disponible.
- Plantilla de salida `references/output-template.md` y seis casos de prueba definidos en `tests/cases.md`.


## Course Skill Improver 0.1.0 — 2026-11-13
- Creada `skills/course-skill-improver/SKILL.md`, centrada en aprendizaje por feedback sin reentrenamiento.
- Clasificación de cambios locales, preferencias contextuales y reglas permanentes.
- Flujo: comparar → diagnosticar → proponer diff → aprobar → versionar → probar regresiones.
- Archivos `FEEDBACK.md`, `references/feedback-record.md` y `tests/cases.md`.
- Prohibición de modificar reglas permanentes sin aprobación explícita y protección de datos en repositorio público.


## Course Lesson Builder 0.2.0 — 2026-11-13
- Cobertura completa y obligatoria de todos los puntos de contenido de la clase en la narración.
- Orden obligatorio: puntos curriculares → narración auditada → texto en pantalla derivado de la narración.
- El texto en pantalla queda íntegramente explicado por la narración, pero la narración no necesita figurar completa en pantalla.
- Dos matrices: puntos → segmentos de narración y texto visible → segmentos de narración.
- Auditoría obligatoria de cobertura, correspondencia semántica y calidad didáctica; hallazgos críticos bloquean aprobación.
- Entregable conjunto: narración y propuesta de textos en pantalla, sin generar Google Slides por defecto.


## Course Curriculum Builder 0.3.0 — 2026-11-13
- Cobertura integral obligatoria de todas las referencias utilizadas como base curricular: sin resúmenes sustitutivos ni omisiones.
- Inventario exhaustivo de unidades formativas de las fuentes, incluidos apartados, tablas, figuras y prácticas pertinentes.
- Nueva matriz bidireccional de trazabilidad fuente → sección/clase/punto de contenido.
- Auditoría exhaustiva de cobertura, no por muestreo; omisiones críticas bloquean declarar el temario completo.
- El temario puede ampliarse para sostener el alcance y debe informar restricciones de acceso o duración.
- El Google Sheets pasa a cuatro pestañas: Temario, Puntos de contenido, Matriz de cobertura y Auditoría.


## Course Lesson Builder 0.1.0 — 2026-11-13
- Nueva skill modular `skills/course-lesson-builder/SKILL.md`.
- Entrada prioritaria: clase concreta, puntos de contenido y contexto actual del Google Sheets.
- Primera salida: guion de narración docente completo, natural, riguroso y listo para revisión.
- Mapa de cobertura, estimación de duración, fuentes y auditoría obligatoria con 13 criterios.
- Extensible en el futuro a texto en pantalla, prácticas y recursos, sin generarlos por defecto.


## Course Curriculum Builder 0.2.0 — 2026-11-13
- Auditoría obligatoria tanto de borrador como de entrega final.
- 13 criterios independientes: técnica, cobertura, pedagogía, títulos, conversión, SEO, móvil, viabilidad y fuentes.
- Nueva pestaña `Auditoría` en Google Sheets, con hallazgos, evidencia, severidad y ajustes.
- Resumen de auditoría incluido siempre en la respuesta; sin puntuaciones inventadas.

## Course Curriculum Builder 0.1.0 — 2026-11-13
- Nueva skill `skills/course-curriculum-builder/SKILL.md` para temarios editables de tres niveles.
- Criterios editoriales para títulos claros, didácticos y orientados a conversión honesta.

## 0.2.0 — 2026-11-13
- Nueva skill modular `skills/course-slide-template/SKILL.md` para futuros cursos Udemy.
- Interpretación del tema como paso obligatorio antes de recomendar identidad visual.
- Paleta base: color principal oscuro potente, secundario luminoso afín, blanco puro.
- Propuesta de tipografía contextual, sin imponer Inter.
- Estructura fija: apertura de clase con elemento gráfico y título; desarrollo blanco con título y barra separadora.
- Vista previa y **aprobación explícita antes de generar** la plantilla.
- Estética tech con presencia visual, evitando sobrecarga, saturación y mala legibilidad.

## 0.1.0 — 2026-11-13
- Estructura inicial de la skill NIST CSF.
- Prompt de ilustración reconstruido, pendiente de validación literal.
- Reglas de composición, precisión NIST y auditoría; enlaces de referencia.