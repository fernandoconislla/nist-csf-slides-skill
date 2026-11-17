---
name: course-class-producer
description: Orquesta desde el nombre o ID de una clase la lectura de su temario vigente, narración auditada, planificación, gráficos y creación de Google Slides editables con narración en notas y auditoría integral.
---

# Course Class Producer — v0.1.0

## Control de figuras oficiales pequeñas en aperturas (2026-11-14)

No basta con verificar que las slides de desarrollo tengan gráficos NIST: auditar **también** la panorámica de componentes. Si existe una representación institucional pertinente de Núcleo, Perfiles y Tiers, exigir las **tres imágenes auténticas pequeñas** en la slide 02 de la clase 4.4, sin reemplazarlas por círculos con números. Comprobar fuente, recorte, proporción, legibilidad y correspondencia con el guion antes de aceptar maquetas SVG y antes de escribir Slides. Revisar `../../proposals/class-4.4-componentes-del-marco-v4.md`; la corrección editorial no supone aceptación visual final.

## Puerta SVG y estados de aprobación (2026-11-14)

Orquestar `../../references/editorial-redundancy-svg.md`: narración completa auditada → pantalla → storyboard → **maquetas SVG visibles** → optimización editorial → aprobación explícita → construcción nativa → QA estructural/visual → aprobación final del usuario. La introducción panorámica puede resumir propósitos antes de desarrollarlos, sin considerarse redundancia automática. Registrar estado y limitaciones verificadas. Marcar `Aprobada` en Sheets solo tras confirmación final de diapositivas producidas; `Grabada` solo tras confirmación de grabación.


## Puertas de producción de composición visual (obligatorias)

Exigir a `course-lesson-builder` y `course-slide-builder` el contrato de `references/visual-composition.md`: **Puerta A preventiva** (storyboard auditado, economía visual, balance, geometría); **Puerta B de construcción** (objeto editado vs plan, transformaciones, alineación, reequilibrio); **Puerta C final** (QA estructural, inspección visual real y regresión). Rechazar transición a «Terminada y verificada» si falta una puerta o la inspección renderizada no es posible. Preservar aprobación editorial previa al primer cambio del deck. Correcciones autorizadas sobre diapositivas existentes no permiten alteración silenciosa de guiones ni slides ajenas.

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

## Flujo obligatorio de propuesta, aprobación y presentación acumulativa (2026-11-13)

**Regla de precedencia:** esta secuencia prevalece sobre cualquier instrucción anterior que autorice generar Google Slides directamente al recibir «genera la clase». La aprobación de una clase anterior NO autoriza producir automáticamente la siguiente.

**Fase A — propuesta editorial, sin escribir diapositivas:** identificar la clase y sus puntos vigentes en Google Sheets; preparar narración COMPLETA por diapositiva, texto EN PANTALLA y especificación gráfica/layout de cada diapositiva; explicar la cobertura y los límites respecto a clases vecinas; optimizar y auditar la propuesta; **presentarla al usuario para revisión**. Sin aprobación explícita, no crear, copiar, añadir, eliminar ni modificar diapositivas en Google Slides. Si hay ajustes, regenerar la propuesta hasta su aprobación. El texto «genera ahora [clase]» solicita inicialmente esta propuesta, no la construcción del archivo, salvo que la autorización de ejecución esté ya expresamente concedida para esa propuesta.

**Fase B — construcción tras aprobación:** una vez que el usuario **apruebe la propuesta concreta**, construir las nuevas diapositivas de esa clase **dentro de la presentación acumulativa del curso ya existente**, AL FINAL y en el orden aprobado, sin abrir una presentación por clase ni sustituir la anterior. Usar la plantilla/identidad como referencia de estilos, y la presentación acumulativa como destino de edición. Conservar intactas todas las clases aprobadas anteriores y el archivo maestro de plantilla. No confundir «plantilla maestra» (fuente inmutable) con «presentación acumulativa» (destino editable).

**Fase C — control y aprobación visual:** sincronizar y releer notas del presentador íntegramente, verificar todas las diapositivas recién incorporadas en su contexto dentro del deck acumulativo, ejecutar auditoría de regresión y mostrar al usuario el enlace a la presentación actualizada. Las correcciones de producción sobre una propuesta aprobada se auditan y presentan para aceptación visual, sin alterar otras clases.

