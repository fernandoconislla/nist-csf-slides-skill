# PROJECT_STATE — NIST CSF 2.0

## 8. Corrección de activos en la diapositiva 02 — 2026-11-14

El usuario detectó una desviación de la regla de imágenes oficiales: la apertura panorámica de la clase 4.4 había mostrado círculos con números. **Corrección aprobada a nivel de criterio visual:** miniaturas oficiales reales de Núcleo, Perfiles y Tiers con nombre y finalidad breve, tres columnas equilibradas y legibles. Reglas actualizadas en skills y referencias. Propuesta editorial conservada en `proposals/class-4.4-componentes-del-marco-v4.md` (**NO aprobada como clase**). Queda **pendiente** rehacer y presentar maqueta SVG de slide 02 con los tres espacios de imágenes, obtener imágenes auténticas y probar legibilidad real, auditar storyboard global y solicitar aprobación editorial; no modificar Slides acumulativo ni marcar casillas.

> Punto de reanudación del proyecto. Verificado el **14 de noviembre de 2026** (hora de Perú).
> **Este archivo no sustituye las fuentes vivas.** En cada nueva sesión, comprobar el estado actual de GitHub, Google Sheets y Google Slides antes de trabajar. No inferir que una propuesta está aprobada.

## 1. Enlaces y jerarquía de fuentes

| Recurso | Uso | URL |
|---|---|---|
| Repositorio de skills | Reglas y pruebas; rama `main` | https://github.com/fernandoconislla/nist-csf-slides-skill |
| Skill principal | Puertas y orden de trabajo | https://github.com/fernandoconislla/nist-csf-slides-skill/blob/main/SKILL.md |
| Visual composition | Diseño preventivo y criterios VIS | https://github.com/fernandoconislla/nist-csf-slides-skill/blob/main/references/visual-composition.md |
| Temario maestro | IDs, clases, puntos, cobertura, auditoría, aprobada/grabada | https://docs.google.com/spreadsheets/d/19KQpeCfZpkNPC9m0zAbRGGh-E0p7vdMNL0aiwiiIk1Y/edit |
| Plantilla maestra | **Solo lectura**; estilos, portada y desarrollo | https://docs.google.com/presentation/d/1LuxRkFk9y4Bb4dDNLOP0gZWYXc90A8TFcxFi4ER-F6A/edit |
| Presentación acumulativa | **Destino editable** de clases nuevas tras aprobación editorial | https://docs.google.com/presentation/d/1h8BqC56ud8_4xKm_Aco9V-XcMdfVlaLwNedodUMgOvE/edit |
| Fuente oficial | NIST CSWP 29 en español | https://nvlpubs.nist.gov/nistpubs/CSWP/NIST.CSWP.29.spa.pdf |

**Regla de fuente de verdad:** GitHub dicta el proceso; Sheets dicta el temario y estado de clases; la presentación acumulativa dicta el contenido materialmente producido; la plantilla dicta la identidad visual. Las notas de presentador deben cotejarse con la narración aprobada. Resolver diferencias a partir de lecturas actuales, no de recuerdos.

## 2. Estado verificable al cierre de esta actualización

- Curso: **NIST CSF 2.0 — Implementación y Auditoría de Ciberseguridad**.
- Temario: **16 módulos, 68 clases**; pestañas `Temario`, `Puntos de contenido`, `Matriz de cobertura`, `Auditoría`, `Análisis competitivo`, además de cuatro respaldos ocultos de 2026-11-13.
- `Temario` contiene casillas **Aprobada** (G) y **Grabada** (H). `Estado` (F) es distinto: no interpretarlo como seguimiento de aprobación visual.
- **Aprobadas por el usuario:** 4.1, 4.2, 4.3 (casillas G activas). **Grabadas:** ninguna confirmada (H desmarcadas). Marcar `Grabada` solamente cuando el usuario lo confirme.
- Presentación acumulativa: **11 diapositivas**: 4.1 ocupa 1–4, 4.2 ocupa 5–7 y 4.3 ocupa 8–11. Las 11 tienen notas de presentador en el recurso Google Slides consultado anteriormente. Se recuperó texto/estructura, pero **no se ha completado en esta recuperación una inspección visual de todas las diapositivas**.
- Plantilla maestra: presentación separada con **2 diapositivas**; sus masters/layouts y render final deben analizarse antes de una nueva construcción.
- Identidad NIST aprobada: 16:9, Inter, azul marino `#102B46`, celeste `#00B8D9`, blanco `#FFFFFF`. Las figuras oficiales no se recolorean ni deforman.
- La copia independiente de la clase 4.2, `1WKV9iJHHn1E47Ubn9c6-GRBa-Zbx1gcHIVIrCo_ydJQ`, **no** es el destino ni una fuente aprobada.
- GitHub `main` antes de añadir este archivo: commit `6d0d528acf3e1b24463cc9bdcc5f355c6b3daca0`. Leer el nuevo HEAD en sesiones posteriores.

## 3. Clase activa — 4.4 «Componentes del Marco»

**Estado:** propuesta editorial en elaboración; **NO aprobada**, **NO grabada**, **NO construida**.

**Duración objetivo:** ~3–5 minutos. Alcance: panorama suficiente para comprender qué existe y para qué sirve, sin desarrollar temas de las clases posteriores.

**Decisiones y requisitos expresos del usuario:**
1. Presentar los tres componentes: **Núcleo del CSF**, **Perfiles Organizacionales** y **Niveles del CSF (Tiers)**.
2. Dar una explicación breve, clara y suficiente del propósito de cada componente.
3. Mencionar la organización del Núcleo por **funciones, categorías y subcategorías**.
4. **Enumerar**, sin definir una por una, las seis funciones: **Gobernar, Identificar, Proteger, Detectar, Responder y Recuperar**.
5. Explicar brevemente cómo se complementan los tres componentes.
6. Evitar anticipar los desarrollos específicos: 4.5 (funciones), 4.6 (categorías/subcategorías), 4.7 (perfiles/tiers), secciones posteriores de aplicación.
7. **Gráficos oficiales** para temas específicos de NIST. Verificar en la publicación original la figura precisa de Núcleo, funciones, Perfiles y Tiers, sus etiquetas, alcance y correspondencia narrativa. No reemplazar un gráfico oficial por iconos genéricos ni presentar un esquema docente como oficial. La portada mantiene la identidad visual del curso.

**Diferencia pendiente entre conversación y fuente viva:** el Google Sheet vigente tiene **dos** puntos, `4.4.1` (visión general de los tres componentes) y `4.4.2` (cómo se complementan). La propuesta editorial más reciente sugirió **tres** apartados, separando una vista rápida de la estructura del Núcleo y la enumeración de seis funciones. Esta propuesta **aún no ha sido incorporada al Sheet ni aprobada como contenido final**. Antes de editar los puntos, contrastar con el usuario o elaborar la propuesta con trazabilidad conservando IDs y cobertura. No declarar sincronización inexistente.

**Storyboard provisional:** propuesta de seis diapositivas (portada, tres componentes, Núcleo/jerarquía, seis funciones, Perfiles, Tiers). **No aprobado.** Se planteó antes de redactar narración completa y sin inspección integral de la plantilla; volver a determinar cantidad y composición siguiendo el orden obligatorio, sin convertir seis en una cuota fija.

