---
name: course-slide-builder
description: Transforma una narración docente completa y auditada, textos en pantalla y un sistema visual aprobado en una presentación Google Slides 16:9 editable, con gráficos y narración íntegra distribuida en notas del presentador.
---

# Course Slide Builder — v0.1.0


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
Planificar, construir y verificar **las diapositivas terminadas de una clase** a partir de su narración ya elaborada. Entregar Google Slides nativo editable, con texto en pantalla, recursos gráficos, y **el guion de narración correspondiente a cada diapositiva dentro de las notas del presentador**. No confundir notas con una pista de audio embebida; audio/TTS/sincronización es una fase opcional separada y requiere herramientas compatibles.

## Dependencias y entradas
- Obligatoria: clase inequívoca, identificadores y **narración completa auditada** de `course-lesson-builder`, con sus segmentos y puntos curriculares.
- Obligatoria para construir el deck final: **plantilla Google Slides aprobada** de `course-slide-template` (URL, versión y estructura) y, si se necesitan ilustraciones generadas, **`course-image-style.md` aprobado** de `course-image-style-builder`.
- Textos en pantalla propuestos, matriz Puntos→Narración y matriz Pantalla→Narración, fuentes y limitaciones.
- Opcionales: orden y rango objetivo de diapositivas, imágenes y diagramas oficiales, capturas, vídeos, ejemplos, requisitos de accesibilidad.
- Cuando solo exista la narración pero falte un recurso visual, preparar plan y señalar dependencia; **no sustituir sin aprobación** paleta/estilo ni inventar figuras oficiales.
- Trabajar sobre la copia de la plantilla; nunca alterar original ni otro deck existente sin instrucción expresa.
- Antes de editar Slides nativo, cargar la habilidad del conector Google Slides y usar sus métodos de lectura, copia y edición; comprobar límites reales de notas, multimedia, animaciones y permisos antes de prometer inserción.

## Secuencia obligatoria
**Puntos curriculares → Narración completa y validada → Unidades visuales → Texto en pantalla (derivado) → Selección de gráficos → Google Slides + notas → Auditoría de correspondencia y visual.**

La narración es el contenido maestro; las diapositivas no determinan artificialmente qué debe decir el docente. Se admite iterar textos en pantalla por problemas de legibilidad siempre que todo su contenido se explique por la narración.

## 1. Planificación visual (slide planner interno)
1. Leer todos los segmentos de la narración, su orden, punto(s) curricular(es) y propuesta de texto en pantalla.
2. Dividir en **unidades didácticas visuales** por concepto, contraste, proceso, demostración o transición lógica. **Prohibido aplicar una diapositiva por punto como regla fija**: un punto puede requerir varias slides y varios puntos relacionados pueden compartir una.
3. Crear una fila por slide en `references/slide-plan-template.md` con: ID slide, secuencia, papel, clase, IDs de puntos, IDs de segmentos de narración **exactos y contiguos cuando corresponda**, título editable, texto visible exacto, concepto gráfico, tipo de representación, fuente, notas y criterios de validación.
4. Repartir **todos** los segmentos narrados de la clase en slides o transiciones explícitas; no perder contenido narrado para acortar la presentación. Evitar una sola slide saturada o un número artificial de slides.
5. Asegurar una idea dominante por slide, no confundir «una idea» con «una sola frase»; los detalles técnicos pueden agruparse cuando se explican con claridad.
6. Elegir como tipo de recurso: formas nativas, diagrama vectorial editable, ilustración, foto, screenshot, tabla, gráfico de datos, diagrama oficial o ninguno. **No usar imagen por decoración**.
7. Mantener un mapa bidireccional `punto → segmentos → slides` y `slide → texto visible → segmentos narrados`; registrar excepciones.

## 2. Texto en pantalla
- Utilizar los textos auditados de `course-lesson-builder` como punto de partida.
- Todo título, etiqueta, cifra, diferencia, viñeta y conclusión visible debe estar **explicado completamente en la narración asignada**. La correspondencia puede ser semántica; no se exige recitación literal.
- El texto visible será selectivo, legible y corto respecto de la narración. No introducir nuevos requisitos, conceptos, ejemplos o porcentajes.
- La narración puede contener explicaciones sin texto en pantalla equivalente: eso es intencional.
- Usar texto nativo de Google Slides. No rasterizar palabras del contenido para conservar apariencia; excepción: texto intrínseco de una captura o figura oficial.
- La síntesis visual no podrá borrar distinciones esenciales del estándar fuente.

## 3. Elección y producción de gráficos
**Prioridad:** elemento nativo editable apropiado → recurso oficial fiel → recurso aportado/verificable → ilustración generada desde estilo maestro → sin elemento si no aporta claridad. Esta prioridad puede variar por precisión: un diagrama oficial complejo debe insertarse desde la fuente, no imitarse como un gráfico nativo técnicamente inexacto.

