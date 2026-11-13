---
name: course-curriculum-builder
description: Investigar y estructurar temarios de cursos en secciones, clases y puntos de contenido, con títulos claros, didácticos y orientados a conversión; entregar un Google Sheets editable.
---

# Course Curriculum Builder — v0.2.0

## Objetivo
Transformar un tema o fuentes de referencia en un temario de curso listo para revisión editorial y desarrollo posterior, sin perder fidelidad técnica. El resultado debe ser pedagógicamente progresivo y atractivo para estudiantes potenciales de Udemy.

## Entrada
Basta con **una** entrada informativa suficiente: tema/título provisional, URL o documento de referencia, o temario existente. Opcionalmente: objetivos de aprendizaje, público, nivel, idioma, duración, enfoque teórico/práctico, herramientas/laboratorios, competencias previas, cursos competidores, contenidos obligatorios/excluidos y restricciones.

No bloquear la generación porque falten entradas opcionales. Cuando existan referencias oficiales, contrastar versiones, identificar su alcance y diferenciar la fuente del diseño pedagógico propio. No inventar estadísticas de demanda o ventas.

## Estructura de salida
Jerarquía estricta: **Sección → Clase → Punto de contenido**. Los puntos delimitan aquello que se enseñará; no son necesariamente diapositivas ni clases nuevas.

Ejemplo de IDs: 03, 3.1 y 3.1.1. Evitar duplicaciones y vacíos de alcance entre clases.

## Nombres editoriales: regla obligatoria
Los títulos de sección, clase y punto de contenido deben optimizarse para:
1. **Claridad inmediata:** entender de qué trata sin releerlo.
2. **Valor didáctico:** lenguaje accesible y específico para la audiencia y nivel.
3. **Progresión:** avanzar de fundamentos a aplicación, con prerrequisitos correctos.
4. **Intención del estudiante:** reflejar problemas, capacidades o resultados realmente abordados.
5. **Conversión honesta:** despertar interés y comunicar utilidad sin clickbait, superlativos no sustentados ni promesas que el contenido no cumple.
6. **Precisión técnica:** denominaciones, acrónimos, versiones y referencias correctos.
7. **Concisión y escaneabilidad:** evitar títulos largos, redundantes y genéricos; legibles en móvil y en la interfaz de Udemy.
8. **Consistencia:** misma convención de capitalización, terminología, longitud y nivel de detalle para temas equivalentes.
9. **Diferenciación justificada:** no copiar mecánicamente temarios competidores ni inventar ventajas.
10. **Naturalidad:** evitar frases prefabricadas, sobreventa y tono artificial.

Preferir títulos orientados al concepto o habilidad específica. No añadir automáticamente fórmulas como «Domina», «Definitivo», «desde cero» o «paso a paso». Usar verbos de acción cuando mejoran la precisión, no por obligación. No forzar palabras clave SEO en todos los títulos.

### Función de cada nivel
- **Sección:** bloque formativo reconocible y coherente.
- **Clase:** unidad de aprendizaje delimitada, cuyo título anticipa su tema o resultado.
- **Punto de contenido:** descripción concreta del concepto, procedimiento o ejercicio dentro de esa clase; suficientemente explícita para guiar la producción sin convertirse en guion detallado.

## Flujo
1. Interpretar entradas e investigar fuentes, con trazabilidad de referencias.
2. Identificar objetivos, competencias y límites de alcance.
3. Construir sección, clase y puntos de contenido.
4. Auditar cobertura, redundancias, secuencia, carga de cada clase, precisión, valor práctico y títulos.
5. Presentar propuesta editorial; permitir cambios.
6. Generar un **Google Sheets nativo y editable por el usuario**.
7. Considerar la hoja actualizada como fuente vigente. Para cambios posteriores, volver a leer la versión en vivo y conservar las ediciones realizadas por el usuario.

## Google Sheets
Dos vistas sugeridas:
- **Temario:** secciones y clases para visión general.
- **Puntos de contenido:** identificador de sección, de clase, de punto y descripción, con seguimiento cuando corresponda.

