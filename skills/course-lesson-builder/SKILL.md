---
name: course-lesson-builder
description: Desarrollar el contenido completo de una clase específica de un curso, a partir del temario vigente y referencias. Genera contenido completo de una clase: primero narración que cubra todos sus puntos de contenido y después texto en pantalla íntegramente respaldado por esa narración.
---

# Course Lesson Builder — v0.2.0


## Ciclo obligatorio de optimización y auditoría (regla transversal)

- No limitarse a detectar defectos: ejecutar **inspección → optimización efectiva → auditoría → corrección → auditoría de regresión**, iterando mientras existan problemas materiales solucionables.
- Evaluar **redundancia intra-clase e inter-clases**, progresión, cobertura, precisión normativa, proporcionalidad de contenidos y límites entre módulos. Comparar los puntos detallados del temario, no solo los títulos.
- Para cada cambio, documentar **antes → después, motivo, fuente, efecto sobre identificadores/cobertura, gravedad y estado**. Preservar decisiones aprobadas y cambios manuales; no eliminar contenido normativo ni alterar el archivo maestro sin autorización.
- Las repetición pedagógica solo se admite cuando cambia la función: introducción, explicación, práctica o evaluación con un aprendizaje distinto. No presentar teoría repetida como aplicación.
- Verificar de nuevo tras cada iteración que no existan omisiones, contradicciones ni nuevos solapamientos; la **auditoría de regresión es obligatoria**, no opcional.
- La salida debe distinguir **corregido y verificado**, **pendiente de validar** y **no aprobado**. Bloquear aprobación ante errores técnicos graves o pérdida de cobertura; evitar puntuaciones complacientes.
- Responsabilidades: `course-curriculum-builder` controla redundancias y cobertura del curso completo; `course-lesson-builder` controla narración y pantalla por clase; `course-slide-builder` controla organización visual y propósito pedagógico de cada diapositiva; `course-class-producer` coordina las puertas de calidad y no aprueba entregas incompletas.

## Portada frente a explicación: regla de diseño instruccional

- Una **diapositiva de portada** presenta la clase y admite solo una apertura narrada breve: tema, relevancia y ruta. **No desarrollar definiciones, fechas, marcos conceptuales ni explicaciones técnicas extensas sobre la portada**.
- Si la clase exige definir su tema, crear a continuación una diapositiva específica (por ejemplo: «¿Qué es NIST CSF 2.0?») con narración completa y texto visible derivado.
- La cantidad de diapositivas responde a las **funciones pedagógicas diferenciadas**, no a una cifra predeterminada ni a un punto por diapositiva. Se permite eliminar cierres redundantes y narrar la conclusión sobre la última diapositiva cuando resulte claro.
- Portada ≠ definición ≠ evolución ≠ propósito ≠ aplicación: cada unidad debe aportar información nueva y evitar repetición encubierta.
- Orden de producción: **puntos vigentes → narración completa → auditoría y corrección → texto en pantalla → storyboard → auditoría de redundancia → presentación editable y verificación visual**. No crear diapositivas antes de comprobar cobertura narrativa.

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

## Misión y alcance
Convertir **una clase concreta** del temario en contenido docente desarrollable y verificable. Las salidas iniciales obligatorias son **narración íntegra** y **propuesta de texto en pantalla derivada de esa narración**, ambas alineadas con todos los puntos curriculares. Arquitectura extensible para futuras salidas: diapositivas editables, demostraciones, actividades y materiales descargables.

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
3. **Cubrir exhaustivamente todos y cada uno de los puntos de contenido vigentes**, con profundidad adecuada para que la explicación se sostenga por sí misma. Un punto solo mencionado superficialmente no cuenta como cubierto.
4. Evitar temas futuros, redundancias con clases anteriores y ejemplos prematuros que creen confusión.
5. Introducir los conceptos antes de utilizar jerga no explicada. Mantener terminología consistente con el curso.
6. Diferenciar definiciones oficiales, interpretaciones pedagógicas, ejemplos hipotéticos y opiniones.
7. Si una práctica o demostración requiere pasos, describirlos con rigor y verificabilidad; no fingir ejecución.
8. No forzar ejemplos, analogías o historias cuando no mejoren la comprensión.
9. No inventar un tiempo exacto de narración: estimar con conteo de palabras y ritmo declarado, considerando pausas y demostraciones aparte.