**Archivo acumulativo actual de NIST CSF 2.0:** `https://docs.google.com/presentation/d/1h8BqC56ud8_4xKm_Aco9V-XcMdfVlaLwNedodUMgOvE/edit` contiene la clase 4.1 aprobada y es el destino para añadir 4.2 y las posteriores al aprobarlas. **No utilizar** la copia separada no aprobada de 4.2 (`1WKV9iJHHn1E47Ubn9c6-GRBa-Zbx1gcHIVIrCo_ydJQ`) como nueva fuente de verdad ni agregarla sin revisión y autorización.

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

## Recuperación de ejecución y QA del foco (2026-11-14)
- El orquestador no transforma «hazlo» o «corrige» en una propuesta futura; intenta realmente la escritura autorizada. **Primero detectar conector disponible y lectura de estado.** Ante error: hasta tres enfoques técnicos distintos seguros, comprobar cambios parciales y revisión antes de reintentar, no duplicar slides/assets.
- Escalera: corregir JSON/campos → partir batch o cambiar método nativo → usar activo local original y otra vía compatible; detener solo ante bloqueo comprobado o riesgo de integridad. Registrar razones y evidencias.
- Incluir en auditoría `Fuerza del foco visual` con evidencia de imágenes renderizadas, junto a `Ausencia de redundancia`. Un marco técnicamente existente, pero visualmente débil, **NO** supera auditoría.
- Mantener aprobaciones separadas: generado ≠ auditado ≠ aprobado ≠ grabado. Releer deck y notas, hacer render, registrar IDs exactos y no alterar clases aprobadas.

## Cierre integral tras aprobación 4.7 — 2026-11-14
- «Aprobado»: localizar fila exacta por ID en Sheets, revisar validación, actualizar solo Aprobada=TRUE, conservar Grabada, releer. No inferir estados de otras clases desde memorias.
- «Actualiza skills con pendientes»: revisar raíz, productor, lecciones, builder, estilo, plantilla, temario, improver, referencias, tests, estado y changelog; deduplicar reglas ya adoptadas y verificar lecturas de GitHub.
- Prioridad: fidelidad del original > legibilidad > foco correctamente localizado > estética. «Fidelidad» no significa insertar texto del PDF como imagen protagonista cuando un diagrama pedagógico representa mejor la relación, indicando su fuente.
- Al aprobar una clase editada, conservar la presentación como fue aceptada; sincronizar estado sin alterar slides por iniciativa propia. Si falla una operación, inspeccionar cambios parciales antes de reintentar.

## Cierre transaccional por aprobación expresa de clase — 2026-11-14

**Disparador:** «aprobado», «esta clase está aprobada» o equivalente referido inequívocamente a la clase activa. La aprobación permite actualizar su **estado**, no cambiar el contenido ni crear la siguiente clase.

1. **Resolver identidad:** consultar el contexto y la hoja `Temario` viva, confirmar código, título y **fila exacta**, y validar estado anterior de G/H; no usar filas memorizadas sin comprobación.
2. **Sincronizar Sheets:** establecer **solo la casilla `Aprobada` (G) en TRUE**, de ser necesario; no alterar `Grabada` (H), estado editorial, formato, otras clases, notas ni títulos. Leer de vuelta C:H (o rango equivalente) y comprobar identidad y ambos booleanos. Si ya es TRUE, no duplicar escritura.
3. **Sincronizar GitHub:** leer `PROJECT_STATE.md` y su SHA vigente; incorporar un registro de cierre fechado que señale clase, título, IDs/rango de slides, revisión del deck verificada, `Aprobada`, `Grabada`, clase siguiente y pendientes reales. Guardar con control de SHA y **releer** el archivo para comprobar la versión resultante. Evitar registrar como auditado aquello no comprobado.
4. **Control del curso:** informar los dos resultados por separado, las discrepancias y lo que falta. Ante error en una fuente, comprobar primero si hubo escritura parcial; reintentar con seguridad, sin sobrescribir cambios concurrentes. **No declarar sincronización completa** si Sheets o GitHub siguen sin confirmar.
5. **Preservación:** la aprobación protege las diapositivas tal como fueron aceptadas; la grabación solo cambia por confirmación explícita. No iniciar la clase siguiente hasta que el usuario lo pida.

**Caso de aprendizaje 5.1, slides 19 y 42:** antes de trasladar un foco visual de una slide referente a otra, contrastar las **imágenes base** y sus dimensiones/proporciones; si son distintas, primero asegurar equivalencia de base y ajustar foco mediante coordenadas relativas a ella, no exclusivamente a la página. Inspeccionar miniatura/render actualizado y diferenciar lectura estructural de prueba visual real. Prohibido afirmar alineación visual verificada por haber calculado coordenadas únicamente.