No sustituir títulos modificados manualmente por el usuario sin autorización. Mantener numeración coherente al insertar o eliminar elementos. No forzar aprobación de un título mediante una puntuación ficticia: justificar hallazgos de auditoría con ejemplos y correcciones concretas.

## Auditoría obligatoria, integrada a cada generación

**No entregar solo el temario.** Cada ejecución de generación o regeneración debe incluir una auditoría del resultado real y sus correcciones, con un resumen visible al usuario y registro editable en la hoja `Auditoría` del mismo Google Sheets.

### Criterios independientes
1. **Precisión técnica y vigencia:** comprobar versiones, términos, estándares y afirmaciones contra fuentes disponibles.
2. **Cobertura y pertinencia:** identificar competencias esenciales omitidas, contenidos irrelevantes y adecuación al objetivo formativo.
3. **Progresión didáctica:** secuencia lógica, prerrequisitos, aumento gradual de dificultad y conexiones entre secciones.
4. **Delimitación de clases:** evitar solapamientos, redundancia, fragmentación artificial y clases excesivamente amplias.
5. **Calidad de puntos de contenido:** especificidad suficiente para desarrollar la clase sin confundirlos con diapositivas.
6. **Claridad y naturalidad de títulos:** comprensión inmediata, fluidez, lenguaje humano y ausencia de clichés o texto artificial.
7. **Valor percibido y conversión honesta:** títulos atractivos, promesa concreta, público y beneficio comprensibles, sin clickbait ni exageraciones.
8. **SEO relevante para Udemy:** terminología buscable e intención de búsqueda cuando haya evidencia; no declarar volúmenes de búsqueda o tasas de conversión sin datos.
9. **Legibilidad móvil y concisión:** títulos escaneables, longitud razonable, acrónimos introducidos y jerarquía visual.
10. **Equilibrio entre teoría y práctica:** ejercicios, casos o laboratorios cuando el objetivo y los recursos lo justifiquen.
11. **Viabilidad y carga lectiva:** alcance realista para duración, nivel, materiales y recursos disponibles.
12. **Consistencia curricular:** numeración, convenciones de títulos, terminología y ausencia de saltos o duplicados.
13. **Fidelidad y trazabilidad de referencias:** distinguir fuente oficial, interpretación docente y contenido añadido; señalar lagunas de verificación.

### Método de auditoría
- Realizar una **auditoría preliminar** del borrador, corregir defectos concretos y luego auditar **la versión final realmente entregada**.
- En cada criterio emitir `Cumple`, `Requiere ajuste` o `No verificable`, con **evidencia específica** (sección, clase, punto o fuente), hallazgo, impacto y acción correctiva. Evitar puntuaciones arbitrarias sin rúbrica verificable.
- Clasificar hallazgos como **Crítico**, **Mayor** o **Menor** según su impacto en precisión, aprendizaje y comercialización. Un error técnico material es crítico y requiere corrección antes de entrega.
- Documentar `Antes → Después` cuando se cambien títulos, secuencia o cobertura; no realizar cambios invisibles.
- Si un criterio no puede verificarse por falta de información, registrarlo como `No verificable`, nunca como aprobado.
- La auditoría de conversión/SEO es una evaluación editorial; no equivale a una predicción cuantitativa de ventas.

### Entregable y pestañas de Google Sheets
1. **Temario:** visión condensada de secciones y clases, con identificadores y seguimiento editable.
2. **Puntos de contenido:** cada punto vinculado a su clase con numeración jerárquica y seguimiento opcional.
3. **Auditoría:** criterio, estado, severidad, evidencia/ubicación, hallazgo, ajuste aplicado o pendiente y fuente si procede.

Mostrar además al usuario un **resumen ejecutivo de auditoría junto al enlace**, que indique qué se corrigió, qué sigue pendiente y qué no se pudo verificar. El documento sigue siendo totalmente editable por el usuario.

## Entregable final
Un Google Sheets nativo con las tres pestañas anteriores y una auditoría adjunta en la respuesta. El Google Sheets actualizado es fuente de verdad para las skills de guiones y diapositivas; releer antes de usar y preservar cambios manuales.