**Próximo trabajo específico:** recuperar estructura visual real de la plantilla y de las 11 diapositivas vigentes; leer puntos 4.4 y clases vecinas; preparar narración íntegra de 3–5 minutos, auditarla; derivar texto visible, matriz de trazabilidad, activos oficiales y storyboard; obtener **aprobación editorial explícita** antes de escribir en Slides.

## 4. Proceso obligatorio — tres puertas

**Fase A: editorial, sin escritura de Slides**
1. Leer skill raíz, referencias visuales, `course-class-producer` y subskills; reconsultar Sheets.
2. Verificar fuentes normativas, cobertura y límite entre clases.
3. Elaborar **narración completa por segmento/slide**, evaluar redundancia, exactitud y duración; optimizar.
4. Derivar texto **en pantalla** exclusivamente de la narración; mapa `punto → narración → slide` y `slide → pantalla → narración`.
5. Analizar masters/layouts/ejemplares de plantilla, elementos editables, geometrías y renders; seleccionar figuras auténticas.
6. Proponer storyboard detallado, especificación de activos y disposición, auditar preventivamente la composición y **solicitar aprobación expresa**.

**Fase B: construcción**
7. Solo tras aprobación, **añadir** nuevas diapositivas al **final de la presentación acumulativa**, conservando plantilla y clases previas. No generar un deck por clase.
8. Usar textos y formas nativas editables; conservar relaciones, colores, dimensiones y proporciones de figuras oficiales.
9. Insertar notas íntegras en cada slide; sustituir notas anteriores por `deleteText ALL` + `insertText` si se regeneran, nunca concatenar.

**Fase C: QA y aceptación**
10. Releer literalmente notas, verificar su correspondencia con pantalla y puntos.
11. Inspeccionar el render real, geometrías, legibilidad, densidad, contrastes y errores, reequilibrar si procede.
12. Ejecutar regresión sobre clases anteriores y tests `NIST41` y `VIS-01…VIS-09`; distinguir casos escritos de **pruebas efectivamente ejecutadas**.
13. Entregar enlace al deck acumulativo para aceptación visual. **Solo marcar Aprobada en Sheets tras confirmación del usuario**. **Solo marcar Grabada cuando confirme la grabación**.

Las mejoras de skills requieren evidencia, propuesta/diff, aprobación y pruebas. Evitar commits silenciosos con alteraciones de reglas.

## 5. Pendientes y riesgos abiertos

- **P0 operativo:** reconciliar la propuesta de 4.4 con los dos puntos vigentes del Sheet y fijar alcance antes de narrar.
- **P1:** analizar/revisar realmente los renders de plantilla y diapositivas 1–11; la lectura de objeto/texto no equivale a auditoría visual.
- **P1:** validar imágenes oficiales contra NIST CSWP 29; las imágenes encontradas por búsqueda son referencias, no activos verificados automáticamente.
- **P1:** no confundir el proceso de cinco pasos para **crear y utilizar Perfiles Organizacionales** de NIST SP 1301 con un procedimiento universal de implementación del marco.
- **P1:** pestaña `Auditoría` documenta límites por verificar (paráfrasis oficiales, material comercial ISACA, entregables efectivos). Distinguir cumplimiento estructural de calidad del desarrollo.
- **P1:** pruebas VIS registradas en GitHub pero la ejecución de regresión de una nueva clase permanecía pendiente durante la recuperación.
- **P2:** mantener este archivo actualizado cuando el usuario apruebe clases, confirme grabaciones, cambie el temario o se complete un hito técnico. Siempre indicar fecha y evidencias, sin suplantar a Sheets.

## 6. Arranque rápido para una nueva conversación

> «Recupera el estado real de mi curso NIST CSF 2.0. Conecta GitHub y Google Drive. Lee primero `PROJECT_STATE.md` y `SKILL.md` en `fernandoconislla/nist-csf-slides-skill`, además de `references/visual-composition.md`, el temario maestro y las presentaciones enlazadas. Comprueba el estado vivo (no confíes ciegamente en el resumen). Sigue `course-class-producer` y sus puertas de aprobación. Retoma la clase 4.4 «Componentes del Marco»: panorámica de 3–5 min, tres componentes, enumerar las seis funciones sin explicarlas, mencionar categorías/subcategorías y usar figuras oficiales. Primero presenta narración y storyboard auditados; no escribas Google Slides antes de mi aprobación.»

## 7. Actualización de reglas — 2026-11-14 (feedback clase 4.4)

- La apertura panorámica puede explicar **brevemente para qué sirve cada componente**, aunque las siguientes diapositivas amplíen esas finalidades. Es repetición pedagógica funcional, **no redundancia perjudicial automática**; las duplicaciones reales siguen auditándose con evidencias.
- Reintroducida como puerta editorial obligatoria la **maqueta SVG 16:9 visible en conversación** por diapositiva: tras guion completo auditado, texto exacto y storyboard; antes de aprobar y producir Slides.
- Referencia compartida: `references/editorial-redundancy-svg.md`; siete skills especializadas, raíz y composición visual actualizadas. Casos RED/SVG/STATE **definidos pero todavía NO ejecutados**.
- **Estado de 4.4 sin cambios:** propuesta editorial de cinco diapositivas **no aprobada**, ninguna diapositiva añadida en este ciclo. La maquetación SVG previa fue preliminar, con placeholders. Revisar si los recursos oficiales encajan tras seleccionar activos auténticos.
- **Pendiente:** comparar las dos filas vigentes 4.4.1/4.4.2 de Sheets con el desglose en tres temas propuesto por conversación; no afirmar que tres puntos se guardaron. Mantener los IDs hasta nueva autorización.
- **Pendiente:** hacer inspección **real** de renders de la plantilla y de las nuevas slides; comprobación nativa de masters/layouts por sí sola no es QA visual.
- **Pendiente:** confirmar figuras oficiales exactas Núcleo/Perfiles/Tiers y relación con el guion; evitar figura de procedimiento de perfiles cuando no se narran sus pasos.
- **Pendiente:** narración, textos en pantalla y maquetas finales auditados, aprobación editorial, construcción en deck acumulativo, notas íntegras, QA y aprobación visual final de 4.4.

## 9. Construcción parcial verificable de clase 4.4 — 2026-11-14

**Cambios reales en el deck acumulativo:** el usuario solicitó «genera clase» y se insertaron **5 diapositivas nativas editables en posiciones 12–16** (IDs `csf44_cover`, `csf44_overview`, `csf44_core`, `csf44_profiles`, `csf44_tiers`). Total del deck: **16 diapositivas**. Las once anteriores permanecen en posiciones 1–11. Plantilla maestra **sin editar**.

**Nota importante:** Cualquier apartado anterior de este archivo que diga «4.4 no construida» se refiere al punto histórico antes de esta actualización y está superado por este registro.

**Narración:** se rellenaron las notas de los cinco slides, se leyeron de vuelta y se comprobó que no están vacías. La portada hereda su imagen original; dos diapositivas llevan la **rueda oficial NIST CSF 2.0** desde NIST https://www.nist.gov/sites/default/files/images/2024/04/15/CSF-wheel-revamp-v5-transparent_Op%203.png. La rueda corresponde a **funciones**, NO a toda la jerarquía de categorías/subcategorías.