Para cada recurso:
- Definir exactamente qué demuestra, no solo su estética.
- Utilizar `PROMPT_MAESTRO_APROBADO + CONCEPTO + COMPOSICIÓN + RESTRICCIONES TÉCNICAS` en imágenes generadas.
- La línea gráfica se conserva entre slides; la composición varía según el concepto.
- Usar fondo transparente o blanco puro según integración y compatibilidad real.
- Diagramas y logos oficiales (p. ej., rueda de funciones NIST, Tiers) son **activos externos** que requieren fuente verificable y fidelidad de contenido/relaciones; no inventar ni deformar.
- Preservar proporción, recorte, nitidez, contraste y márgenes. No cortar etiquetas técnicas.
- Evitar gráficos no explicados, iconografía indiscriminada y decoración genérica.

## 4. Construcción de Google Slides
- Formato fijo **16:9** y layouts aprobados de `course-slide-template`.
- Diapositiva de apertura: fondo principal oscuro, elemento gráfico izquierda, título de clase editable derecha, blanco y acento secundario.
- Desarrollo: **fondo #FFFFFF**, título oscuro arriba, línea fina del secundario, contenido solo bajo separador, sin pie de página ni ornamentos automáticos.
- Duplicar o utilizar los layouts del deck **aprobado** respetando estructura y geometría. No reconstruir la plantilla desde cero por comodidad.
- Mantener títulos, formas, diagramas, flechas, tablas y etiquetas como objetos nativos cuando sea posible; las ilustraciones rasterizadas permanecen assets individuales.
- Comprobar fuente, contraste, color, alineación, clipping, márgenes, tamaños y espacio negativo a escala real. Ajustar composición, no recurrir a texto minúsculo para encajar información excesiva.
- **Notas del presentador:** insertar el texto íntegro del/los segmento(s) vinculados a cada slide, con ID de segmento opcional y sin marcadores técnicos que deban narrarse. No reducir el guion al resumen de pantalla.
- Si la herramienta conectada no permite escribir/leer notas, marcarlo como bloqueo parcial y entregar la transcripción segmentada complementaria, **sin afirmar que la narración quedó incorporada**.
- Si se solicita además audio reproducible, tratar como subproyecto explícito de grabación/TTS, importación a Drive, inserción y sincronización; no confundir con notas.

## 5. Verificación final y entrega
- Validación **estructural**: número/orden de slides, IDs, texto nativo, assets, layouts, notas (mediante lectura de vuelta cuando sea posible).
- Validación **visual**: renderizar el deck y revisar cada slide; corregir superposiciones, cortes, contrastes, espaciados y saturación.
- Validación **semántica**: cada punto está desarrollado en narración; todos los segmentos narrados están asociados; cada afirmación visual tiene soporte; cada gráfico es fiel.
- Prohibido declarar “Google Slides listo” si solo existe storyboard, PPTX local, imagen estática o enlace no confirmado.
- Entregar URL nativa real, plan de slides y auditoría. Adjuntar guion separado solo cuando es útil o cuando las notas no pudieron insertarse.

## Auditoría obligatoria
1. Cobertura de cada punto curricular por narración y slides.
2. Cobertura de **todos** los segmentos de narración en notas o transcripción explícita.
3. Correspondencia afirmación visible ↔ segmento narrado (bloqueante).
4. Coherencia de cada gráfico con su narración y el estándar fuente (bloqueante para diagramas técnicos).
5. Selección de recursos con utilidad didáctica.
6. Densidad adecuada y una idea dominante por slide.
7. Integridad de la plantilla, paleta, tipografía y fondo blanco de desarrollo.
8. Legibilidad y accesibilidad: contraste, tamaño, recorte, escala.
9. Edición nativa de texto y objetos donde proceda.
10. Consistencia del estilo de ilustración global, con composiciones variables.
11. Correspondencia slide ↔ notas correctas y ordenadas.
12. Precisión y vigencia técnica.
13. Ausencia de redundancia visual/narrativa innecesaria.
14. Naturalidad y ausencia de texto generado artificialmente.
15. Calidad de exportación/render de cada slide.
16. Proveniencia, créditos, permisos y enlaces de assets.

Estados: `Cumple`, `Requiere ajuste`, `No verificable`; severidad Crítico/Mayor/Menor, evidencia y corrección. Una omisión curricular o afirmación visible sin sustento narrado es **crítica**. Auditar borrador, corregir y volver a auditar la entrega real.

## Salidas
- `slide-plan.md` o tabla equivalente (una fila por slide).
- Presentación Google Slides editable 16:9 con notas por slide, **si las herramientas permiten completar la inserción y verificarla**.
- Matrices de trazabilidad y auditoría final.
- Lista de assets oficiales/generados con procedencia y limitaciones.

## Control editorial
No modificar la narración o el temario aprobado silenciosamente para acomodarlo a una slide; devolver necesidades de corrección a `course-lesson-builder` o proponer redistribución. Si el contenido exige más espacio, crear más slides. Las modificaciones de reglas globales pasan por `course-skill-improver`.
