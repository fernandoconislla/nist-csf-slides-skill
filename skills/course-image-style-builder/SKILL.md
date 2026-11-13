---
name: course-image-style-builder
description: Analiza una imagen visual de referencia y el tema de un curso; integra la paleta aprobada para producir un sistema gráfico y prompt maestro reutilizable en todas las imágenes de apoyo de sus diapositivas.
---

# Course Image Style Builder — v0.1.0

## Objetivo y límites
Generar y versionar **una línea gráfica maestra para las ilustraciones del curso**, no la plantilla de diapositivas ni las diapositivas terminadas. El artefacto principal es un `course-image-style.md` por curso, consumido por posteriores generadores de imágenes. Debe producir imágenes de diferentes conceptos con **consistencia de estilo** sin copiar el contenido ni la composición exacta de la imagen de referencia.

Trabaja después de `course-slide-template`: recibe su paleta y tipografía aprobadas (la tipografía no obliga a insertar texto dentro de ilustraciones). No modificar los archivos o prompts aprobados de otros cursos.

## Entradas
- **Contexto:** título del curso, disciplina, público y tono, cuando estén disponibles.
- **Paleta:** tres colores aprobados por `course-slide-template`: principal oscuro, secundario luminoso visualmente afín y blanco #FFFFFF. Si aún no está aprobada, solicitar o reutilizar la decisión pertinente; no declarar definitivo un sistema dependiente de ella.
- **Imagen de referencia:** archivo, captura o imagen accesible para el análisis; puede contener una o varias ilustraciones si se especifica qué elementos estudiar.
- **Preferencias opcionales:** restricciones, formato/aspecto, iconos o logotipos oficiales, estilo de ilustración, gráficos aceptados/rechazados, necesidad de fondo transparente, generador previsto.

Si se proporciona solo el título, proponer una dirección artística inicial y explicar que la extracción precisa de geometría, perspectiva, sombras y composición **requiere imagen referencial**. No afirmar que se analizó algo no recibido.

## Análisis visual de referencia: exhaustivo y observable
Registrar atributos observables y separar **observaciones** de **interpretaciones**:
1. **Composición:** sujeto dominante, foco, balance, simetría/asimetría, tercios, jerarquía, direccionalidad, márgenes, encuadre, densidad y zonas vacías.
2. **Geometría:** formas primarias, proporciones, módulos, alineaciones, bordes, esquinas, grosor de trazo, contornos y radios aparentes.
3. **Perspectiva:** frontal, ortográfica, isométrica, axonométrica, 2.5D, 3D u otra; ángulos observables, escala y consistencia.
4. **Profundidad y volumen:** capas, oclusiones, extrusión, planos, relieve, sombras proyectadas y oclusión ambiental visible.
5. **Color y contraste de la referencia:** tonos, distribución de masas cromáticas, saturación, contraste, opacidad; distinguir el estilo del color particular, que puede sustituirse por la paleta aprobada.
6. **Iluminación y acabados:** dirección, suavidad, highlights, reflejos, brillos, gradientes, texturas, materiales.
7. **Ilustración e iconografía:** abstracción, complejidad, simplificación, coherencia de símbolos, escala y tratamiento de figuras humanas.
8. **Fondo y espacio negativo:** blanco, transparente, degradado o entorno; sujeto aislado o escena; compatibilidad con el fondo blanco de las diapositivas de desarrollo.
9. **Tipografía/textos visibles:** uso o ausencia de palabras, etiquetas, letras técnicas, legibilidad; no inferir tipografías exactas cuando no pueden identificarse.
10. **Reproducibilidad:** atributos que deben conservarse globalmente y atributos variables por cada concepto.
11. **Elementos oficiales:** logos, emblemas y diagramas con colores/relaciones que no deben alterarse para encajar la estética.
12. **Incertidumbre:** cualquier propiedad no observable debe marcarse como estimación, no como hecho.

No extraer únicamente adjetivos vagos (`premium`, `tech`, `moderno`). Traducir cada atributo importante a instrucciones operativas comprobables.

## Síntesis con la identidad del curso
- Interpretar el tema y adaptar la iconografía a conceptos pertinentes sin recurrir a clichés por defecto.
- **Precedencia cromática:** colores del curso aprobados > colores de la imagen referencial > convenciones estéticas inventadas. La imagen aporta *estilo y composición*, no reemplaza automáticamente la paleta.
- Mantener los tres colores base del curso; permitir matices para sombras/luces derivados de ellos si son imprescindibles, sin convertirlos en colores de marca adicionales.
- Preparar ilustraciones para **integrarse en diapositivas 16:9 de desarrollo con fondo blanco puro**, con recursos independientes, espacio negativo y legibilidad a escala de proyección.
- El formato de cada recurso (cuadrado, vertical, horizontal, transparente) dependerá del contenido/ubicación; no confundir formato del recurso con formato de la diapositiva.
- No fijar un mismo layout para todas las imágenes: preservar estilo (geometría, perspectiva, iluminación, contornos, densidad), pero variar composición según el concepto y la futura diapositiva.
- Evitar texto decorativo y acrónimos generados dentro de ilustraciones por defecto. Etiquetas técnicas precisas se componen preferentemente como texto editable en Google Slides.
- No deformar diagramas oficiales; en lugar de recrear de memoria, usar material oficial con atribución cuando corresponda.