## Regresión de alineación y auditoría entre diapositivas (2026-11-15)
Ante una observación de texto descentrado, encargar al `course-slide-builder` la auditoría exhaustiva **de todas las diapositivas de la clase activa**: emparejar cada rótulo con su contenedor, calcular `Δx/Δy` con tamaño y transformación efectivos, distinguir rótulos independientes de bloques de varias jerarquías, corregir el error sin rediseñar ni afectar notas, releer resultados y pasar inspección renderizada. El hecho de aplicar `contentAlignment=MIDDLE` y `paragraphStyle.alignment=CENTER` no acredita centrado geométrico; solicitar datos de centros antes/después. No extender correcciones a clases ya aprobadas fuera del alcance. Caso de referencia: 5.2, slides 46 y 49, desfases verticales de -3,49 y +4,01 unidades de diseño corregidos hasta `Δy=0` por lectura nativa; QA óptico de render se informa por separado.

## Precedente visual de clase 5.2 y protección de decisiones manuales (2026-11-15)
- Una modificación manual posterior del usuario en la diapositiva nativa se convierte en **base de trabajo actual**. Antes de «corregir» o regenerar, releer la slide viva y no restaurar barras, títulos, contenedores o énfasis que el usuario haya retirado. Distinguir corrección puntual de rediseño.
- Auditar la secuencia didáctica como jerarquía real: portada → categoría GV.OC panorámica → cinco subcategorías GV.OC-01 a -05. El cuadro de categoría de la panorámica tiene mayor peso visual (amarillo suave + borde grueso); los códigos subordinados comparten fondo blanco y borde amarillo. La plantilla de las cinco slides individuales sigue homogénea.
- La auditoría de salida incluye revisión **diapositiva por diapositiva** de margen efectivo de texto, desbordamientos por wrapping, centrado de etiquetas, conectores anclados, semántica de las relaciones, paleta funcional NIST, notas y estado de aprobación. Identificar por separado hallazgos demostrados mediante API frente a hipótesis sin render.
- Registro de la última corrección de 5.2: slides 45 (márgenes), 47 (líneas), 48 (inclusión) y 50 (dos conectores nativos). Se confirmó persistencia y conservación de notas mediante lectura nativa; **la verificación visual a partir de render quedó pendiente**. No convertir esa persistencia técnica en aprobación de la clase.

## Puertas obligatorias de diseño, construcción y auditoría de calidad — 2026-11-15
Para **todos los criterios visuales y pedagógicos refinados** aplicar una triple comprobación independiente:
- **Puerta 1, antes de construir:** inspección de la última presentación (incluidas modificaciones manuales), precisión NIST y diseño integral de cada slide: identidad, jerarquía, redundancia, legibilidad, distancias, conectores, centros locales y posición del conjunto en relación con el resto de la slide; anticipar wrapping y simetría. No pasar una maqueta que ya contiene un problema previsible.
- **Puerta 2, al construir:** ejecutar restricciones del storyboard y recalcular sus invariantes después de cada cambio. Una modificación a cuadro, flecha, texto o nodo exige revisión inmediata de elementos dependientes y composición completa; preservar notas, plantilla, clases previas e IDs; verificar Google Slides mediante lectura de vuelta.
- **Puerta 3, al auditar:** contrastar diseño propuesto vs implementación y render real en tres escalas (local, diagrama, diapositiva) y entre todas las diapositivas de clase. Evaluar fuente, semántica, jerarquía, color, balance, simetría, igual longitud de líneas cuando corresponde, puntos de enlace, texto no dividido, márgenes, ritmo, precisión, redundancia y notas. Hallazgos con evidencia, gravedad y ajuste aplicado; auditoría de regresión tras corrección.

**Caso regresivo GV.OC-02:** usuario detectó desde captura que las líneas superior e inferior tenían longitudes 27 y 45, aunque la geometría de cada caja era consistente. El caso muestra que una auditoría de centrado texto/caja es insuficiente: PLANEAR simetría de conectores, IMPLEMENTAR medidas iguales, AUDITAR distancias y diagrama completo. Corregido por desplazamiento de bloque ORGANIZACIÓN de 9 unidades y líneas de 36 unidades. **Caso GV.OC-05:** diagrama aislado coherente, pero inicialmente desalineado respecto al cuadro izquierdo; centrar globalmente el conjunto sin romper relaciones internas.