**Estado real:** **PRODUCCIÓN PARCIAL — NO APROBADA, NO GRABADA**. La diapositiva 02 tiene imágenes oficiales de Perfiles y Tiers **pendientes de inserción**, la diapositiva 04 pendiente de captura NIST de Perfiles y la diapositiva 05 pendiente de la figura 4 del documento CSWP 29. Se utilizaron rótulos visibles de «PENDIENTE DE INSERCIÓN», nunca recreaciones pretendidamente oficiales. **No declarar que ha cumplido la regla de tres figuras oficiales pequeñas.**

**Pendientes bloqueantes para aprobación:** 1) conseguir figuras auténticas exactas de Perfiles y Tiers en formato insertable; 2) sustituir marcadores y verificar correspondencia/relevancia, tamaños y legibilidad; 3) verificar fidelidad de diapositiva Núcleo (rueda oficial no sustituye figura 1 completa); 4) revisar todos los renders reales (las miniaturas se solicitaron, pero sus píxeles no se inspeccionaron efectivamente); 5) auditoría completa de posiciones, transformación, densidad y regresión; 6) obtener aceptación visual final del usuario. Mantener G14 `Aprobada=false`, H14 `Grabada=false` hasta confirmación.

**Auditoría estructural realizada:** lectura del deck verifica 16 slides con 4.4 en posiciones 12–16, notas no vacías y al menos rueda institucional insertada en las diapositivas 13 y 14. Esta evidencia **no** equivale a aprobación visual final.

## 10. Corrección visual de las cinco diapositivas 4.4 — 2026-11-14

Tras petición expresa «corrige», se corrigieron **en el deck acumulativo existente** las diapositivas 12–16, preservando IDs/posición de las 11 aprobadas y la plantilla maestra. **Presentación:** https://docs.google.com/presentation/d/1h8BqC56ud8_4xKm_Aco9V-XcMdfVlaLwNedodUMgOvE/edit. **Revisión verificada:** `yyp4h8D3Sb3XqA`; **16 slides**.

**Cambios efectivamente aplicados:**
1. Slide 12: portada con imagen protagonista original preservada; título «Componentes / del Marco».
2. Slide 13: **tres imágenes auténticas pequeñas** (rueda de funciones NIST, recorte de captura real de plantilla Current/Target y figura 4 Tiers), tres nombres y descripciones, sin círculos de números ni placeholders. El recorte proviene de la captura de un libro de trabajo NIST mostrada por un tercero; conservar esta procedencia y no presentarlo como un archivo gráfico publicado directamente por NIST.
3. Slide 14: figura 1 auténtica **CSF Core structure** con funciones, categorías y subcategorías; retiradas la rueda (representación incompleta) y la enumeración extra redundante. Etiquetas de la figura en inglés; la narración permanece en español.
4. Slide 15: captura real de plantilla de Perfiles con Actual/Objetivo y rótulo separado de Perfil Comunitario; sin placeholder.
5. Slide 16: figura 4 auténtica de cuatro Tiers en escalera, proporción respetada y cierre narrado; etiquetas de la figura en inglés.

**Procedencia de figuras**: el contenido de la figura 1 y 4 se comprobó en el PDF oficial NIST CSWP 29 (español), pero los bytes insertados son reproducciones fieles alojadas por terceros: `csf.tools/wp-content/uploads/2024/03/csf-core-1024x604.png`, `ajcs01.github.io/CRM_Lec_L7/figures/nisttiers.png`; la rueda de NIST directamente de `nist.gov/sites/default/files/images/2024/04/15/CSF-wheel-revamp-v5-transparent_Op%203.png`. Captura de plantilla de Profiles originalmente desde artículo UpGuard basado en la plantilla NIST; en slide 13 se utilizó un recorte fiel de la misma, sin IA ni redibujado. Pueden sustituirse más adelante por extracciones de la publicación oficial en español si el usuario exige etiqueta en español.

**QA realizado:** exportación PDF nativa de **16 páginas**, renderización de las páginas **12–16**, inspección visual efectiva de las cinco diapositivas (composición, márgenes, legibilidad, sin marcadores); lectura nativa de slides y notas. Imágenes por página 12–16 = `1, 3, 1, 1, 1`; longitudes de notas = `199, 447, 702, 711, 793` caracteres; **0** marcadores «PENDIENTE». Comprobación geométrica básica de límites. Archivos visuales de QA guardados solo en entorno de trabajo; no son aprobación del usuario.

**Resultado interno:** errores de generación señalados previamente corregidos en el deck. **Estado formal: PENDIENTE de aceptación visual expresa del usuario** y prueba de regresión visual comparativa de las once previas (solo comprobados ID/orden, no se modificaron). **NO** marcar Aprobada o Grabada sin confirmación. Ante correcciones futuras, editar exclusivamente 12–16.

## 11. Aprobación de 4.4 y apertura de 4.5 — 2026-11-14

**Aprobación expresa:** el usuario escribió «aprobado y propon siguiente». Se marcó **4.4 como Aprobada=TRUE** en Google Sheets maestro: pestaña `Temario`, celda `G14`. Lectura posterior confirmó `Temario!C14:H14` con `G14=TRUE` y `H14=FALSE`. **No grabada.** Presentación acumulativa sigue con 16 diapositivas, clase 4.4 posiciones 12–16. No editar 4.4 salvo petición posterior.

**Siguiente clase:** **4.5 — Núcleo del Marco: Las seis funciones**, todavía **NO aprobada ni generada**. Puntos de Sheets `4.5.1–4.5.7`: Gobernar, Identificar, Proteger, Detectar, Responder, Recuperar, interdependencia y operación continua. Para propuesta nueva, basarse en §2 y figura 2 de NIST CSWP 29 oficial, en español, y preservar 4.6 para categorías/subcategorías. Usuario exige que toda solicitud «propón» **incluya auditoría** y maquetas SVG visibles antes de construir. En curso de propuesta editorial; no crear diapositivas 17+ sin aprobación expresa.

## 12. Clase 4.5 construida — 2026-11-14

**Pedido del usuario:** «genera» tras aprobar editorialmente la estructura de **9 diapositivas**, una por cada función. Clase: **4.5 — Núcleo del Marco: Las seis funciones**.

**Generación verificada:** presentación acumulativa https://docs.google.com/presentation/d/1h8BqC56ud8_4xKm_Aco9V-XcMdfVlaLwNedodUMgOvE/edit, revisión `qVmNsVAyjDJE0Q`. Se añadieron **9 diapositivas (17–25)** con IDs:
`csf45_cover`, `csf45_overview`, `csf45_gv`, `csf45_id`, `csf45_pr`, `csf45_de`, `csf45_rs`, `csf45_rc`, `csf45_integration`.

**Formato y recursos:** portada duplicada de 4.4 con imagen original y título «Núcleo del Marco / Las seis funciones»; rueda oficial NIST CSF 2.0 insertada en slide 18 y cada una de 19–24, sin repintarla ni deformarla. Seis slides individuales comparten figura izquierda, propósito/ámbitos derecha y rótulo «Función en foco: [nombre]» debajo. Slide 25 usa dos paneles para actividad continua (GV/ID/PR/DE) y preparación permanente (RS/RC). Paleta azul marino #102B46, cian #00B8D9, fondo blanco e Inter.

