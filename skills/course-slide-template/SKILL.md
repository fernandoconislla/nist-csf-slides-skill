---
name: course-slide-template
description: Proponer y, tras aprobación explícita, crear una plantilla Google Slides para cualquier curso, basada en su temática, una paleta de tres colores y tipografía adecuada.
---

# Course Slide Template — v0.2.0

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
