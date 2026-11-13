---
name: course-class-producer
description: Orquesta desde el nombre o ID de una clase la lectura de su temario vigente, narración auditada, planificación, gráficos y creación de Google Slides editables con narración en notas y auditoría integral.
---

# Course Class Producer — v0.1.0

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