**Narración:** notas completas insertadas y leídas de vuelta en 9 slides (longitud en caracteres: 358, 541, 759, 700, 822, 697, 662, 744, 710). Todas las notas están presentes. Sin desarrollo de categorías/subcategorías de clase 4.6. Cumple el esquema 4.5.1–4.5.7.

**Control de alcance:** 25 slides en total; la comparación nativa de IDs confirma **las primeras 16 preservadas en sus posiciones**. Nueve nuevas en posiciones 17–25 sin omisiones ni cambios de orden. Inspección geométrica nativa de las nueve: ningún objeto sale de los límites. Se exportó el deck a PDF y se renderizaron/inspeccionaron las nueve páginas 17–25, incluidas comparativa de todas las composiciones.

**Estado:** clase **GENERADA, PENDIENTE DE APROBACIÓN VISUAL DEL USUARIO, NO GRABADA**. No marcar `Aprobada` ni `Grabada` hasta confirmación. La comprobación visual confirma ausencia de desbordes visibles, pero el rótulo «Función en foco» no es un indicador conectado a un sector: si el usuario exige una flecha/callout específico hacia cada función, añadirlo a demanda sin deformar la figura original.

**Próxima clase** tras aprobación expresa: 4.6 Núcleo del Marco: Categorías y Subcategorías. Seguir propuestas y auditorías antes de producir.

## 13. Clase 4.5 — foco visual opción A insertado y auditado (2026-11-14)

**Usuario:** «corrige con opción A», posteriormente confirmó conexión y ordenó «hazlo entonces». **Ejecución real:** se insertaron **seis overlays independientes** sobre la rueda NIST en las diapositivas **19–24**, sin reemplazar ni deformar la imagen institucional y sin alterar notas ni otros elementos. Una máscara transparente con contornos cian y halo suave por sector: `csf45_gv_spotlight_v1` (anillo Gobernar), `csf45_id_spotlight_v1` (Identificar), `csf45_pr_spotlight_v1` (Proteger), `csf45_de_spotlight_v1` (Detectar), `csf45_rs_spotlight_v1` (Responder), `csf45_rc_spotlight_v1` (Recuperar). No se oscurecen las demás funciones ni se recolorea el material oficial. Capa editable como objeto imagen por encima de la rueda. Dimensiones de cada overlay 262 x 262 pt, origen (117, 176) pt. Rueda subyacente preservada, con rótulo «Función en foco» igualmente preservado.

**QA:** lectura estructural confirma las 6 imágenes de resaltado y **25 diapositivas**, revisión de Drive `te7zJSHfXZf2Tg`. Exportación PDF de 25 páginas y renderizado de páginas 19–24; inspección visual efectiva de los seis focos confirma contorno alineado con cada sector, etiquetas legibles, paleta azul marino/cian y sin obstrucción de la narración en pantalla. Contact sheet de QA en ruta de trabajo `/mnt/data/csf45_highlight_qa/contact.png`.

**Estado:** corrección **implementada**, clase 4.5 **pendiente de aprobación expresa del usuario**; `Aprobada=false`, `Grabada=false` todavía. No modificar clase 4.4 ni módulos previos. Preservar regla: figura oficial intacta + enfoque editorial selectivo en capas separadas cuando el mismo recurso NIST aparece reiterado para subcomponentes.

## 14. Clase 4.6 generada con recortes originales (2026-11-14)

**Solicitud:** usuario subió el PDF `NIST.CSWP.29.spa.pdf` y pidió «continúa», autorizando la construcción visual de la clase 4.6 conforme a la propuesta de seis slides. Se tomó el PDF oficial español original y se extrajeron cinco **recortes reales en PNG** con PyMuPDF a 3x, recortando texto NIST sin reescritura dentro de las imágenes. Los recortes fuente se conservan en el entorno de trabajo `/mnt/data/nist_crops_46_final/`; no presuponer que esas rutas están disponibles en otras sesiones.

**Presentación Google Slides acumulativa:** https://docs.google.com/presentation/d/1h8BqC56ud8_4xKm_Aco9V-XcMdfVlaLwNedodUMgOvE/edit. **31 slides**, clase 4.6 en **26–31**, ids: `csf46_cover`, `csf46_category`, `csf46_category_code`, `csf46_subcategory`, `csf46_numbering`, `csf46_exercise`. Revisión actual verificada `qLS2mXoLyU04pw`. El resto 1–25 permanece antes de 4.6; no se editaron las clases previas.

**Mapa visual confirmado**:
- 26 portada duplicada de familia gráfica de 4.5, título «Núcleo del Marco / Categorías y / Subcategorías».
- 27 tabla 1 p.16 del texto original de NIST (página PDF 22), con bloque de seis categorías de Gobernar enmarcado en cian.
- 28 fila `GV.RM` de tabla 1 con marco cian ajustado a la fila, sin reescribir el texto original.
- 29 bloque `GV.RM` y `GV.RM-01` de la página impresa 17 (página PDF 23), marco cian solo sobre identificador.
- 30 bloque original `PR.DS` de página impresa 21 (página PDF 27), incluidos `PR.DS-01, -02, -10, -11`, dos marcos cian sobre `PR.DS-02` y `PR.DS-10`, para explicar salto intencional de numeración.
- 31 bloque original `GV.RM-01`, código señalado, más descomposición editable `GV` / `RM` / `01` en tres paneles.

Todos los cuadros de enfoque son formas nativas editables, con imagen oficial como elemento independiente y proporciones preservadas. Notas narradas insertadas y verificadas, recuentos en caracteres: `370,626,602,694,734,776`. QA: exportación nativa a PDF con **31 páginas**, render final de 26–31 y contacto `/mnt/data/csf46_render_final/contact.png`; 2 rondas de revisión y corrección de contornos para no abarcar la línea inferior o tapar resultados. Verificado que no existen elementos fuera de página en ninguna de las 6. Las primeras 25 se conservaron como previo. Sección de numeración fiel a nota del apéndice A sobre huecos de categorías trasladadas de CSF 1.1.

**Estado editorial:** clase 4.6 **GENERADA, PENDIENTE DE APROBACIÓN VISUAL EXPRESA DEL USUARIO**, no marcar como grabada ni aprobada; la generación no acredita revisión ni aprobación del usuario. No modificar 4.5 ni 4.4 por implicación. Si se solicita ajuste, se pueden editar exclusivamente slides 26–31.

## 15. Clase 4.6 — corrección de foco visual + reglas de reintento (2026-11-14)
Usuario solicitó directamente reforzar los resaltados (27–31) y actualizar las skills con protocolo de reintentos. **Ejecutado en Google Slides original**, revisión verificada `QtyPp6rt-svPiQ` (31 diapositivas). Solo páginas 27–31 modificadas; en ellas se añadieron 5 chips cian y 6 contornos cian interiores, se ampliaron los 6 bordes originales a marino 6,5 pt. El borde interior es cian 3 pt. Se movieron rótulos/fuentes para dejar sitio a los chips. Chips exactos: «CATEGORÍAS DE GOBERNAR», «CATEGORÍA: GV.RM», «SUBCATEGORÍA: GV.RM-01», «SALTO INTENCIONAL: 02 → 10», «EJEMPLO COMPLETO: GV.RM-01». Imágenes oficiales originales no reemplazadas.
**QA real:** lectura nativa de presentación comprobó 31 slides, 5 chips, 6 marcos internos y notas intactas; export PDF y render de slides 27–31, inspección visual de todos los focos en `/mnt/data/csf46_strong_focus_qa/contact.png`. Ahora están visualmente destacados a tamaño de contacto, sin tapar texto fuente esencial. Se corrigió primer fallo de lectura por máscara `fields` inválida mediante relectura con esquema completo; la conexión funcionaba. **Estado:** corrección aplicada y verificada internamente, clase 4.6 pendiente aprobación visual del usuario. No marcar aprobada o grabada automáticamente.

