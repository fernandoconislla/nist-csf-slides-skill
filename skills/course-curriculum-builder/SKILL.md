---
name: course-curriculum-builder
description: Investigar y estructurar temarios de cursos en secciones, clases y puntos de contenido, con títulos claros, didácticos y orientados a conversión; entregar un Google Sheets editable.
---

# Course Curriculum Builder — v0.5.0

## Objetivo
Transformar un tema o fuentes de referencia en un temario de curso listo para revisión editorial y desarrollo posterior. **Cuando el usuario aporta referencias como base curricular, el temario debe cubrir íntegramente su contenido formativo pertinente, sin resumirlo, descartar temas por extensión ni omitir detalles requeridos.** El resultado debe ser pedagógicamente progresivo y atractivo para estudiantes potenciales de Udemy.

## Entrada
Basta con **una** entrada informativa suficiente: tema/título provisional, URL o documento de referencia, o temario existente. Opcionalmente: objetivos de aprendizaje, público, nivel, idioma, duración, enfoque teórico/práctico, herramientas/laboratorios, competencias previas, cursos competidores, contenidos obligatorios/excluidos y restricciones.

Los **enlaces a cursos competidores de Udemy son una entrada explícitamente opcional**: si existen, analizarlos; si no existen, producir el curso normalmente. No exigirlos ni inventar equivalentes.

No bloquear la generación porque falten entradas opcionales. Cuando existan referencias oficiales, contrastar versiones, identificar su alcance y diferenciar la fuente del diseño pedagógico propio. No inventar estadísticas de demanda o ventas.

## Regla prioritaria: cobertura integral de las referencias (obligatoria)

**Las referencias aportadas como base curricular son el alcance mínimo obligatorio del temario, no material opcional para resumir.** El temario debe representar todos los temas, subtemas, conceptos, procedimientos, prácticas, categorías, códigos y distinciones relevantes para aprender lo que la referencia enseña. No sintetizar varios temas independientes en una etiqueta genérica que oculte su contenido; cada elemento debe ser localizable en una sección, clase o **punto de contenido** explícito.

### Procedimiento de cobertura
1. **Inventario exhaustivo previo:** recorrer íntegramente cada fuente accesible, incluidos anexos, tablas, figuras, ejercicios y apartados pertinentes. Registrar el índice temático real a la granularidad mínima necesaria, no solo el índice visible del documento.
2. **Clasificación del material:** distinguir contenido formativo (obligatorio), metadatos/editorial (p. ej., copyright, bibliografía, créditos), referencias auxiliares y material ilegible o inaccesible. No excluir contenido formativo por decisión unilateral.
3. **Mapeo bidireccional:** asignar a cada unidad formativa un identificador de fuente (documento, versión, capítulo, página/sección) y uno o más identificadores curriculares (sección/clase/punto). Verificar también que cada punto del temario tenga fundamento o se marque como ampliación propuesta.
4. **Desglose suficiente:** si una unidad de referencia contiene varios conceptos distintos, crear los puntos de contenido necesarios. Se permite agrupar o reordenar para mejorar didáctica, **sin perder componentes ni profundidad temática planificada**.
5. **Escala antes que recorte:** si el material es extenso, aumentar número de secciones, clases y puntos y estimar la duración real. No reducir cobertura para alcanzar una duración deseada; señalar el conflicto y ofrecer una división en módulos, volúmenes o cursos, pero no eliminar temas sin aprobación expresa.
6. **Referencias múltiples:** integrar contenidos superpuestos sin repetición innecesaria, manteniendo trazabilidad de todas las fuentes. Detectar versiones incompatibles o contradicciones y señalarlas, no escoger silenciosamente.
7. **Validación final:** realizar una comparación completa inventario ↔ temario después de las correcciones editoriales. Una referencia no leída íntegramente, con páginas no accesibles o parcialmente extraída impide declarar «cobertura total verificada». Informar exactamente qué parte quedó sin comprobar.

### Prohibiciones
- No resumir una norma, libro, estándar, curso o documento extenso en unas pocas clases genéricas por conveniencia.
- No omitir capítulos, subapartados, prácticas, tablas técnicas relevantes o temas de examen por ser difíciles, repetitivos, avanzados o extensos.
- No confundir «mencionado en el título de una clase» con «cubierto con puntos de contenido específicos».
- No declarar 100 % de cobertura si existen unidades sin asignar, material no revisado o brechas de acceso.
- No convertir la obligación de cobertura en la reproducción literal del texto fuente: el entregable es un **temario original, reestructurado y trazable**, no una copia del documento.