## Contrato de cobertura y secuencia de producción (prioridad máxima)

**Orden obligatorio: Puntos del temario → Narración completa → Texto en pantalla.** Nunca comenzar seleccionando slides o redactando frases de pantalla para después acomodar la narración.

### 1. Cobertura exhaustiva de los puntos
- Obtener la lista completa de puntos de contenido de la clase desde el Google Sheets actualizado; preservar identificadores, matices y alcance.
- Construir una **matriz de cobertura**: ID y título de punto → objetivo/conceptos incluidos → segmento(s) de narración que los explican → estado.
- Cada punto debe quedar desarrollado, no solo nombrado o insinuado. Cuando un punto incluya varias dimensiones técnicas o pedagógicas, asegurar que cada una se explique.
- Si la profundidad necesaria supera la duración prevista, señalar el conflicto y proponer más tiempo o división aprobada; **nunca recortar puntos silenciosamente**.
- Antes de redactar el texto visible, auditar que la narración cubre el 100 % de los puntos verificables. Una omisión se considera crítica y debe corregirse.

### 2. Narración docente (contenido maestro)
Estructura editorial sugerida, adaptable a una clase teórica, práctica o mixta:
- Identificación de curso, sección, clase, versión y referencias.
- Objetivo de aprendizaje verificable.
- **Guion narrado completo**: introducción breve, desarrollo de cada punto, transiciones naturales y cierre proporcionado.
- Mapa de cobertura con pasajes identificables y fuentes.
- Duración aproximada calculada por palabras y ritmo declarado; agregar demostraciones por separado si existen.

La narración debe poder pronunciarse naturalmente: frases claras, ritmo oral, rigor técnico, sin listados recitados o conexiones artificiales. Evitar clichés como «En el mundo actual...» o «Es importante destacar...» y ejemplos forzados. Cada frase debe aportar valor.

### 3. Texto en pantalla (derivado, no fuente)
Una vez validada la narración, crear una propuesta de **texto en pantalla** por unidades visuales coherentes (no forzosamente una diapositiva por punto).
- Seleccionar definiciones, diferencias, secuencias, principios, conclusiones o términos que realmente ayudan a seguir la exposición.
- **Todo contenido semántico del texto en pantalla debe estar explicado íntegramente por la narración correspondiente**, ya sea literalmente o mediante una paráfrasis inequívoca y técnicamente equivalente.
- El texto visible puede ser más breve, esquemático o selectivo. **No es obligatorio que la narración completa aparezca en pantalla**.
- El texto visible **no puede introducir afirmaciones, ejemplos, cifras, requisitos, acrónimos, promesas, condiciones o matices que la narración no explique**. Tampoco debe cambiar el sentido mediante simplificación excesiva.
- La narración no tiene que repetir palabra por palabra el texto visible, pero debe explicar la idea completa y cualquier matiz relevante de ese texto.
- Evitar texto decorativo, párrafos extensos, listas redundantes, títulos vacíos y saturación. Mantener legibilidad móvil y jerarquía visual.
- Separar por unidad: `Título de pantalla`, `Texto visible`, `Segmento de narración asociado`, `Puntos curriculares cubiertos`. No crear todavía un archivo Slides si no se solicita.
- Una clase puede contener pasajes narrados sin texto visible equivalente; son válidos siempre que la narración cumpla el temario.

### Regla asimétrica explícita
**Texto en pantalla ⊆ contenido explicado por la narración.**

No se exige `narración ⊆ texto en pantalla`. La cobertura completa del temario se verifica **en la narración**, no contando viñetas visuales. Las dos obligaciones son independientes y acumulativas:
1. `Puntos de contenido ⊆ narración desarrollada`.
2. `Texto en pantalla ⊆ narración desarrollada`.