## 16. Clase 4.6 — eliminación de oclusión de códigos y reintento efectivo (2026-11-14)
**Corrección solicitada:** slides **29, 30 y 31** tenían 4 focos de doble marco grueso que tapaban parcialmente `GV.RM-01`, `PR.DS-02` y `PR.DS-10`. **Se retiraron los 8 objetos de marco originales + interiores** y se crearon 8 indicadores laterales marino/cian (dos por objetivo), sin tapar glifos, manteniendo los chips cian y el contenido oficial NIST. No se tocaron otras diapositivas, notas ni recortes.
**Reintento real:** primera escritura falló por `requiredRevisionId` obsoleto `QtyPp6rt-svPiQ`; lectura nueva confirmó `JAyvmxVwXNw1Vw` y ausencia de nuevos objetos, por lo que se repitió la misma mutación sin riesgo de duplicado; escritura correcta con revisión `IF8N21sT4INjEw` y 24 operaciones aceptadas. Deck contiene 31 diapositivas.
**QA:** exportación actualizada a PDF y render de páginas 29–31: `/mnt/data/csf46_focus_safe_qa/contact.png`. Se inspeccionó el contacto tras corregir: los códigos completos se leen con indicadores a la izquierda, sin contornos sobre caracteres. **Clase 4.6 sigue pendiente de aprobación visual expresa**.

## 17. Clase 4.7 producida en Google Slides — 2026-11-14

**Solicitud:** usuario aprobó editorialmente V2 «Perfiles y Niveles del Marco» y pidió **«genera»**. Se construyó la clase como **seis slides nativas y editables**, posiciones **32–37**, en el deck acumulativo https://docs.google.com/presentation/d/1h8BqC56ud8_4xKm_Aco9V-XcMdfVlaLwNedodUMgOvE/edit. Revisión verificada `hVD8OPGTjRXlcA`; **37 slides** totales. Las primeras 31 conservan su posición e IDs.

**Slides:**
- 32 `csf47_cover`: portada institucional original con «Perfiles y Niveles / del Marco».
- 33 `csf47_profiles`: recorte auténtico de sección 3.1 (Perfil Actual y Objetivo) **corregido para eliminar una línea superior cortada**; dos bloques editables de síntesis.
- 34 `csf47_community`: pasaje real del Perfil Comunitario sección 3.1 y síntesis editorial editable.
- 35 `csf47_tiers_intro`: **«Niveles del Marco»**, figura 4 oficial de los cuatro Tiers, sin anticipar características individuales.
- 36 `csf47_tiers_features`: características resumidas por cada Nivel (1 Parcial, 2 Riesgo informado, 3 Repetible, 4 Adaptativo), cuadro editable y fuente apéndice B tabla 2.
- 37 `csf47_integration`: Perfiles y Niveles en dos paneles independientes, conexión bidireccional y síntesis.

**Narración:** íntegra de la propuesta V2 en notas de los seis slides; lectura de vuelta confirmó longitudes 470, 853, 753, 672, 1278 y 728 caracteres. Fondo blanco de desarrollo, Inter, paleta marino #102B46 y cian #00B8D9. Las imágenes derivan de recortes reales del PDF oficial en español, no gráficos inventados. Se añadieron créditos discretos en páginas 33–36.

**QA:** exportada presentación acumulativa de 37 páginas a PDF y render de páginas 32–37, inspeccionadas visualmente; contacto en `/mnt/data/csf47_render_final/contact.png`. Corrección ejecutada tras detectar el comienzo de línea cortado en captura del Perfil Organizacional; nuevo recorte muestra solo las definiciones completas. No se observan desbordamientos en las seis vistas. Lectura estructural confirmó orden, notas y recortes. Hubo un fallo interno transitorio de lectura y otro de escritura compuesta; ambos se recuperaron con lectura fresca y escritura dividida, sin duplicar objetos.

**Estado:** clase **4.7 GENERADA, PENDIENTE APROBACIÓN VISUAL DEL USUARIO, NO GRABADA**. No marcar como aprobada o grabada en Sheets sin confirmación explícita; preservar clases anteriores. La clase 4.6 está aprobada en Sheets G16; 4.5 continúa G15=false según última lectura.

## 18. Clase 4.7 — cambios pendientes ejecutados: perfiles visuales y un Tier por slide (2026-11-14)
**Solicitud:** «aplica los cambios pendientes». Se corrigió sobre la presentación acumulativa nativa https://docs.google.com/presentation/d/1h8BqC56ud8_4xKm_Aco9V-XcMdfVlaLwNedodUMgOvE/edit. Revisión verificada final: `VnwO_6-31Cb71Q`; **40 diapositivas** en total. Clase 4.7 ahora ocupa posiciones **32–40 (9 slides)**; anteriores 1–31 conservadas.
- 32 portada preservada.
- 33 `csf47_profiles`: sustituido el recorte de definición textual por representación gráfica nativa editable **Perfil Actual → diferencias → Perfil Objetivo**, sin adelantar procedimientos de análisis de brechas. Narración alineada con el nuevo gráfico.
- 34 `csf47_community`: eliminado recorte teórico; nuevo diagrama editable de **línea base de resultados compartidos → ejemplos reales en catálogo NIST**: manufactura, transporte y ransomware; se explica que puede informar un Perfil Objetivo. Página oficial consultada: https://www.nist.gov/cyberframework/profiles (confirmó ejemplos 2026-11-14). Narración actualizada.
- 35 `csf47_tiers_intro`: conserva figura 4 auténtica y presenta los 4 Niveles sin desarrollar características.
- 36–39 `csf47_tier1..tier4`: sustituyen la antigua slide 36 resumen. **Una slide por Nivel** y sus notas completas. Cada una conserva la **misma figura 4 oficial sin alteraciones** y tiene chip «NIVEL n EN FOCO» más **barra cian bajo el escalón correspondiente**, fuera de etiquetas; a la derecha dos secciones distintas **Gobernanza** y **Gestión de riesgos**, basadas en apéndice B tabla 2 del PDF original. Cuatro nombres: Parcial, Riesgo informado (figura lo nombra Conocimiento de los riesgos), Repetible, Adaptativo (figura lo nombra Adaptable). Dos intentos de creación: primero rechazado por falta de `image_uris` multiplicado para 4 imágenes idénticas; relectura corroboró que no se insertó ninguna y segunda escritura con 4 entradas exactas tuvo éxito. Narraciones de entre 599 y 703 caracteres. Se amplió altura de los paneles y se ajustó texto inferior tras inspección de render, sin tapar contenidos.
- 40 `csf47_integration`: cierre previo preservado y desplazado al final.
**QA real:** relectura de deck, 40 slides, nueve notas no vacías y tres recortes originales (portada + figura en 35–39) frente a gráficos editables en 33/34; exportación Google Slides a PDF de 40 páginas, render y revisión de 32–40. Vista general en `/mnt/data/csf47_v3_final/contact.png`. No se observan oclusiones de texto oficial ni placeholders pendientes; el recurso original de los Tiers sigue legible. No se alteraron las clases anteriores.
**Estado:** 4.7 **GENERADA / REVISIÓN VISUAL DEL USUARIO PENDIENTE / NO GRABADA**, no marcar aprobada sin aceptación explícita. La clase 4.6 permanece aprobada y la 4.5 continúa no aprobada según último Sheet leído.