## Propuesta visual y aprobación
Mostrar antes de fijar el prompt maestro:
- Resumen de hallazgos de la referencia y estilo dominante.
- Decisiones de reinterpretación y correspondencia con la paleta HEX.
- Sistema de composición, geometría, perspectiva, iluminación y tratamiento de objetos.
- Reglas positivas y negativas, con explicación de excepciones.
- Un **ejemplo de prompt de ilustración** para un concepto real del curso, y cuando sea factible una vista previa visual identificada como provisional.
- Preguntar si aprueba o solicita ajustes. **No declarar aprobado ni final el prompt sin confirmación explícita**.

## Artefactos de salida
Tras aprobación, entregar:
1. **`course-image-style.md`** — prompt maestro y especificación reutilizable según `references/output-template.md`.
2. **`course-image-style.json`** opcional — parámetros estructurados (versión, paleta, geometría, perspectiva, sombras, texturas, fondo, negativas, procedencia).
3. Registro de referencia, decisiones, versión y auditoría de calidad.
4. Un prompt de aplicación **por ilustración**, formado por prompt maestro + concepto específico extraído del plan de diapositivas + restricciones de ese recurso.
No producir imágenes finales para todas las clases ni generar diapositivas por defecto. No subir imágenes referenciales privadas a un repositorio público sin autorización específica.

## Interfaz con el generador de imágenes
**Entrada por imagen:** ID de curso + versión aprobada del prompt maestro + concepto/objetivo visual + tipo de representación + proporción/área disponible + eventual fuente oficial.

**Salida esperada:** ilustración del concepto, aislable e integrable en Google Slides, consistente con el estilo maestro.

**Fórmula:** `PROMPT_MAESTRO_APROBADO + CONCEPTO_ESPECIFICO + RESTRICCIONES_DE_COMPOSICION + REGLAS_TECNICAS`.

El prompt maestro debe permanecer estable durante un curso. Cambios globales posteriores deben pasar por `course-skill-improver` o una revisión explícita de la identidad del curso, con nueva versión y aprobación, para no provocar cambios silenciosos entre clases.

## Auditoría obligatoria
Realizar `proponer → auditar → corregir → aprobar → entregar → verificar`. Evaluar por separado:
1. Fidelidad observable a la referencia y separación entre observación/inferencia.
2. Integración cromática con la paleta aprobada y contraste en fondo blanco.
3. Reglas de geometría, perspectiva, volumen, iluminación y acabados suficientemente reproducibles.
4. Consistencia entre conceptos distintos **sin copiar composiciones rígidas**.
5. Compatibilidad con la plantilla 16:9 y con su zona de contenido disponible.
6. Simplicidad, legibilidad, densidad y escalabilidad en proyección.
7. Coherencia temática e iconografía técnicamente apropiada.
8. Respeto a logotipos/diagramas oficiales y precisión de etiquetas.
9. Ausencia de decoraciones, textos o elementos innecesarios.
10. Claridad del prompt maestro, reglas positivas y negativas y excepciones.
11. Versionado, trazabilidad de fuente y estado de aprobación.
12. Prueba de consistencia con **al menos dos conceptos diferentes**, cuando haya herramientas de generación disponibles; no declarar comprobada la prueba visual si solo se inspeccionó el prompt.

Estados: `Cumple`, `Requiere ajuste` o `No verificable`, con hallazgo, evidencia y corrección. No asignar puntuaciones arbitrarias. Los fallos graves de fidelidad, contraste o precisión impiden aprobar la especificación final.

## Relación con otros módulos
- `course-slide-template`: propietario de paleta, tipografía y estructura fija de diapositivas.
- `course-curriculum-builder`: define qué temas se imparten.
- `course-lesson-builder`: define qué se explica y el texto en pantalla.
- Planificador y generador de diapositivas (futuros): determinan el objetivo visual de cada recurso.
- Esta skill: **únicamente** define y conserva el lenguaje gráfico maestro de las ilustraciones.
- `course-skill-improver`: incorpora feedback aprobado al comportamiento global de la skill; no confundir reglas generales con parámetros propios de un curso.
