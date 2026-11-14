# Reglas editoriales y maquetas SVG — aprendizaje de la clase 4.4 (2026-11-14)

## Aprendizaje adicional: imagen oficial también en panorámica (2026-11-14)

La apertura de la clase 4.4 no usa tres números circulares; contiene tres **imágenes institucionales pequeñas** de Núcleo, Perfiles Organizacionales y Niveles (Tiers), con nombre y finalidad breve. El criterio institucional vale para introducciones y desarrollos: no relegar figuras NIST a las slides posteriores. Verificar de forma individual cada activo y su legibilidad a escala reducida; hacer recorte fiel cuando proceda, respetar proporciones/colores y no simular autenticidad con SVG. La portada conserva su propia gráfica. En `proposals/class-4.4-componentes-del-marco-v4.md` está la propuesta actualizada y todavía no aprobada. Añadir regresión **OFF-01**: apertura de tres componentes sustituye las imágenes disponibles por iconos/números → fallo. **OFF-02**: tres imágenes oficiales pero una ilegible o estirada → fallo. **OFF-03**: portada pierde gráfica aprobada al forzar rueda oficial → fallo.

## Precedencia y alcance
Referencia operativa para `course-curriculum-builder`, `course-lesson-builder`, `course-slide-builder`, `course-class-producer`, `course-slide-template` y `course-skill-improver`. Complementa `references/visual-composition.md` y el flujo de aprobaciones de `SKILL.md`. **No** autoriza editar por sí sola Google Sheets ni Google Slides. Las particularidades de 4.4 son un caso de prueba, no una plantilla universal.

## 1. Redundancia: repetición no equivale a defecto
1. Separar **repetición léxica** (mismas palabras), **conceptual** (misma explicación sin aporte), **pedagógica funcional** (panorama → desarrollo → aplicación) e **interclases** (repetir material reservado a otra clase).
2. **Una apertura panorámica breve puede indicar qué es cada componente y para qué sirve, aunque las diapositivas siguientes lo expliquen individualmente.** No penalizarla automáticamente: orienta al estudiante y establece un mapa mental. La repetición es legítima si cambia la función y la profundidad.
3. Penalizar únicamente si el segundo bloque vuelve a desarrollar **prácticamente la misma definición, enumeración, ejemplo o beneficio** sin agregar profundidad, contraste o una perspectiva nueva. Mostrar el pasaje exacto y la diferencia de función antes de proponer suprimirlo.
4. La intro no necesita ser una lista de nombres carente de significado. Tampoco debe robar el detalle de secciones específicas.
5. No revisar puntuaciones arbitrariamente: la auditoría independiente **Ausencia de redundancia (1–10, decimal)** requiere evidencia concreta, ámbito intra/interclases y justificación. Cambiar una nota previa implica explicar por qué cambió la interpretación. Evitar notas complacientes.
6. Una transición o recordatorio de «lo veremos después» puede servir una sola vez por clase; múltiples recordatorios sin función se condensan.
7. El material de orientación, conceptualización, práctica y evaluación puede referirse al mismo objeto **sin redundancia perjudicial** cuando persiguen aprendizajes distintos.

### Caso concreto 4.4 — «Componentes del Marco»
- Duración orientativa: **3–5 min**, panorámica. Tres componentes: **Núcleo (Core), Perfiles Organizacionales, Niveles (Tiers)**.
- Apertura: presentar y dar la **finalidad resumida** de los tres; los desarrollos siguientes amplían brevemente cada uno. No suprimir esos propósitos de la apertura por criterio mecánico de redundancia.
- Núcleo: mencionar funciones/categorías/subcategorías, **enumerar** Gobernar, Identificar, Proteger, Detectar, Responder, Recuperar, **sin explicar las seis** (clase 4.5). Categorías/subcategorías sin códigos ni ejemplos detallados (clase 4.6).
- Perfiles/Tiers: finalidad general; no convertir la panorámica en lección sobre tipos, niveles individuales, cinco pasos, brechas ni implementación (clase 4.7 y posteriores).
- Relación de los componentes: una síntesis al final puede ser válida como integración, pero evitar repetir literalmente el texto de la apertura.
- **Estado de 4.4:** todavía no aprobada ni grabada. Conservar identificadores vigentes 4.4.1 y 4.4.2 hasta que se autorice una revisión curricular; la propuesta de tres puntos del chat no es modificación aprobada del Sheet.
- La estructura provisional de cinco slides **no es un número obligatorio ni una aprobación**. Ajustar según guion auditado.