Cada clase debe incluir una **matriz de cumplimiento por criterio** que registre estado de las tres puertas (propuesto, comprobado en API, comprobado en render). Ausencia de render no permite aprobar visualmente. La aprobación editorial/grabación siguen siendo decisiones expresas del usuario.

## Auditoría dual obligatoria en clases y propuestas — 2026-11-16
Incluir en cada storyboard/maqueta SVG y cada slide construida una **auditoría de representación conceptual individual** (todos los símbolos, relaciones, flechas; concepto, lectura sin etiqueta, ambigüedad, nota decimal 0–10 y mejora) independiente de la **auditoría visual/general** (precisión NIST, calidad, geometría, composición, jerarquía, legibilidad, consistencia, pedagogía y ausencia de redundancia). Mostrar ambos promedios; objetivo conceptual ≥9,0 y ningún icono principal <8,5. Ante fracaso: NO APROBADO y propuesta de corrección.
Separar propuesta aprobada, implementación estructural, render visual inspeccionado y aprobación final del usuario. La persistencia en Slides, PDF exportado o un thumbnail disponible no son evidencia de QA visual si la imagen no se examinó. Corregir regresiones sin reabrir innecesariamente slides aprobadas.
Regresiones de referencia: slides 46–48 aprobadas; slide 49 Capacidades se mantiene como cuadrado con check por preferencia explícita, y los rótulos Objetivos/Capacidades/Servicios críticos requieren centrado vertical homogéneo. Orientación de flujo GV.OC-04 (servicios que la organización da/que terceros esperan) opuesta a GV.OC-05 (dependencias de la organización). Aplicar en todas las clases las dos auditorías sin que el usuario deba recordarlo.

## Patrón gráfico aprobado — foco único y flechas a cajas breves (2026-11-16)
Regla para diapositivas conceptuales con UN objeto central y varias acciones o relaciones: usar un solo gráfico protagonista inequívocamente identificado, con flechas nativas que parten de él hacia cajas de texto corto (verbo y complemento conciso). El gráfico debe hacer explícito QUÉ se caracteriza o gestiona; evitar lupa, estrella, check, documento o tendencia ascendente genéricos si no transmiten la identidad del objeto. Evitar párrafos, ejemplos y adornos en las cajas; desarrollar el significado en la narración. Las flechas representan relaciones reales, no secuencia temporal, aprobación ni causalidad inventadas. Alinear simétricamente ramas, conectores y cajas, con márgenes suficientes, sin clipping, y balancear el conjunto frente a la columna NIST izquierda. Mantener Inter, paleta del curso, figuras oficiales intactas y objetos editables.
Referencia editorial aprobada: GV.RM-07, diapositiva 59: protagonista «OPORTUNIDAD ESTRATÉGICA», ramas «CARACTERIZAR — Beneficios y condiciones» e «INCLUIR — En la discusión de riesgos». La regla es preferente SOLO cuando la semántica lo justifica: no sustituye figuras oficiales NIST, jerarquías, cronologías, comparaciones u otros gráficos que requieran relaciones diferentes.
Puertas obligatorias: (1) planificar foco, etiquetas, sentido semántico de flechas y simetría; (2) implementar con objetos y conexiones nativas, conservar texto oficial y notas; (3) auditar cada símbolo/relación y la composición, texto, desbordes y render real observado. Las dos auditorías independientes siguen obligatorias. Aprobación de propuesta no equivale a aprobación de la slide o de la clase.

## Orquestación obligatoria de auditorías sin omisiones (2026-11-16)
La puerta de publicación de cada propuesta, slide y clase requiere inventario C01–C17 de `../../references/visual-composition.md` con evidencias por fase. Encargar auditoría doble al builder y **comprobar cobertura**, no asumirla por mención del promedio. Al pedir el usuario «genera», «corrige», «optimiza» o «audita», ejecutar preventivamente las verificaciones aplicables; después de cualquier mutación de Slides repetir post-render y regresión antes de anunciar resultado. Si el usuario señala un fallo puntual, corregirlo y auditar de nuevo todas las dependencias de la slide, no solo el objeto editado. Bloquear entrega/aprobación técnica si existe símbolo sin reconocimiento de silueta, conexión incorrecta, falta de render visual realmente observado o cualquier criterio aplicable sin evidencia. Preservar el estado de aprobación en Sheets y cambios manuales. Reportar claramente PASS/FAIL/BLOCKED y acciones pendientes; aprobación editorial ≠ auditoría técnica ≠ aprobación explícita de clase.