## 19. Clase 4.7 aprobada y sistema de skills actualizado — 2026-11-14
**Aprobación del usuario:** «aprobado actualiza las skills con todos los pendientes». En Google Sheets maestro https://docs.google.com/spreadsheets/d/19KQpeCfZpkNPC9m0zAbRGGh-E0p7vdMNL0aiwiiIk1Y/edit, pestaña Temario, **G17=TRUE**; relectura confirmó **H17=FALSE**. No fue marcada como Grabada. Esta aprobación sucede después de la V3 de nueve diapositivas; sustituye los estados anteriores de 4.7 «pendiente de aprobación».
**Deck sin cambios al aprobar:** https://docs.google.com/presentation/d/1h8BqC56ud8_4xKm_Aco9V-XcMdfVlaLwNedodUMgOvE/edit, 40 diapositivas, revisión verificada VnwO_6-31Cb71Q, clase 4.7 en 32–40, nueve notas no vacías. Páginas 33–34 son diagramas editables de Perfil Actual/Objetivo y Comunitario; 35 figura 4 completa, 36–39 cuatro Niveles con figura oficial y señaladores, 40 integración.
**Estado de otras filas, según última lectura viva:** 4.5 G15=TRUE y H15=TRUE, 4.6 G16=TRUE y H16=FALSE; son valores del Sheet, pueden reflejar cambios ajenos al chat y **NO** deben reescribirse a partir de notas antiguas que afirmaban 4.5 pendiente. Clase siguiente 5.1 «Función Gobernar: propósito y categorías» G18=FALSE/H18=FALSE; no crear automáticamente sin petición.
**Aprendizajes consolidados:** autoridad de la fuente, distinción imagen textual/diagrama, comunidad separada del perfil organizativo, una slide por Tier, doble dimensión de apéndice B, introducción no redundante, foco exacto sin oclusión, QA por render, reintentos seguros, y aprobación independiente de grabación. Las actualizaciones en GitHub se documentan en CHANGELOG/FEEDBACK/tests. Registrar cumplimiento real, no confundir regla escrita con test ejecutado.

## 20. Clase 5.1 generada (2026-11-14)
- Solicitud directa «genera» tras propuesta V1 de 3 slides. Se ejecutó edición nativa en presentación acumulativa: https://docs.google.com/presentation/d/1h8BqC56ud8_4xKm_Aco9V-XcMdfVlaLwNedodUMgOvE/edit, revisión final `pr9bY-cVSkzMVw`. **43 slides** totales, anteriores 1–40 preservadas; nueva clase posiciones **41–43** con IDs `csf51_cover`, `csf51_purpose`, `csf51_categories`.
- 41: portada azul marino duplicada de familia institucional, título «Función Gobernar», imagen protagonista conservada.
- 42: «Propósito de la función Gobernar», rueda oficial NIST CSWP 29 fig. 2 y cuatro ideas clave editables; el texto redundante de fuente bajo la figura se retiró en QA.
- 43: «Las seis categorías de Gobernar», recorte REAL de la tabla 1 NIST CSWP 29 spa, p. impresa 16, con seis categorías GV.OC/RM/RR/PO/OV/SC. El primer recorte cortaba la palabra Gobernar; fue reemplazado por recorte limpio desde el PDF original, con encabezado y primera columna completos. El recorte conserva sus proporciones.
- Notas de narración completas insertadas: 356, 920 y 1265 caracteres. Inspección estructural Google Slides confirmó orden, 43 slides y notas. Exportación a PDF 43 páginas; render final de 41–43 inspeccionado en `/mnt/data/csf51_quality/final_contact.png`. Sin desbordamientos visibles. Estado **GENERADA, AUDITADA VISUALMENTE, PENDIENTE APROBACIÓN DEL USUARIO**; no modificar G18 ni H18 del Sheet antes de aprobación.
- Protocolo de reintentos: la exportación fue correcta; primer render local falló por transporte, se efectuó alternativa con Python/Fitz con éxito. No declarar pérdida de conexión por error de herramienta. Siguiente 5.2 solo por petición.

## 21. Clase 5.1 — actualización editorial de títulos (2026-11-14)
Usuario aprobó explícitamente el cambio de título («listo aplica»). Cambios ejecutados y verificados:
- Google Sheets maestro, Temario fila 18, columna D: `Gobernar (GV): Dirección estratégica de la ciberseguridad`. G18 y H18 permanecen FALSE.
- Google Slides acumulativo, 43 diapositivas, revisión `JWEUU6hr0Gzdgw`: diapositiva 41 portada `Gobernar (GV)` / `Dirección estratégica de la ciberseguridad`; diapositiva 42 título `Gobernar: Dirección estratégica de la ciberseguridad`; diapositiva 43 título `Categorías de la función Gobernar`. Se corrigió ortografía «Governar»/«funciona» a «Gobernar»/«función», de acuerdo con la aprobación del usuario. Ajustado tamaño tipográfico del título de la slide 42 a 27 pt por longitud.
- Lectura posterior confirmó los tres títulos, el nuevo campo de la hoja y total 43 slides. No se modificaron los textos de narración ni la aprobación/grabación. **Estado de 5.1: generada, pendiente aprobación visual formal**.

## 22. Clase 5.1 — foco Gobernar en figura oficial (2026-11-14)
- Usuario detectó que la diapositiva 42 no señalaba la función estudiada dentro de la rueda NIST («no resaltaste la función que nos toca ver»).
- Corregida **solo slide 42** `csf51_purpose`: chip marino editable «GV · GOBERNAR», con barra vertical cian y punto cian dirigidos al arco superior de la banda amarilla de **GOBERNAR** en la Fig. 2 oficial, sin tapar el nombre ni los otros sectores. Objetos: `csf51_govern_chip`, `csf51_govern_connector`, `csf51_govern_pointer`, `csf51_govern_chip_txt`. No se reemplazó/recoloreó la imagen ni se modificaron las notas.
- Revisión Slides `xsKd259Py7sDWQ`; lectura confirmó 43 diapositivas, cuatro objetos nuevos de foco. Exportación PDF de 43 páginas y render visual individual inspeccionado: `/mnt/data/csf51_slide42_govern_focus.png`.
- Aprendizaje: cuando una clase estudia una función específica, la rueda completa es orientación, pero debe llevar **foco visual explícito en el sector o anillo exacto** y señalador externo sin oclusión. Estado de 5.1 continúa pendiente aprobación formal del usuario.

