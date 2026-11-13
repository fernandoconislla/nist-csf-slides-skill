---
name: course-slide-template
description: Proponer y, tras aprobación explícita, crear una plantilla Google Slides para cualquier curso, basada en su temática, una paleta de tres colores y tipografía adecuada.
---

# Course Slide Template — v0.2.0


## Excepción de portada y prioridad de recursos visuales (obligatorio)

- **Portada de clase:** prevalece la identidad visual maestra ya aprobada del curso (fondo, paleta, tipografía, layout y elemento gráfico protagonista). NO reemplazar automáticamente el gráfico de portada por el logotipo, la portada del documento o la figura oficial del tema específico tratado en esa clase. Solo variar título y componentes intercambiables previstos por la plantilla, sin rediseñarla.
- **Diapositiva de desarrollo con elemento específico:** priorizar recurso institucional/oficial verificable (p. ej., logo NIST, portada de publicación NIST CSF 2.0 o figura normativa auténtica), frente a escudos genéricos, íconos inventados o ilustraciones IA que pretendan representarlo. Conservar colores, proporciones y relaciones oficiales; atribuir su procedencia.
- **Diapositiva conceptual o de proceso:** utilizar iconos, diagramas nativos editables o ilustración cuando favorezca comprensión. No forzar una imagen oficial a una idea abstracta ni duplicar el mismo recurso institucional entre slides.
- **Puerta de calidad:** antes de aprobar, contrastar por separado (a) fidelidad de la portada a la identidad del curso, (b) autenticidad de cada recurso específico en desarrollo y (c) legibilidad, centrado de las composiciones dentro del área de contenido, paleta y correspondencia con la narración. La falta de imágenes pertinentes o una portada alterada sin autorización bloquea la aprobación visual.

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
Crear la **plantilla visual**, no desarrollar la lección. Compatible con cursos Udemy de distintas disciplinas. Reutilizar la estructura geométrica de la referencia y adaptar su dirección artística al curso.

## Entrada
- Obligatoria: título del curso.
- Opcionales: audiencia, enfoque, tres colores, tipografía y preferencias visuales.
- Si faltan colores o fuente, **proponerlos** interpretando el título y, cuando exista, la audiencia.
- Si el usuario aporta parámetros, respetarlos y señalar eventuales problemas de contraste o lectura; no reemplazarlos sin aprobación.

## Interpretación artística obligatoria
1. Identificar disciplina, promesa del curso, nivel y carácter esperado.
2. Traducirlos a una dirección de arte coherente (p. ej. tecnológica, corporativa, experimental, académica).
3. Recomendar **una propuesta principal** con justificación concisa; ofrecer alternativas cuando el usuario las solicite.
4. No asignar una paleta fija por palabras clave ni usar automáticamente azul para toda la ciberseguridad.
5. Priorizar una estética tech potente, profesional, limpia y adecuada a la proyección en diapositivas, cuando sea coherente con el tema. Potencia visual no significa neones indiscriminados, efectos excesivos o fondos recargados.

## Sistema cromático
Exactamente tres colores base:
- **Principal:** tono oscuro, fuerte y de alto contraste, que domina la apertura y colorea títulos sobre blanco.
- **Secundario:** tono más luminoso y suave, de una familia cromática próxima o armoniosa con el principal. Debe ofrecer contraste visible y energía como acento (barra, fragmento del título).
- **Blanco:** `#FFFFFF`, obligatorio como fondo de las diapositivas de desarrollo.

Los dos primeros pueden pertenecer a una familia azul, verde, violeta, turquesa, rojo, naranja u otra elegida por interpretación del tema. No se exige monocromía matemática; sí coherencia cromática. Evitar acentos tan pálidos que desaparezcan en blanco. Evaluar contraste de títulos y barra. Los colores de activos oficiales no se alteran para encajarlos en la paleta.

## Tipografía
- Proponer una familia tipográfica según disciplina, personalidad, audiencia y legibilidad.
- Preferir fuentes accesibles en Google Slides y de lectura clara en proyección.
- Respetar la tipografía suministrada; justificar cualquier alternativa.
- En la plantilla de referencia, Inter es una opción, **no un valor fijo para todos los cursos**.

## Estructura fija de la plantilla
Referencia:
https://docs.google.com/presentation/d/1LuxRkFk9y4Bb4dDNLOP0gZWYXc90A8TFcxFi4ER-F6A/edit

Formato **16:9**, 13,333 × 7,5 pulgadas.

### 1. Apertura de cada clase
- Fondo principal oscuro.
- Elemento gráfico intercambiable y protagonista a la izquierda.
- Nombre/título de la clase a la derecha, con texto blanco y énfasis selectivo en color secundario.
- En la referencia: Inter Bold 40 pt; conservar proporciones y distribución como punto de partida, adaptando tamaño solamente por legibilidad.
- Títulos nativos editables y gráfico separado.

### 2. Desarrollo
- Fondo **blanco puro** invariable.
- Título arriba, alineado a la izquierda, en color principal oscuro.
- Línea separadora horizontal en color secundario.
- Gran zona blanca libre debajo para el contenido que una skill posterior colocará.
- En la referencia: Inter Bold 31,5 pt; título a ~0,58 pulgadas de arriba y ~0,83 pulgadas desde la izquierda; línea a ~1,54 pulgadas desde arriba y de grosor 1 pt.
- No agregar pies de página, tarjetas, logo, ornamentos ni bloques de contenido a la plantilla vacía.

## Propuesta y aprobación (punto de control obligatorio)
**Antes de crear o editar una presentación:** mostrar título del curso, interpretación del tema, concepto visual, paleta con códigos HEX, fuente recomendada y vistas previas de ambas diapositivas (apertura y desarrollo). Preguntar si aprueba o desea modificaciones. **No crear la plantilla final antes de recibir aprobación explícita** de esos elementos.

## Generación tras aprobación
- Crear una copia del diseño de referencia o derivar sus layouts respetando la estructura acordada.
- Mantener formas, líneas y texto como objetos editables de Google Slides.
- No modificar la presentación original.
- Validar colores, blancos puros, márgenes, lectura y preservación de relaciones geométricas.
- Verificar el resultado en Slides, aplicar correcciones y compartir enlace.

## Alcance y otras skills
Esta skill crea la identidad visual y los dos layouts. No redacta el temario, genera todas las slides de la clase ni crea el recurso gráfico específico. Para lo último, delegar en la skill de ilustraciones (`prompts/ilustracion-base.md`) una vez aprobada la dirección artística.

## Registro
Cada nueva regla aprobada debe registrarse y versionarse en GitHub. Distinguir explícitamente propuestas pendientes de aprobación de decisiones ya aprobadas.
