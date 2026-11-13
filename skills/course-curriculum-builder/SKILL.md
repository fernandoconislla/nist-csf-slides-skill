---
name: course-curriculum-builder
description: Investigar y estructurar temarios de cursos en secciones, clases y puntos de contenido, con títulos claros, didácticos y orientados a conversión; entregar un Google Sheets editable.
---

# Course Curriculum Builder — v0.1.0

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

## Auditoría editorial antes de entrega
Comprobar cada título por claridad, precisión, especificidad, utilidad comunicada, coherencia con el nivel, escaneabilidad y ausencia de exageraciones. Distinguir títulos dirigidos a navegación curricular de títulos orientados a captación: ambos deben ser atractivos, pero los títulos internos no son anuncios.

## Entregable
Enlace a Google Sheets editable; las secciones y clases pueden consultarse de forma condensada, y los puntos de contenido en vista detallada. La hoja es la fuente de referencia para posteriores skills de guiones y diapositivas.