## 23. Clase 5.1 — borde transparente de alto contraste (2026-11-14)
- El usuario pidió sustituir la etiqueta externa por un borde transparente alrededor de «GOBERNAR» en la rueda NIST de la slide 42 y autorizó elegir el estilo y ejecutarlo. Elegido: doble borde rectangular redondeado **marino 5 pt + cian 2,8 pt, sin relleno**; área del foco ajustada al texto de la función dentro del anillo amarillo oficial.
- Se eliminaron 4 objetos anteriores (`csf51_govern_chip`, `csf51_govern_connector`, `csf51_govern_pointer`, `csf51_govern_chip_txt`) y se crearon `csf51_gv_focus_outer` y `csf51_gv_focus_inner`; se preservaron rueda oficial, narración y resto del deck.
- Primera mutación rechazada por campo incorrecto `outline.solidFill`; relectura confirmó ausencia de efectos y se corrigió al contrato válido `outline.outlineFill.solidFill`. Revisión final `b3i9UqFQjMhAEg` (43 diapositivas).
- PDF exportado y slide 42 renderizada inspeccionada: `/mnt/data/csf51_slide42_double_border.png`. Borde inequívoco y alto contraste, sin texto oculto. Clase 5.1 sigue pendiente de aprobación visual global.


## 24. Clase 5.1 aprobada y estado actualizado — 2026-11-14

- **Aprobación expresa del usuario:** «esta clae esta aprobada» se refiere a **5.1 — Gobernar (GV): Dirección estratégica de la ciberseguridad**, tras corrección del foco gráfico de la diapositiva 42.
- **Google Sheets maestro verificado en vivo:** pestaña `Temario`, fila 18, `G18=TRUE` (**Aprobada**) y `H18=FALSE` (**Grabada**). La aprobación no implica grabación. Clase siguiente `5.2 — Contexto organizativo (GV.OC)`, fila 19, `G19=FALSE` y `H19=FALSE`.
- **Google Slides acumulativo verificado:** 43 diapositivas; 5.1 ocupa 41–43, con IDs `csf51_cover`, `csf51_purpose`, `csf51_categories`. Revisión verificada tras el ajuste `JgZFNDfjCL0tPQ`. En 42 se reemplazó la rueda previa por la imagen oficial de la slide 19 y se trasladó el mismo recurso de spotlight, preservando las relaciones relativas de posición y tamaño para evitar el desalineamiento provocado por diferentes proporciones de rueda. El recurso nuevo se llama `csf51_gv_spotlight_matching19`; los dos marcos previos fueron eliminados.
- **Estado formal:** 5.1 **APROBADA, NO GRABADA**. La aprobación expresada por el usuario prevalece sobre todos los registros históricos de «pendiente». No volver a alterar 41–43 sin solicitud expresa.
- **Próxima clase para propuesta editorial:** 5.2, cuyos puntos vigentes son 5.2.1 (propósito de GV.OC) y 5.2.2–5.2.6 (GV.OC-01 a GV.OC-05). Seguir el flujo y puertas de aprobación del orquestador. No crear ni aprobar 5.2 automáticamente.
- **Regla de seguimiento acordada con el usuario:** cada vez que apruebe una clase, sincronizar de inmediato su estado en Google Sheets y este archivo, contrastando ambas fuentes vivas, y preservar independientemente el campo Grabada. Verificar lecturas posteriores y no modificar slides aprobadas.

## 25. Clase 5.2 — Contexto organizativo (GV.OC) APROBADA — 2026-11-15

- **Aprobación explícita del usuario:** «aprobada la clase», referida a la clase activa **5.2 — Contexto organizativo (GV.OC)**, tras revisión y correcciones visuales de páginas 44–50.
- **Google Sheets maestro — lectura y escritura verificadas:** pestaña `Temario`, fila **19**, identificador `5.2`, título `Contexto organizativo (GV.OC)`; **G19=TRUE (Aprobada)** y **H19=FALSE (Grabada)**. Se modificó únicamente la casilla G19, preservando H19, la columna F, los títulos y las demás filas.
- **Presentación acumulativa — verificada sin modificarla durante el cierre:** https://docs.google.com/presentation/d/1h8BqC56ud8_4xKm_Aco9V-XcMdfVlaLwNedodUMgOvE/edit ; **50 diapositivas** en total, revisión consultada `1njiWtdGzYRSVA`; clase 5.2 en páginas **44–50**, IDs `csf52_cover`, `csf52_s2`, `csf52_s3`, `csf52_s4`, `csf52_s5`, `csf52_s6`, `csf52_s7`.
- **Identidad y contenido final:** portada institucional 44, categoría GV.OC y cinco subcategorías GV.OC-01…05 en 45–50. Jerarquía categoría/subcategorías, amarillo funcional de Gobernar, conectores editables, márgenes, centrado y simetría corregidos a partir del feedback y modificaciones manuales del usuario. Las notas de presentador se conservaron según las lecturas de control anteriores. No se afirma nueva inspección de render durante este cierre, ni ejecución completa de la batería automatizada de regresión.
- **Estado formal:** clase **APROBADA / NO GRABADA**. La aceptación expresa del usuario cierra su revisión editorial y visual. No editar estas diapositivas salvo nueva solicitud; no equiparar aprobación con grabación.
- **Siguiente clase:** **5.3 — Estrategia de gestión de riesgos (GV.RM)**, fila 20 de la pestaña Temario; en la última lectura G20=FALSE, H20=FALSE. No generar automáticamente: esperar petición expresa de continuar o producirla.
- **Nota de precedencia:** este cierre sustituye cualquier estado histórico de 5.2 «pendiente» en este archivo; los historiales de otras clases requieren consulta viva de Sheets y no deben deducirse de entradas antiguas.

## 26. Clase 5.3 — Estrategia de gestión de riesgos (GV.RM) generada — 2026-11-15
- **Solicitud explícita:** «genera la clase» tras la propuesta editorial V2 de nueve diapositivas. Se añadió la clase de forma **nativa y editable en la presentación acumulativa** https://docs.google.com/presentation/d/1h8BqC56ud8_4xKm_Aco9V-XcMdfVlaLwNedodUMgOvE/edit, sin alterar las clases aprobadas 1–50.
- **Estado real de la presentación:** **59 diapositivas**, con 5.3 en posiciones **51–59** y IDs `csf53_cover`, `csf53_category`, `csf53_rm01` a `csf53_rm07`. Se corrigió el orden tras duplicar desde ejemplares nativos; lectura final confirma la secuencia.
- **Contenido:** portada de familia institucional, categoría GV.RM con jerarquía amarillo Gobernar y siete códigos homogéneos, siete subcategorías con **enunciados literales contrastados contra NIST CSWP 29 spa (apéndice A, páginas impresas 17–18)** y diagramas nativos editables. Recursos gráficos distinguen objetivos acordados, apetito/tolerancia, integración en ERM, respuestas estratégicas, comunicación, método común y oportunidades.
- **Narración:** notas completas integradas por diapositiva, verificadas por lectura nativa; longitudes 602, 846, 664, 681, 671, 623, 663, 670 y 699 caracteres para 51–59 respectivamente.
- **QA:** exportación PDF de 59 páginas; render visual y contacto de las páginas 51–59 inspeccionados en `/mnt/data/csf53_qa/contact.png`. Detectado texto partido «Documentar/Categorizar» en la 58: corrección de tipografía en las cuatro etapas a 12 pt, exportación y segunda inspección de `/mnt/data/csf53_qa/slide_58_final.png` confirmaron ambos rótulos completos en una línea. Lectura nativa verificó las 59 páginas, orden, notas y ausencia de objetos fuera del lienzo.
- **Estado formal:** 5.3 **GENERADA / REVISADA / PENDIENTE APROBACIÓN DEL USUARIO / NO GRABADA**. No modificar la casilla `Aprobada` (G20) ni `Grabada` (H20) sin confirmación explícita. La última lectura de `Temario` mostró ambas en FALSE.
- **Siguiente paso:** revisión del usuario sobre las páginas 51–59; solo tras aprobación formal sincronizar estado con Sheets y GitHub. Los criterios de composición son preventivos, de implementación y de auditoría; no sustituir la inspección óptica por propiedades de API.