## Entregable conjunto
1. Guion narrado completo, organizado por segmentos y listo para revisión/grabación.
2. Propuesta de textos en pantalla, agrupada en unidades visuales e identificada por título, texto visible y segmento narrado correspondiente.
3. Matriz de cobertura por punto curricular y matriz de correspondencia de todas las frases y afirmaciones visibles con la narración.
4. Estimación de duración, fuentes y auditoría obligatoria.

## Generación y auditoría obligatoria
Flujo: leer el temario vigente → inventariar **todos** los puntos → verificar referencias → redactar narración completa → auditar exhaustivamente la cobertura narrativa → corregir omisiones → derivar el texto en pantalla → auditar toda correspondencia pantalla–narración → corregir → auditar el entregable final.

### Criterios de auditoría
1. **Cobertura íntegra (bloqueante):** cada punto curricular y sus componentes está explicado con profundidad suficiente, no solo mencionado.
2. **Precisión técnica y actualidad:** terminología, normas, versiones, cifras y afirmaciones verificadas.
3. **Profundidad:** explicación adecuada al nivel y al objetivo de la clase.
4. **Progresión pedagógica:** conceptos introducidos en orden comprensible y con prerrequisitos.
5. **Delimitación:** no repetir innecesariamente otras clases ni anticipar su contenido.
6. **Claridad:** exposición autónoma, precisa y con ejemplos cuando ayudan.
7. **Naturalidad oral / AI slop:** frases pronunciables, sin tono robótico ni muletillas.
8. **Coherencia:** continuidad, transiciones útiles y consistencia de ideas.
9. **Aplicación:** valor práctico sin demostraciones inventadas o ejemplos forzados.
10. **Duración y densidad:** estimación fundamentada, compatible con el alcance completo.
11. **Trazabilidad:** fuentes y límites de verificación identificados.
12. **Grababilidad:** segmentación y ritmo adecuados, sin recitar instrucciones editoriales.
13. **Correspondencia objetivo–desarrollo–cierre:** la explicación cumple la competencia prevista.
14. **Cobertura íntegra del texto visible por la narración (bloqueante):** cada afirmación, título, cifra, condición o matiz mostrado es explicado en la narración asociada, sin contradicción ni significados nuevos.
15. **Economía de texto en pantalla:** síntesis selectiva, legibilidad y jerarquía, sin obligación de reflejar toda la narración.

### Matrices de auditoría
- **Puntos → Narración:** ID de punto, componentes a explicar, identificadores de segmentos, evidencia breve, estado y observaciones.
- **Pantalla → Narración:** unidad visual, texto visible, segmentos narrados que lo explican, estado y observaciones.
- Para cada criterio: `Cumple`, `Requiere ajuste` o `No verificable`, evidencia, gravedad (**Crítica**, **Mayor**, **Menor**) y corrección aplicada o pendiente.
- Ningún punto sin explicación suficiente puede marcarse `Cumple`. Ningún texto visible con contenido nuevo o insuficientemente explicado puede aprobarse.
- Las auditorías del borrador y de la versión final son independientes. Si hay fuentes inaccesibles, comunicarlo sin fingir cobertura verificada ni asignar puntuaciones arbitrarias.

## Entrega y revisión
Entregar por defecto:
1. **Narración completa y editable**, desarrollada a partir de todos los puntos de contenido.
2. **Propuesta de texto en pantalla**, alineada por unidades visuales y segmentos narrados.
3. Matrices de cobertura y correspondencia.
4. Estimación razonada de duración, fuentes y **resumen de auditoría** con correcciones y pendientes.

Si se solicita únicamente narración, respetar ese alcance. Si se solicita un documento editable, generarlo sin alterar Google Sheets salvo pedido explícito. En revisiones, preservar elementos aprobados y auditar nuevamente el resultado.

## Evolución
La skill está dedicada al contenido de una clase. En futuras versiones podrá coordinar creación de diapositivas nativas, actividades y recursos descargables mediante habilidades específicas. La propuesta de texto en pantalla **ya es parte de la versión actual**, pero no implica generar Google Slides automáticamente.