Si el usuario indica que una fuente es solo de inspiración o contraste y no parte del alcance obligatorio, registrar esa condición explícitamente. Toda exclusión curricular debe estar autorizada o identificada como pendiente, nunca ocultada.

## Análisis competitivo opcional de Udemy

### Activación
Ejecutar este módulo **solo cuando el usuario facilite enlaces de cursos competidores, solicite investigar la competencia o autorice expresamente esa comparación**. Se aceptan varios enlaces. No aplicar automáticamente una estrategia comercial de otro curso.

### Procedimiento
1. Abrir cada enlace original y comprobar que corresponde al curso esperado; conservar la URL canónica y la fecha de consulta. Ignorar los parámetros de cupón para el análisis curricular.
2. Recopilar **solo información pública verificable**: título, subtítulo, objetivos declarados, público, nivel, requisitos, secciones, clases visibles, duración publicada, prácticas/plantillas anunciadas, actualización y reseñas cuando puedan comprobarse. Diferenciar anuncio comercial de contenido demostrado.
3. Crear una **matriz comparativa normalizada** de bloques de aprendizaje, progresión, granularidad, terminología, formatos de práctica y propuesta de valor. Registrar «No visible» donde Udemy o el acceso no muestren información; no imaginar puntos internos de las clases.
4. Comparar contra el inventario **obligatorio** de fuentes técnicas oficiales y el temario del usuario. Identificar: temas compartidos, oportunidades formativas válidas, lagunas de los competidores solo cuando observables, redundancias, alternativas de secuenciación y diferenciadores pedagógicos justificados.
5. Utilizar el análisis para **proponer** organización en secciones, clases, puntos de contenido, títulos y actividades; no tratar duración de los competidores como duración objetivo ni igualar su número de clases por conveniencia.
6. Diseñar una diferenciación **demostrable** en el temario, por ejemplo una evidencia o entregable práctico específico que el curso realmente desarrollará. No proclamar superioridad, ventas esperadas, rankings ni mayor profundidad sin respaldo.
7. Si la propuesta altera un temario existente, presentar `Antes → Después`, justificación y efecto sobre el mapeo de fuentes. No sobrescribir el Google Sheets vigente ni ediciones manuales sin aprobación del cambio.

### Jerarquía y restricciones
**Referencia técnica obligatoria > decisiones curriculares aprobadas por el usuario > hallazgos de competidores como inspiración editorial**. El contenido técnico relevante de la fuente obligatoria no puede omitirse aunque los competidores no lo enseñen. Una clase de un competidor no se convierte en contenido obligatorio solo por existir. No copiar literalmente descripciones extensas, guiones o temarios; crear estructura original. Evitar inferir ventas a partir de ratings, número de alumnos o duración.

### Salida verificable
Si hay competidores, incluir en la propuesta:
- Tabla **Competidor → evidencia y fecha → patrón curricular → implicación para nuestro curso**.
- Matriz de correspondencia `fuente oficial → tema propio → tratamiento observable en competidor` para contrastar la diferenciación sin confundir las fuentes.
- Recomendaciones editoriales y pedagógicas priorizadas con beneficios y riesgos.
- **Auditoría competitiva independiente**: veracidad de datos, cobertura observable vs. no observable, originalidad, diferenciación comprobable, compatibilidad técnica y ausencia de imitación artificial.

Las **cuatro pestañas originales siguen siendo obligatorias**. Cuando exista análisis de competencia, registrar las conclusiones en `Auditoría` y, si aporta claridad, añadir una **quinta pestaña opcional `Análisis competitivo`** con fuentes, evidencia y decisiones. No añadirla cuando no se haya solicitado competencia.

### Ejemplo de entradas del proyecto NIST CSF 2.0
- https://www.udemy.com/course/nist-csf-20-fundamentos-e-implementacion-practica/
- https://www.udemy.com/course/gestion-de-ciberseguridad-nist-csf-20-marco-actualizado/

Estas URLs son **referencias competitivas opcionales, no fuentes normativas obligatorias**. Se deben volver a consultar en ejecuciones futuras para evitar datos desactualizados.

