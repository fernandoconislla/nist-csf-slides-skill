# NIST CSF Slides Skill — Laboratorio de skills para cursos

Repositorio en evolución para crear materiales y plantillas de cursos Udemy. El módulo inicial se dedica a NIST CSF 2.0, mientras que las nuevas skills pueden ser reutilizables para otras disciplinas.

## Skills
- [Course Slide Template](skills/course-slide-template/SKILL.md): interpreta el título del curso, propone colores y tipografía, muestra las dos diapositivas base, solicita aprobación y después crea la plantilla nativa en Google Slides.

- [Course Curriculum Builder](skills/course-curriculum-builder/SKILL.md): genera y optimiza temarios de tres niveles en Google Sheets editable, con cobertura oficial, auditoría y comparación opcional de cursos competidores de Udemy.
- [Course Lesson Builder](skills/course-lesson-builder/SKILL.md): desarrolla una clase concreta desde el temario vigente; su primera salida es el guion de narración completo, con auditoría.

- [Course Skill Improver](skills/course-skill-improver/SKILL.md): transforma comentarios, correcciones y ejemplos en propuestas de reglas; solo actualiza skills tras aprobación, con registro, auditoría y pruebas de regresión.

- [Course Image Style Builder](skills/course-image-style-builder/SKILL.md): analiza referencias visuales, adapta su composición y estilo a la paleta aprobada y produce un prompt gráfico maestro reutilizable por curso. Incluye [plantilla de salida](skills/course-image-style-builder/references/output-template.md) y [pruebas](skills/course-image-style-builder/tests/cases.md).

- [Course Slide Builder](skills/course-slide-builder/SKILL.md): planifica unidades visuales desde la narración auditada, crea Google Slides editables con recursos gráficos y notas del presentador; incluye [plan de slides](skills/course-slide-builder/references/slide-plan-template.md) y [pruebas](skills/course-slide-builder/tests/cases.md).
- [Course Class Producer](skills/course-class-producer/SKILL.md): orquesta desde el nombre/ID de una clase la lectura del Sheets vigente, narración, gráficos, Slides, notas y auditoría; incluye [manifiesto de ejecución](skills/course-class-producer/references/run-manifest.md) y [pruebas](skills/course-class-producer/tests/cases.md).

## Flujo de producción de una clase
1. Leer la clase y sus puntos de contenido desde Google Sheets vigente.
2. Generar y auditar narración completa con `course-lesson-builder`.
3. Derivar y validar texto en pantalla desde la narración.
4. Reutilizar la plantilla y línea gráfica **aprobadas** para el curso.
5. Planificar slides y seleccionar/generar gráficos con `course-slide-builder`.
6. Construir Google Slides 16:9 editable con narración distribuida en notas.
7. Auditar cobertura, correspondencia pantalla/narración, gráficos y presentación final.

La orquestación corresponde a `course-class-producer`. El audio narrado reproducible requiere una fase distinta de inserción/sincronización; **notas del presentador no equivalen a audio**.

## Recursos legados y especializados
- [SKILL.md](SKILL.md): instrucciones iniciales para NIST CSF 2.0.
- [Prompt de ilustraciones](prompts/ilustracion-base.md): v0.1 reconstruido; pendiente de contrastar con el texto original.
- [Temario de sección 03](references/seccion-03.md): clases acordadas.
- [Historial](CHANGELOG.md): cambios versionados.

## Flujo de plantilla
1. Título del curso y entradas opcionales.
2. Interpretación editorial de la temática.
3. Propuesta de tema tech/profesional (principal oscuro potente, secundario luminoso y blanco puro) y tipografía.
4. Vista previa de portada de clase y diapositiva de desarrollo.
5. Aprobación explícita.
6. Creación de Google Slides editable, sin modificar la referencia.

La diapositiva de desarrollo siempre utiliza fondo blanco puro, título oscuro, línea del color secundario y un área de contenido vacía.

Referencia Google Slides:
https://docs.google.com/presentation/d/1LuxRkFk9y4Bb4dDNLOP0gZWYXc90A8TFcxFi4ER-F6A/edit

**Repositorio público:** no subir credenciales ni recursos confidenciales.