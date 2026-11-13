---
name: course-class-producer
description: Orquesta desde el nombre o ID de una clase la lectura de su temario vigente, narración auditada, planificación, gráficos y creación de Google Slides editables con narración en notas y auditoría integral.
---

# Course Class Producer — v0.1.0


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

## Excepción de portada y prioridad de recursos visuales (obligatorio)

- **Portada de clase:** prevalece la identidad visual maestra ya aprobada del curso (fondo, paleta, tipografía, layout y elemento gráfico protagonista). NO reemplazar automáticamente el gráfico de portada por el logotipo, la portada del documento o la figura oficial del tema específico tratado en esa clase. Solo variar título y componentes intercambiables previstos por la plantilla, sin rediseñarla.
- **Diapositiva de desarrollo con elemento específico:** priorizar recurso institucional/oficial verificable (p. ej., logo NIST, portada de publicación NIST CSF 2.0 o figura normativa auténtica), frente a escudos genéricos, íconos inventados o ilustraciones IA que pretendan representarlo. Conservar colores, proporciones y relaciones oficiales; atribuir su procedencia.
- **Diapositiva conceptual o de proceso:** utilizar iconos, diagramas nativos editables o ilustración cuando favorezca comprensión. No forzar una imagen oficial a una idea abstracta ni duplicar el mismo recurso institucional entre slides.
- **Puerta de calidad:** antes de aprobar, contrastar por separado (a) fidelidad de la portada a la identidad del curso, (b) autenticidad de cada recurso específico en desarrollo y (c) legibilidad, centrado de las composiciones dentro del área de contenido, paleta y correspondencia con la narración. La falta de imágenes pertinentes o una portada alterada sin autorización bloquea la aprobación visual.

## Sincronización obligatoria de narración en cada regeneración (bloqueante)

- Cada vez que se regenere, optimice o modifique una clase o cualquiera de sus diapositivas, revisar y sincronizar **todas las notas del presentador afectadas** con la versión vigente y aprobada de la narración, incluso cuando el cambio principal sea visual.
- Para cada diapositiva, efectuar **sustitución completa del contenido del cuadro de notas** (`deleteText ALL` y luego `insertText` con el segmento vigente) en vez de insertar al final de notas preexistentes. Prohibido `insertText` a secas sobre notas ya pobladas: provoca concatenaciones, duplicados y residuos de versiones anteriores.
- Usar una única fuente maestra de narración, con IDs estables, asignación uno a uno a cada slide y trazabilidad de los puntos curriculares. No copiar un fragmento común en múltiples diapositivas ni reintroducir una narración anterior.
- Al terminar, **releer en vivo las notas de todas las diapositivas**; comparar literalmente con los segmentos aprobados, revisar orden, integridad, ausencia de duplicados, encabezados técnicos sobrantes y correspondencia con la pantalla.
- Una discrepancia, nota sin actualizar o imposibilidad de verificar lectura de vuelta es un **bloqueo de aprobación**. Reportar el estado real y no declarar la presentación terminada ni la narración sincronizada mientras persista.
- No modificar el diseño manual del usuario para resolver un defecto exclusivamente narrativo. Preservar los objetos y posiciones de Google Slides salvo que el usuario haya pedido edición visual.

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
Ejecutar de principio a fin la producción de **una clase existente** a partir del nombre o identificador dentro de un curso conocido. Es una **skill orquestadora**: delega el trabajo especializado en otras skills y comprueba los contratos entre etapas; no sustituye los procedimientos de cada módulo.

**Salida objetivo:** Google Slides 16:9 editable, texto en pantalla, gráficos pertinentes, narración completa segmentada en notas del presentador, matrices de correspondencia y auditoría final.

## Entrada mínima
- Nombre o ID identificable de una clase **en el contexto del curso actual**.
- Resolver automáticamente el Google Sheets del curso y su última versión accesible; preferir un enlace ya proporcionado en la conversación, una referencia de configuración del proyecto o búsqueda de los archivos del curso. Si existen varias clases coincidentes sin forma de distinguirlas, solicitar una identificación mínima.
- Una clase nueva fuera de temario requiere primero actualización curricular aprobada; no inventar puntos ni reemplazar clases.

**No volver a pedir** título, referencia oficial, paleta o plantilla que ya estén disponibles y aprobadas. No pedir preferencias opcionales por rutina.

## Fuentes de verdad y dependencias
1. **Google Sheets vigente**, `Temario` + `Puntos de contenido` (+ `Matriz de cobertura`, `Auditoría` si existen). Ediciones del usuario tienen precedencia sobre copias antiguas del temario.
2. Referencias técnicas vigentes y obligatorias; distinguir documentación oficial de ampliaciones docentes.
3. `course-slide-template` **aprobado**, con URL nativa y versión.
4. `course-image-style.md` **aprobado** del curso, cuando se necesiten ilustraciones generadas.
5. `course-lesson-builder` para narración íntegra y textos de pantalla.
6. `course-slide-builder` para planificar, producir y verificar el deck.

`course-curriculum-builder` no se vuelve a ejecutar automáticamente para generar una sola clase. Si el temario no existe, señalar esa dependencia; si falta aprobación del template o estilo, trabajar la fase que sí sea posible, sin inventar aprobaciones.

## Procedimiento orquestado (con puertas de control)
### Paso 0 — Resolver la clase
- Leer Google Sheets **en vivo** y localizar la coincidencia por ID/título exacto; capturar sección, título, todos los puntos, fuentes y títulos vecinos.
- Registrar URL, IDs de fila/punto, versión disponible y cualquier ambigüedad.
- Nunca usar de manera silenciosa una lista vieja de puntos almacenada en memoria si hay una hoja actualizada accesible.