## Estructura de salida
Jerarquía estricta: **Sección → Clase → Punto de contenido**. Los puntos delimitan aquello que se enseñará; no son necesariamente diapositivas ni clases nuevas.

Ejemplo de IDs: 03, 3.1 y 3.1.1. Evitar duplicaciones y vacíos de alcance entre clases.

## Granularidad competitiva del temario público (obligatoria)

**Udemy exhibe secciones y clases en el programa público; los puntos de contenido detallados del Google Sheets son una capa interna de producción.** Por tanto, cubrir un tema únicamente en un punto interno no garantiza que el alumno potencial perciba esa cobertura, profundidad y valor al comparar cursos.

### Decisión editorial sobre cada tema
1. Comparar la granularidad de las **clases públicamente visibles** de competidores cuando hayan sido proporcionados, frente a nuestras clases visibles y puntos internos. No inferir los puntos internos ni el desarrollo real del competidor.
2. Detectar las **brechas de visibilidad**: tema relevante que el competidor expone como clase y el curso propio deja oculto dentro de una clase de alcance excesivo. Registrar título visible del competidor, ubicación propia y evidencia.
3. Valorar promover un punto (o grupo coherente de puntos) a **clase independiente**, si reúne suficiente **autonomía didáctica**, profundidad real para desarrollar una narración útil, importancia para el estudiante, especificidad del resultado y capacidad de comunicar un beneficio o competencia de manera honesta.
4. Desagregar clases excesivamente amplias aun cuando no exista competidor, siempre que se justifique pedagógicamente y aumente la **visibilidad del valor** del curso.
5. Agrupar temas demasiado pequeños, dependientes o redundantes: **no multiplicar clases artificialmente ni crear microclases para aparentar extensión**. Ninguna clase se justifica solo porque un competidor la tenga.
6. Redactar títulos visibles concretos, atractivos, móviles y precisos; conservar los códigos técnicos y detalles exhaustivos en puntos y matriz de cobertura cuando no convenga ponerlos en el título.
7. Verificar que los nuevos títulos cumplen lo prometido con puntos específicos, narración plausible y ejercicios reales cuando se anuncien. No hacer promesas de talleres, auditorías o herramientas que no se desarrollarán.
8. Presentar `Antes → Después`, motivos de promoción/división/agrupación, efecto en cantidad de clases y correspondencia curricular; solicitar aprobación antes de modificar el Google Sheets original.

### Regla de equilibrio
La granularidad es una decisión de **diseño instruccional y percepción de valor** al mismo tiempo. Ni maximizar el número de clases ni minimizarlas por conveniencia. El criterio prioritario es: **hacer visible una unidad de aprendizaje suficientemente sustantiva sin fragmentar artificialmente conocimientos inseparables**.

### Auditoría específica
Comprobar:
- Cobertura visible de competencias y conceptos diferenciadores en títulos de clases.
- Brechas de visibilidad frente a competidores observables, cuando se hayan aportado URLs.
- Justificación para convertir puntos internos en clases independientes.
- Ausencia de microclases, relleno y redundancia introducidos por exposición comercial.
- Preservación de la trazabilidad fuente → clase → puntos y de la cobertura obligatoria.
- Alineación entre títulos/promesas públicas y contenidos internos efectivamente planificados.

Registrar hallazgos en `Auditoría` y, si existe, `Análisis competitivo`. No afirmar un aumento de conversiones sin datos medidos.

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
1. Interpretar entradas, revisar íntegramente las referencias base y construir un inventario exhaustivo de unidades formativas.
2. Identificar objetivos, competencias y alcance obligatorio de cada referencia; marcar lagunas de acceso.
3. Si hay competidores proporcionados, realizar el análisis competitivo opcional y registrar sus implicaciones sin sustituir la cobertura oficial.
4. Construir sección, clase y puntos de contenido, y mapear cada unidad de referencia a su destino.
4. Auditar cobertura unidad por unidad y después redundancias, secuencia, carga lectiva, precisión, valor práctico y títulos.
5. Presentar propuesta editorial; permitir cambios.
6. Generar un **Google Sheets nativo y editable por el usuario**.
7. Considerar la hoja actualizada como fuente vigente. Para cambios posteriores, volver a leer la versión en vivo y conservar las ediciones realizadas por el usuario.

