---
name: course-lesson-builder
description: Desarrollar el contenido completo de una clase específica de un curso, a partir del temario vigente y referencias. Su primera capacidad es generar un guion de narración docente riguroso, natural y listo para grabar.
---

# Course Lesson Builder — v0.1.0

## Misión y alcance
Convertir **una clase concreta** del temario en contenido docente desarrollable y verificable. La primera salida implementada es **la narración íntegra de esa clase**, lista para ser leída o adaptada durante la grabación. Arquitectura extensible para futuras salidas: texto de pantalla, diapositivas, demostraciones, actividades y materiales descargables.

No crear ni alterar el temario global (responsabilidad de `course-curriculum-builder`) ni construir la plantilla (responsabilidad de `course-slide-template`). No asignar una diapositiva por punto de contenido ni producir imágenes sin solicitud explícita.

## Entradas
**Mínima:** identificación inequívoca de la clase (p. ej. `3.1`) junto con el contexto del curso o un enlace a su temario.

**Preferidas:**
- Enlace al Google Sheets del temario vigente, nombre e identificador de clase.
- Título de la sección y puntos de contenido de esa clase, con su orden actual.
- Títulos o alcances de clases anteriores y siguientes para delimitar qué no repetir ni anticipar.
- Fuentes oficiales, PDFs, documentación técnica y URLs relevantes.
- Público objetivo, conocimientos previos, nivel, idioma y tono docente.
- Tipo de clase (conceptual, demostrativa, taller, laboratorio o mixta), duración deseada y recursos disponibles.
- Texto o narración ya escritos, cuando se solicite revisar o continuar.

Si el temario está en Google Sheets, **leerlo en vivo** antes de generar, incluidas las ediciones del usuario. Si hay información insuficiente pero la clase está inequívocamente identificada, investigar lo necesario y declarar las suposiciones significativas. Nunca inventar datos, comandos, resultados ni fuentes.

## Contrato de contenido
1. Resolver el objetivo de aprendizaje de la clase en una frase comprobable.
2. Preservar el título y los puntos de contenido aprobados y su alcance; no reescribir el temario por cuenta propia.
3. Desarrollar todos los puntos con suficiente profundidad para que la explicación se sostenga por sí misma.
4. Evitar temas futuros, redundancias con clases anteriores y ejemplos prematuros que creen confusión.
5. Introducir los conceptos antes de utilizar jerga no explicada. Mantener terminología consistente con el curso.
6. Diferenciar definiciones oficiales, interpretaciones pedagógicas, ejemplos hipotéticos y opiniones.
7. Si una práctica o demostración requiere pasos, describirlos con rigor y verificabilidad; no fingir ejecución.
8. No forzar ejemplos, analogías o historias cuando no mejoren la comprensión.
9. No inventar un tiempo exacto de narración: estimar con conteo de palabras y ritmo declarado, considerando pausas y demostraciones aparte.

## Primera salida: narración de la clase
Estructura editorial sugerida, adaptable al tipo de clase:
- Identificación: curso, sección, clase, versión y fuentes principales.
- Objetivo de aprendizaje.
- **Guion narrado completo**:
  - Apertura breve que sitúa el problema o resultado sin revelar innecesariamente temas futuros.
  - Desarrollo continuo de los puntos de contenido, en orden pedagógico.
  - Transiciones naturales y breves, sin frases de relleno ni repetir títulos literalmente.
  - Cierre que sintetiza lo aprendido sin volver a desarrollar toda la clase.
- Mapa de cobertura: punto de contenido → pasaje del guion.
- Estimación de duración (palabras / rango de palabras por minuto, más tiempo de demostraciones si procede).
- Fuentes y límites de verificación.
- Auditoría y cambios aplicados.

La narración debe poder pronunciarse de forma natural: frases claras, ritmo oral, precisión técnica, sin párrafos acartonados, listados recitados ni énfasis grandilocuente. Evitar «En el mundo actual...», «Es importante destacar...», «A continuación veremos...» repetido y otros signos de texto prefabricado. Adoptar español profesional, accesible al público definido. El texto debe aportar valor frase por frase.

### Relación con diapositivas futuras
El guion es el contenido maestro de la clase, pero no presupone una diapositiva por párrafo. En futuras extensiones, separar **texto en pantalla**, **narración**, **apoyo gráfico** y **acciones del instructor** sin perder alineación. El texto visible podrá ser mucho más breve que la narración. Las diapositivas de desarrollo usarán la plantilla aprobada por separado.

## Generación y auditoría obligatoria
Flujo: leer temario vigente → verificar referencias → delimitar objetivos y alcance → redactar → **auditar borrador** → corregir → **auditar salida final**.

Evaluar explícitamente:
1. **Fidelidad al temario**: todos los puntos incluidos; ninguno reemplazado u omitido.
2. **Precisión y actualidad técnica**: normas, versiones, términos y afirmaciones contrastados.
3. **Profundidad adecuada**: suficiente para el nivel, sin simplificación incorrecta ni digresiones.
4. **Progresión pedagógica**: prerrequisitos, orden y construcción de conceptos.
5. **Delimitación curricular**: no anticipa clases siguientes ni repite innecesariamente anteriores.
6. **Claridad de la explicación**: lenguaje directo, ejemplos útiles y comprensión autónoma.
7. **Naturalidad oral / AI slop**: sin lenguaje robótico, muletillas, estructuras mecánicas o conectores artificiales.
8. **Coherencia y continuidad**: transiciones y referencias internas consistentes.
9. **Valor práctico**: aplicación cuando es pertinente, sin prácticas ficticias o forzadas.
10. **Duración y densidad**: extensión consistente con el alcance y la modalidad.
11. **Trazabilidad de las fuentes**: citas o referencias específicas y límites de verificación.
12. **Grababilidad**: narración pronunciable, fragmentación manejable y sin instrucciones visuales recitadas.
13. **Correspondencia objetivo–desarrollo–cierre**: la clase cumple lo prometido.

Para cada criterio usar `Cumple`, `Requiere ajuste` o `No verificable` con evidencia concreta. Clasificar problemas como crítico, mayor o menor. Corregir errores críticos antes de dar por aprobado el guion. Informar cambios significativos `Antes → Después`, pendientes y fuentes no verificadas. No inventar puntuaciones ni dar por aprobado lo que no fue comprobado.

## Entrega y revisión
- Salida primaria: **guion completo de narración**, organizado para que el usuario pueda leerlo y editarlo, acompañado de mapa de cobertura y auditoría.
- Si el usuario pide documento, generar un documento editable; si pide solo narración, no imponer un formato adicional.
- No modificar Google Sheets ni registrar la narración en el temario salvo petición explícita.
- En revisiones, conservar los puntos aprobados y cambiar solo el alcance solicitado; auditar la versión revisada.

## Extensión
Futuras capacidades independientes podrán generar planes de diapositivas, texto en pantalla, actividades y recursos. No habilitarlas de forma implícita en la primera versión.