## 2. Maquetas SVG visibles: puerta editorial entre narración y Slides
1. Orden: `puntos vigentes → narración completa → auditoría editorial → texto visible → storyboard con función y geometría → maqueta(s) SVG 16:9 visible(s) → optimización/auditoría → aprobación explícita → construcción nativa en Google Slides → QA`.
2. Mostrar la **vista previa de cada maqueta SVG en la conversación** antes de solicitar aprobación. Usar una vista conjunta o un selector por diapositiva cuando sirva para revisar distribución. No basta con describir un SVG ni mostrar código sin vista previa si la interfaz permite renderizarlo.
3. La maqueta representa **composición**, no figura institucional ni entregable final: simular posición y ocupación de imagen oficial con un marcador inequívoco; no dibujar una falsa rueda/figura/plantilla NIST que pueda parecer una reproducción oficial.
4. Antes de diseñar: verificar de forma **nativa** master/layouts del deck maestro, portada aprobada, proporción, tipografía, posiciones, geometría, paleta y referencias reales. La solicitud de una miniatura **no** prueba inspección de sus píxeles. Declarar qué se inspeccionó estructuralmente y qué queda pendiente visualmente.
5. En recursos **específicos y reconocibles** (NIST, Núcleo, perfiles, tiers), usar diagramas/documentos/capturas **auténticos verificables**; proteger escala, recorte, nitidez, etiquetas, atribución y paleta original. No convertir el recurso oficial en una «versión IA». Si la figura presenta demasiado detalle para una clase introductoria, usar otra imagen oficial verdaderamente pertinente o posponerla.
6. Una figura oficial de **procedimiento** (p. ej., los cinco pasos para crear/usar Perfiles) **no equivale** a la representación de la naturaleza de ese componente; no usarla como figura principal si el guion no explica el procedimiento.
7. A cada maqueta exigir: idea didáctica, función de cada objeto, texto exacto, segmento de notas, tipo/fuente de recurso, área segura y márgenes, escala/proporción, jerarquía, contraste, centrado óptico y lectura en formato 16:9. Evitar contenido decorativo y sobrecarga.
8. La aprobación de la **narración/storyboard/maquetas** es una autorización editorial para construir **esa propuesta concreta**, no prueba de que la diapositiva final esté visualmente aprobada. Una vez publicada en Slides, inspección estructural + visual real y aceptación explícita del usuario antes de activar `Aprobada` en Sheets.
9. **Plantilla maestra inmutable**, presentación acumulativa como destino; conservar diapositivas ya aprobadas. No generar PDFs/PPTXs salvo pedido.

## 3. Sincronización de la fuente de verdad y estados
- `PROJECT_STATE.md` es el punto de reanudación, no reemplaza lecturas en vivo. Google Sheets tiene `Temario`, `Puntos de contenido`, `Matriz de cobertura`; preservar IDs y trazabilidad.
- Una petición de cambiar un título/punto del temario exige confirmar el cambio en la hoja y matriz de cobertura **mediante lectura de vuelta**; no declarar «actualizado» si solo se propuso en el chat. La ejecución de cambios necesita autorización por la petición o aprobación del usuario.
- `Aprobada` significa **diapositivas producidas y aprobación final confirmada por el usuario**, no storyboard presentado; `Grabada` significa grabación confirmada. Son independientes.
- Anotar todo pendiente no verificado (fidelidad de activos, render, notas, prueba de regresión) sin presentarlo como prueba superada.

## 4. Casos de regresión a ejecutar (no equivalen a pruebas superadas)
- **RED-01**: panorama «Núcleo/Perfiles/Niveles y finalidad breve» seguido de ampliación. Resultado esperado: repetición **funcional permitida**, no penalización automática.
- **RED-02**: apertura y desarrollo con la misma definición desarrollada y ejemplos literales. Resultado: solapamiento material, propuesta de corrección.
- **RED-03**: 4.4 intenta enseñar seis funciones, códigos o cuatro niveles individualmente. Resultado: anticipación interclases detectada, preservar carácter panorámico.
- **SVG-01**: propuesta con guion y puntos pero sin vistas previas visibles. Resultado: incompleta la puerta editorial visual, no construir.
- **SVG-02**: maqueta sustituye rueda NIST auténtica por pseudofigura. Resultado: sustituir marcador por activo oficial verificable antes de producción.
- **SVG-03**: figura oficial de cinco pasos en una diapositiva que no los explica. Resultado: rechazo por relación recurso–narración, selección de imagen pertinente.
- **STATE-01**: clase con diapositivas existentes pero no aprobación final. Resultado: `Aprobada=false`; `Grabada=false` salvo confirmación.
- **STATE-02**: resumen de conversación discrepa de Sheet. Resultado: reportar diferencia, conservar IDs y no afirmar sincronización inexistente.

**Estado:** son pruebas **definidas**; cualquier ejecución necesita evidencia y registro del resultado. No declararlas «aprobadas» solo por escribir las reglas.