## Google Sheets
Dos vistas sugeridas:
- **Temario:** secciones y clases para visión general.
- **Puntos de contenido:** identificador de sección, de clase, de punto y descripción, con seguimiento cuando corresponda.
- **Matriz de cobertura:** inventario exhaustivo de unidades formativas referenciadas, fuente y ubicación, punto(s) curricular(es) relacionados, estado de cobertura y observaciones. Cada fila debe poder auditarse y editarse.

No sustituir títulos modificados manualmente por el usuario sin autorización. Mantener numeración coherente al insertar o eliminar elementos. No forzar aprobación de un título mediante una puntuación ficticia: justificar hallazgos de auditoría con ejemplos y correcciones concretas.

## Auditoría obligatoria, integrada a cada generación

**No entregar solo el temario.** Cada ejecución de generación o regeneración debe incluir una auditoría del resultado real y sus correcciones, con un resumen visible al usuario y registro editable en la hoja `Auditoría` del mismo Google Sheets.

### Criterios independientes
1. **Precisión técnica y vigencia:** comprobar versiones, términos, estándares y afirmaciones contra fuentes disponibles.
2. **Cobertura integral y pertinencia (bloqueante):** cotejar cada unidad de contenido de cada referencia obligatoria contra puntos curriculares explícitos; registrar cualquier omisión, generalización excesiva o sección inaccesible.
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
14. **Análisis competitivo (condicional):** cuando se aporten URLs de competencia, verificar la información pública, originalidad y diferenciación pedagógica; si no se proporcionan, indicar `No aplica`, no penalizar el temario.
15. **Granularidad pública y valor visible:** verificar que temas sustantivos aparecen con nivel adecuado en títulos de clase y que los puntos internos no oculten valor comparativo; evitar la fragmentación artificial.

### Método de auditoría
- Realizar una **auditoría preliminar** del borrador, corregir defectos concretos y luego auditar **la versión final realmente entregada**.
- La auditoría de cobertura es **exhaustiva, por unidad de fuente**, no por muestreo. Registrar conteos comprobables de unidades identificadas, asignadas, pendientes y no verificables; no usar porcentajes si el inventario no está completo.
- Toda unidad formativa obligatoria sin correspondencia curricular es un hallazgo **crítico**. No presentar el temario como final íntegro mientras exista tal omisión; reparar o indicar explícitamente la limitación.
- En cada criterio emitir `Cumple`, `Requiere ajuste` o `No verificable`, con **evidencia específica** (sección, clase, punto o fuente), hallazgo, impacto y acción correctiva. Evitar puntuaciones arbitrarias sin rúbrica verificable.
- Clasificar hallazgos como **Crítico**, **Mayor** o **Menor** según su impacto en precisión, aprendizaje y comercialización. Un error técnico material es crítico y requiere corrección antes de entrega.
- Documentar `Antes → Después` cuando se cambien títulos, secuencia o cobertura; no realizar cambios invisibles.
- Si un criterio no puede verificarse por falta de información, registrarlo como `No verificable`, nunca como aprobado.
- La auditoría de conversión/SEO es una evaluación editorial; no equivale a una predicción cuantitativa de ventas.

### Entregable y pestañas de Google Sheets
1. **Temario:** visión condensada de secciones y clases, con identificadores y seguimiento editable.
2. **Puntos de contenido:** cada punto vinculado a su clase con numeración jerárquica y seguimiento opcional.
3. **Matriz de cobertura:** identificador y ubicación de la referencia, unidad temática, punto(s) del temario, estado (Cubierto / Pendiente / No verificable) y comentario.
4. **Auditoría:** criterio, estado, severidad, evidencia/ubicación, hallazgo, ajuste aplicado o pendiente y fuente si procede.
5. **Análisis competitivo (opcional):** tabla de fuentes y diferencias comprobables, solo cuando se hayan aportado competidores y facilite la revisión.

Mostrar además al usuario un **resumen ejecutivo de auditoría junto al enlace**, que indique qué se corrigió, qué sigue pendiente y qué no se pudo verificar. El documento sigue siendo totalmente editable por el usuario.

## Entregable final
Un Google Sheets nativo con las **cuatro pestañas** anteriores y una auditoría adjunta en la respuesta. La cobertura íntegra debe estar sustentada por la matriz; si existen limitaciones, declarar qué material no pudo revisarse. El Google Sheets actualizado es fuente de verdad para las skills de guiones y diapositivas; releer antes de usar y preservar cambios manuales.