## 27. Clase 6.3 — Evaluación de riesgos (ID.RA) aprobada — 2026-11-17

- **Presentación acumulativa:** 110 diapositivas, revisión `mrrsibhhm1IBkg`. La clase 6.3 ocupa las diapositivas 99–110: `csf63_cover`, `csf63_category` y `csf63_ra01` a `csf63_ra10`. [Abrir la clase](https://docs.google.com/presentation/d/1h8BqC56ud8_4xKm_Aco9V-XcMdfVlaLwNedodUMgOvE/edit#slide=id.csf63_cover).
- **Auditoría:** revisión de los doce renders, las notas y la cobertura de los once puntos curriculares. Se ajustó el enunciado de la diapositiva 100 para reflejar el alcance del resultado ID.RA: organización, activos y personas. Las diez subcategorías tienen una imagen de apoyo por diapositiva, en marco 4:3 de 320 × 240 px con origen (542, 193) sobre una referencia de 960 × 540 px. Las imágenes se revisaron junto al enunciado y los SVG maestros se conservaron en el espacio de trabajo.
- **Temario:** clase 6.3 en la fila 27, `Aprobada=TRUE` y `Grabada=FALSE`, valores comprobados en lectura posterior. La columna de estado editorial conserva el valor vigente del temario. La grabación está pendiente de confirmación explícita. [Ver casillas](https://docs.google.com/spreadsheets/d/19KQpeCfZpkNPC9m0zAbRGGh-E0p7vdMNL0aiwiiIk1Y/edit#gid=816850988&range=G27:H27).
- **Siguiente clase en el temario:** 6.4 — Mejora (ID.IM), fila 28, pendiente de desarrollo. Comenzar su producción cuando se solicite expresamente.

## 28. Clase 6.4 — Mejora (ID.IM) aprobada — 2026-11-17

- **Presentación acumulativa:** 116 diapositivas, revisión `4wkzUFW8VIj8Wg`. La clase 6.4 ocupa las diapositivas 111–116: `csf64_cover`, `csf64_category` y `csf64_im01` a `csf64_im04`. [Abrir la clase](https://docs.google.com/presentation/d/1h8BqC56ud8_4xKm_Aco9V-XcMdfVlaLwNedodUMgOvE/edit#slide=id.csf64_cover).
- **Auditoría:** se inspeccionaron los seis renders y se verificó la correspondencia literal de las seis notas con el guion. Se cubren los cinco puntos curriculares. La lectura del esquema anterior y posterior confirmó la conservación del contenido y orden visibles de las diapositivas 1–110. Cada subcategoría tiene un gráfico de apoyo en marco 4:3 de 320 × 240 px con origen (542, 193) sobre una referencia de 960 × 540 px.
- **Temario:** fila 28, `Aprobada=TRUE` y `Grabada=FALSE`, verificados mediante lectura posterior. La grabación queda pendiente de confirmación explícita. [Ver casillas](https://docs.google.com/spreadsheets/d/19KQpeCfZpkNPC9m0zAbRGGh-E0p7vdMNL0aiwiiIk1Y/edit#gid=816850988&range=G28:H28).
- **Siguiente clase en el temario:** 7.1 — Proteger (PR): Protección de activos y reducción del riesgo, fila 29. Su producción comienza con una solicitud propia.

## 29. Clase 7.1 — Proteger (PR): Protección de activos y reducción del riesgo aprobada — 2026-11-18

- **Presentación acumulativa:** 119 diapositivas, revisión `2TswlXKoOctgxg`. La clase 7.1 ocupa las diapositivas 117–119: `csf71_cover`, `csf71_purpose` y `csf71_categories`. [Abrir la clase](https://docs.google.com/presentation/d/1h8BqC56ud8_4xKm_Aco9V-XcMdfVlaLwNedodUMgOvE/edit#slide=id.csf71_cover).
- **Patrón de introducción de funciones:** las diapositivas 87–89 de Identificar son las referencias indicadas por el usuario: portada de función, rueda oficial con el sector activo destacado y alcance a la derecha, y panorama de categorías con encabezados y fuente.
- **Auditoría:** se verificó la correspondencia literal de las tres notas con el guion y la cobertura de ambos puntos curriculares. La revisión posterior de las diapositivas 118 y 119 confirmó en los renders el foco sobre Proteger en la Figura 2 y la legibilidad de los encabezados y las cinco filas de la Tabla 1 del NIST. Las notas se conservaron y el contenido visible y orden de las diapositivas 1–117 coincidieron con la lectura previa a la corrección.
- **Temario:** fila 29, `Aprobada=TRUE` y `Grabada=FALSE`, verificados mediante lectura posterior. La grabación queda pendiente de confirmación explícita. [Ver casillas](https://docs.google.com/spreadsheets/d/19KQpeCfZpkNPC9m0zAbRGGh-E0p7vdMNL0aiwiiIk1Y/edit#gid=816850988&range=G29:H29).
- **Siguiente clase en el temario:** 7.2 — Gestión de identidades, autenticación y control de acceso (PR.AA), fila 30. Su producción comienza con una solicitud propia.

## 30. Clase 7.2 — Gestión de identidades, autenticación y control de acceso (PR.AA) aprobada — 2026-11-18

- **Presentación acumulativa:** 127 diapositivas, revisión `YQT-vbvCX5NtLg`. La 7.2 ocupa las diapositivas 120–127: `csf72_cover`, `csf72_category` y `csf72_aa01` a `csf72_aa06`. [Abrir la clase](https://docs.google.com/presentation/d/1h8BqC56ud8_4xKm_Aco9V-XcMdfVlaLwNedodUMgOvE/edit#slide=id.csf72_cover).
- **Auditoría:** se revisaron los ocho renders y se cotejaron las ocho notas con el guion. Se cubren siete puntos curriculares. Se verificó el orden previo de los 119 IDs y el marco de los seis gráficos, 4:3 de 320 × 240 px con origen (542, 193). La 123 ilustra un control contextual de ejemplo con código por correo en el acceso remoto; sus notas distinguen el inicio de sesión de la comprobación inicial de identidad y su vínculo con una credencial.
- **Temario:** fila 30, `Aprobada=TRUE` y `Grabada=FALSE`, verificados mediante lectura posterior. La grabación queda pendiente de confirmación explícita. [Ver casillas](https://docs.google.com/spreadsheets/d/19KQpeCfZpkNPC9m0zAbRGGh-E0p7vdMNL0aiwiiIk1Y/edit#gid=816850988&range=G30:H30).
- **Siguiente clase:** 7.3 — Concienciación y capacitación (PR.AT), fila 31. Su producción comienza con una solicitud propia.
