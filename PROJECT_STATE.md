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