### Paso 1 — Narración y pantalla (`course-lesson-builder`)
- Verificar fuentes relevantes y alcance de cada punto.
- Producir narración completa; segmentar con IDs estables N01...Nxx.
- Verificar que **cada punto curricular esté explicado con suficiente profundidad**. Resolver todas las omisiones críticas antes de continuar.
- Derivar texto en pantalla desde la narración, no al revés. Verificar que cada afirmación visible está explicada.
- Documentar cambios de contenido requeridos antes de tocar la hoja fuente; no sobrescribir ediciones del usuario.

### Paso 2 — Resolver el sistema gráfico del curso
- Leer la paleta, tipografía y dos layouts aprobados desde `course-slide-template`.
- Leer estilo maestro aprobado desde `course-image-style-builder`.
- **Esos parámetros se definen una vez por curso**, no se regeneran cada clase.
- Si faltan aprobaciones: proponerlas mediante el módulo correspondiente y detener únicamente las tareas que dependan de ellas. No simular que el deck final quedó listo.

### Paso 3 — Storyboard (`course-slide-builder`)
- Dividir la narración en unidades visuales; no forzar un slide por punto curricular.
- Asignar IDs de puntos, segmentos narrados, texto en pantalla, propósito gráfico y tipo de asset a cada slide.
- Conservar cobertura completa del guion, incluida introducción y cierre si se narran.
- Auditar plan semántico antes de generar los gráficos o construir el deck.

### Paso 4 — Gráficos y construcción
- Utilizar **activos oficiales** para figuras normativas cuya precisión o integridad importe.
- Generar ilustraciones solo donde aporten comprensión, bajo el prompt maestro aprobado; preservar assets individuales para insertar en diapositivas.
- Copiar el deck plantilla aprobado y construir el Google Slides editable.
- Insertar narración íntegra en notas de cada slide, cuando la API/conector lo permita; verificar mediante lectura de vuelta. Si no es posible, informar salida parcial y entregar transcripción externa segmentada, **no afirmar inserción**.
- Audio real, voz sintetizada y sincronización son capacidades adicionales independientes, no implicadas por la palabra «narración» cuando se entrega como notas.

### Paso 5 — Auditoría integral y entrega
- Releer los puntos actuales para evitar pérdida de cobertura por cambios durante producción.
- Auditar las relaciones: `Puntos ⊆ Narración`, `Pantalla ⊆ Narración`, `Cada slide ↔ su(s) segmento(s) narrados`, `Gráfico ↔ concepto/narración`.
- Auditar legibilidad, utilidad didáctica, edición nativa, estilo, plantillas, origen de assets, precisión y redundancias.
- Revisar visualmente **todas** las slides entregadas, no solo portada y muestra.
- Entregar enlace verificado de Google Slides + plan por slide + fuentes y resumen de auditoría + límites técnicos. No declarar éxito total ante un bloqueo crítico.

## Recuperación y reanudación
- Guardar un manifiesto del trabajo por clase conforme a `references/run-manifest.md`, con artefactos y estados por fase.
- En revisiones, comparar versiones y retomar desde el punto afectado. No regenerar los pasos aprobados sin necesidad.
- Si se modifica el Google Sheets durante la producción, detectar IDs o puntos distintos y revalidar la narración afectada; no sobrescribir contenido.
- Cambios permanentes en instrucciones pasan por `course-skill-improver`, siempre con aprobación.

## Auditoría de orquestación
1. Identificación inequívoca de la clase correcta.
2. Lectura del temario vigente y puntos completos.
3. Uso de referencias técnicas correctas.
4. Cobertura completa de los puntos por la narración (crítico).
5. Explicación de cada texto visible por su segmento de narración (crítico).
6. Asignación completa y ordenada de narración a slides/notas (crítico para entrega con narración).
7. Reutilización efectiva de plantilla, paleta y estilo **aprobados**.
8. Gráficos técnicamente fieles y didácticamente pertinentes.
9. Legibilidad, consistencia visual y editable nativo.
10. Preservación de archivos fuente y cambios del usuario.
11. Verificación real de Google Slides, notas y render.
12. Transparencia sobre dependencias, limitaciones y pendientes.
13. Redundancia y naturalidad docente.
14. Trazabilidad por IDs y versiones, auditoría reproducible.

Cada criterio tendrá `Cumple / Requiere ajuste / No verificable` con evidencia y severidad. Un fallo crítico impide declarar `Producción completa`.

## Semántica de estados
- `No iniciada`: dependencia no disponible.
- `En curso`: trabajo parcial comprobable.
- `Pendiente de aprobación`: decisión de estilo o contenido requerida.
- `Bloqueada`: limitación de herramienta, fuente o integridad.
- `Terminada y verificada`: entregable real inspeccionado y sin fallos críticos.

No realizar promesas de actividad en segundo plano. Ejecutar lo viable en el turno actual y describir solo lo realmente producido. Si el usuario pide solo construir estas instrucciones, publicarlas en GitHub y **no empezar automáticamente a producir una clase real**.

## Relación entre skills
`course-curriculum-builder` (prepara fuente inicial en Sheets) → `course-lesson-builder` (narración completa + pantalla) → `course-slide-builder` (storyboard + assets + deck + notas); en paralelo, una sola vez por curso, `course-slide-template` y `course-image-style-builder`. `course-class-producer` coordina, valida y entrega. `course-skill-improver` gestiona mejoras permanentes.
