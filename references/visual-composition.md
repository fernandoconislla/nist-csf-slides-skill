# Composición visual preventiva y validación — NIST CSF 2.0

## Panorama de componentes con activos oficiales pequeños (2026-11-14)

Una visión general de un marco reconocido **no está exenta de la regla de recursos oficiales** por ser introductoria. Si se presentan tres componentes NIST y existe representación oficial adecuada de cada uno, el storyboard debe reservar tres imágenes oficiales auténticas **pequeñas** de función identificativa. Las imágenes van con nombre y descripción breve, con marco visual comparable sin alterar proporciones (contain), alineación de centros, igual altura óptica y suficiente nitidez/legibilidad; evitar números decorativos o iconos genéricos como sustitutos. En SVG, representar espacios reservados claramente rotulados, no recrear el documento original. Si un recurso oficial pequeño resulta ilegible, buscar recorte auténtico o redistribución; no sustituir por un icono IA. Ejemplo: clase 4.4 slide 02: rueda CSF 2.0, recorte NIST Profiles, figura NIST Tiers. No imponer el requisito sobre la portada ya aprobada ni usar figuras sin pertinencia.

## Puerta SVG visible y fidelidad de figuras (2026-11-14)

Después de narración completa auditada y storyboard, mostrar **maquetas SVG 16:9 visibles**. Deben revelar composición, centrado óptico, tamaños, densidad, márgenes y lugar de los activos auténticos. Los placeholders no deben aparentar ser diagramas oficiales. Una figura que explica un procedimiento no sustituye a una presentación conceptual de un componente. Inspeccionar primero la plantilla nativa y render cuando sea accesible. Leer `editorial-redundancy-svg.md`; aprobación editorial y aprobación visual final son puertas separadas.

## Alcance y precedencia
Referencia operativa para `course-slide-template`, `course-lesson-builder`, `course-slide-builder` y `course-class-producer`. Complementa la identidad aprobada y las restricciones de cada clase. No reemplaza el temario ni autoriza crear una presentación sin aprobación explícita.

## Puerta A — Antes de generar (OBLIGATORIA)
Para cada diapositiva crear un storyboard con: propósito pedagógico único, texto visible y notas asociadas, inventario de objetos, función de cada objeto, layout 16:9, márgenes, zonas, alineaciones, tamaños aproximados, paleta, contraste y relaciones entre objetos.
1. **Economía visual:** un elemento solo se mantiene si informa, agrupa, separa conceptos diferentes o expresa una relación. Eliminar barras horizontales, acentos y bordes puramente ornamentales. La línea celeste principal bajo el título forma parte del layout aprobado; cualquier línea adicional requiere justificación semántica.
2. **Balance preventivo:** calcular la distribución del conjunto (no solo objetos aislados): centro óptico, blancos, densidad, márgenes, ritmo entre grupos y posición del cierre. Si se propone simplificar, **rediseñar primero el layout**; no retirar elementos conservando coordenadas residuales.
3. **Columnas:** anchuras visualmente equivalentes, centros de iconos alineados, títulos en línea base coherente, descripciones y distancia entre bloques homogéneas. Diferenciar elementos por icono/título cuando baste; no agregar barras encima por defecto.
4. **Color funcional:** en NIST `#102B46` para texto e información principal, `#00B8D9` para conexiones y énfasis funcional, blanco `#FFFFFF`. Ejemplo local: símbolo ⇄ celeste, texto «Comunicación bidireccional» azul marino. No aplicar estos roles mecánicamente cuando contradigan contraste o autenticidad de una figura oficial.
5. **Geometría constructiva:** preferir formas nativas completas con contorno a rectángulos hechos de cuatro piezas; conectores/flechas nativas editables con puntos, orientación, peso y proporciones previstas. En Google Slides comprobar la matriz de transformación y las magnitudes efectivas, especialmente al crear líneas de anchura casi nula.
6. **No prescribir píxeles universales:** valores de desplazamiento empleados en un caso concreto (15, 18, 24, 26, 38 px/pt) son correcciones locales, no normas aplicables a clases futuras.
**Criterio de salida:** si el storyboard tiene elementos sin función, alineaciones indefinidas, un recurso oficial deformado o una composición desequilibrada previsible, NO construir; corregir la propuesta antes de solicitar la aprobación o ejecutar.

## Puerta B — Durante la construcción
- Crear objetos según el storyboard aprobado; confirmar dimensiones, transformaciones, cierres, proporciones, flechas y alineación al insertarlos.
- Usar coordenadas en la unidad real del Slides (PT/EMU según API) con conversiones explícitas. Comparar bounding boxes de iconos, rótulos, cajas y flechas; comprobar área útil y márgenes.
- Mantener identificadores estables cuando corresponda; editar solo las diapositivas autorizadas, preservar diseño previo aprobado y notas de presentador.
- Tras quitar cualquier objeto, recalcular inmediatamente el encuadre de los elementos restantes, su centro de masa visual y los espacios superiores/inferiores. No dar por buena una composición simplificada sin nuevo layout.

## Puerta C — Después de generar
- Inspección estructural: objetos, contenido, paleta, transformaciones, contornos, bounding boxes, flechas, solapamientos, notas y orden.
- **Inspección visual real:** observar la renderización para validar jerarquía, escala, contraste, recortes y acabado. Haber solicitado una miniatura no acredita que se haya inspeccionado.
- Regresión: comparar storyboard vs resultado, notas exactas y diapositivas fuera del alcance; si una corrección produce deformación o desequilibrio, reiterar optimización y revisión.
- Estados auditables: `Corregido y verificado`, `Pendiente de validación visual`, `No aprobado`. No atribuir puntuaciones visuales a capturas no observadas.

## Casos reales que justifican las reglas
- Diapositiva 7: ejemplo de economía visual sin barra inferior.
- Diapositiva 9: barra inferior y acentos redundantes, retirados; después fue necesario reequilibrar gráficos y cierre. El divisor vertical entre conceptos distintos sí cumple función.
- Diapositiva 10: tres barras superiores y barra inferior redundantes; se retiraron, después fue necesario subir las tres columnas y el cierre. Diferenciar color de flecha y rótulo.
- Diapositiva 11: cajas abiertas construidas por segmentos y flecha de escala incorrecta; corregidas mediante rectángulos nativos y revisión de transformaciones.
Estos ejemplos son **casos de prueba y preferencias del curso**, no dimensiones universales ni aprobación visual automática.

## Foco documental de alta visibilidad y recuperación (2026-11-14)
- Para recortes NIST de tablas y resultados con mucho texto, usar una **jerarquía triple**: (a) recorte oficial íntegro; (b) contorno de alto contraste, preferentemente marino exterior + cian interior como formas editables superpuestas; (c) etiqueta cian nítida que nombre código o relación, fuera de texto sustantivo. Evitar halos sutiles que desaparezcan en zoom de proyección.
- La legibilidad se audita sobre el PNG o PDF renderizado de la diapositiva final, tanto en contacto como individual. Medir precisión de foco, visibilidad, contraste con amarillo/blanco, distancia al código, recorte, solape. Reubicar la fuente y bloques auxiliares si se añade chip; después volver a renderizar.
- Caso clase 4.6: diapositivas 27–31, bloques Gobernar, GV.RM, GV.RM-01, PR.DS-02→10, lectura GV/RM/01. Mejora aplicada: navy 6.5 pt + cyan interior 3 pt + chip cian 14 pt. Números son precedente, no valores absolutos universales.
- Si un editor o conector falla: ejecutar diagnóstico, alternativa estructural y segundo método seguro con comprobaciones en vivo antes de declarar imposibilidad. Distinguir error de parámetro de falta de permisos o conexión.

## Área libre alrededor de códigos — corrección 29–31 (2026-11-14)
Un foco fuerte nunca debe lograrse **a costa de la legibilidad de códigos originales**. En una tabla o extracto PDF, el marco de 6,5 pt y su segundo contorno interior pueden pisar los glifos del código. Si el rectángulo no puede mantener márgenes tipográficos visibles, retirar ambos y adoptar barras laterales paralelas marino/cian, separadas del texto, junto con etiqueta de foco explícita. El área libre y la ausencia de texto ocluido son bloqueantes, incluso si el foco resulta más vistoso con marco.
Caso real: clase 4.6 slides 29–31; códigos `GV.RM-01`, `PR.DS-02`, `PR.DS-10`. Se sustituyeron 4 pares de marcos por 4 pares de barras laterales, se preservaron chips y recortes. Render PDF posterior inspeccionado.

## Ilustraciones oficiales y representación pedagógica (2026-11-14)
- **Recorte de teoría ≠ apoyo gráfico**. Las relaciones (actual vs objetivo, línea base comunitaria, comparaciones) se explican con diagramas visuales editables y simples, basados en la fuente NIST sin hacerlos pasar por imágenes institucionales. Usar ejemplos de la página oficial para materializar conceptos abstractos.
- Para figura escalonada oficial de cuatro Tiers, conservarla íntegra en una slide panorámica y volver a usarla en 4 individuales con **foco por escalón** por marcador externo (barra o callout) evitando colorear, cortar o cubrir letras originales. La parte derecha debe explicar la dimensión de gobernanza y la de gestión de riesgos con mensajes breves.
- Tras generar, inspeccionar tanto contacto completo como ampliación individual. Prestar atención al texto que sobresale del panel de fondo; ampliar margen, reubicar o simplificar. Caso 4.7, paneles de slides 36–39 corregidos tras la primera revisión.

## Aceptación 4.7 — semántica, jerarquía y foco comprobable (2026-11-14)
- **Fuente primaria vs explicación:** una tabla o figura que contiene relaciones visuales oficiales se reproduce auténtica; un pasaje narrativo recortado es material de consulta, NO apoyo gráfico protagonista. Cuando existe solo texto oficial, crear diagrama conceptual nativo basado en NIST, con fuente indicada, sin atribuirlo como figura oficial.
- **Perfil Organizacional:** dos estados visualmente diferenciados (Actual y Objetivo) y su distancia conceptual; no presentar Comunitario como tercer elemento interno equivalente. **Comunitario:** línea base compartida con ejemplos reales de catálogo NIST (manufactura, transporte, ransomware). Evitar confundir el perfil genérico con el Perfil Objetivo de una organización concreta.
- **Figura de Niveles:** panorámica original completa → cada Nivel individual conserva la misma figura intacta, llamada de atención externa inequívoca y contenido propio. Diferenciar en cada slide Gobernanza y Gestión de riesgos; no duplicar las cuatro descripciones en la panorámica.
- **Área de seguridad visual:** indicadores y chips nunca pisan rótulos originales; usar barra externa si no existe margen para marco. Auditar foco, escala, contraste, textos dentro de paneles y salida a PDF antes de aceptación.

## Centrado verificable de texto y contenedor — regresión GV.OC (2026-11-15)
- Para cada etiqueta dentro de una tarjeta, caja o bloque, identificar explícitamente el par `texto ↔ contenedor` mediante los IDs nativos del deck; no inferir emparejamiento solo por cercanía cuando haya varias cajas.
- Calcular límites reales aplicando `size × transform.scaleX/scaleY + transform.translateX/translateY` (en la misma unidad); obtener `cx=x+w/2` y `cy=y+h/2` para texto y contenedor. Inspeccionar `Δx` y `Δy` para cada par. No confundir `contentAlignment=MIDDLE` ni `paragraphStyle.alignment=CENTER` con geometría realmente centrada: ambos son necesarios para el contenido, pero no corrigen una caja de texto desplazada.
- Si la etiqueta es **un único rótulo centrado**, alinear ambos centros geométricos y verificar readback. Los desplazamientos ópticos intencionales solo se permiten tras inspeccionar el render; no corregir silenciosamente un bloque que contiene dos líneas de distinta función (título+subtítulo) centrando cada una contra la caja mayor.
- Tolerancia de diagnóstico: `|Δx| > 2` o `|Δy| > 2` unidades SVG equivalentes en una diapositiva 960×540 obliga a revisión; `≤2` sigue siendo candidato a inspección óptica. Este umbral es orientativo, NO una certificación visual, y debe ajustarse al tamaño del componente.
- Corregir únicamente el objeto causante y preservar `scaleX`/`scaleY`, tamaño, fuente, colores, notas y elementos aprobados. En `updatePageElementTransform` con `applyMode: ABSOLUTE`, reponer expresamente los valores de escala originales: usar `scaleX=1` sobre un elemento de tamaño intrínseco diferente lo deforma. Releer y comprobar centros después de guardar; después observar el render actualizado.
- Caso real: 5.2, diapositiva 46, rótulo «GESTIÓN DE RIESGOS» `Δy=-3,49` → 0; diapositiva 49, «PARTES EXTERNAS» `Δy=+4,01` → 0, corregidos en Google Slides. Diferenciar **centrado geométrico verificado** de **centrado óptico/render validado**.

## Regresión 5.2 — jerarquía GV.OC, márgenes y conectores (2026-11-15)
- **Jerarquía normativa:** Gobernar (GV) → categoría «Contexto Organizativo (GV.OC)» → subcategorías «GV.OC-01…05». Una diapositiva panorámica de categoría debe diferenciarse de las diapositivas de subcategorías por la **composición y el peso visual**, no solo por una palabra en un título. Dentro de la panorámica, las cinco subcategorías tienen **idéntico formato**, sin énfasis arbitrario.
- **Preferencia visual establecida en 5.2:** cuadro de categoría con fondo amarillo tenue y contorno amarillo más grueso; cinco cuadros de subcategorías con fondo blanco y contorno amarillo de Gobernar. La etiqueta interna «GV.OC» y la modificación manual del usuario prevalecen sobre propuestas previas de añadir títulos o barras; no restaurar elementos eliminados por el usuario sin petición expresa. Respetar el resto de la identidad del máster (Inter, azul marino y cian).
- **Margen real del contenido:** medir la distancia desde los límites transformados de la caja de texto hasta cada borde interior del contenedor. Un objeto que apenas cabe geométricamente NO garantiza que sus glifos y líneas quepan; considerar padding propio de la caja, interlineado y render. Caso 5.2 slide 45: el texto terminaba a 4 unidades del borde inferior y 5 del derecho; se reajustó su caja a x=106, y=248, ancho=330, alto=188 para ganar márgenes nominales, **pero comprobar de nuevo wrapping y altura efectiva tras reducir ancho**. Evitar arreglar un margen creando desbordamiento de texto.
- **Conectores nativos:** para relaciones entre nodos, preferir `createLine` + `updateLineProperties` en vez de glifos «→», «↗» o «↘», y verificar la orientación concreta `startArrow/endArrow`, el inicio y final reales, y la ausencia de cruces con etiquetas. Caso 5.2 slide 50: dos relaciones independientes desde Tecnología y Proveedores hacia Organización; el anclaje visible debe llegar perceptiblemente a la caja receptora, no solo existir en la API.
- **Inclusión ≠ causalidad:** en GV.OC-03, privacidad y libertades civiles son requisitos aplicables **incluidos** entre obligaciones relevantes, no una consecuencia causal de «Requisitos». Si se usa la etiqueta «INCLUYE», las conexiones y agrupación deben expresar pertenencia, sin flechas que confundan el sentido semántico.
- **Partes interesadas:** las líneas de GV.OC-02 deben comunicar relaciones reales entre las cajas de grupos internos/externos y Organización; líneas aisladas que terminan en el vacío se consideran falla, aunque sean nativas.
- **Estados separados:** tras actualizar Google Slides, registrar `estructura/propiedades verificadas` solo después de lectura de vuelta; `render comprobado` requiere observar la imagen actual, no solo obtener un enlace a miniatura. No marcar clase aprobada sin aceptación explícita.

## Protocolo transversal de diseño preventivo → implementación → auditoría (2026-11-15)
**Regla de precedencia:** todos los criterios refinados se aplican en los TRES momentos, no solamente después de un error. Ninguna fase puede dispensar a la siguiente; un gráfico correcto aisladamente puede fallar por su relación con el resto de la diapositiva. Usar siempre el último estado nativo, incluidas las ediciones manuales del usuario.

### A. ANTES DE DISEÑAR (diseño como sistema)
1. **Inspección de fuentes:** abrir máster, clase viva, figuras oficiales NIST, narración, estado de aprobación y últimas decisiones manuales. Separar objeto protegido, objeto editable y elemento propuesto.
2. **Jerarquía y semántica:** establecer función → categoría → subcategorías; definir función didáctica, jerarquía, color NIST, relación lógica y representación precisa de cada objeto. Diferenciar clasificación, pertenencia, dependencia, comunicación y causalidad. No inventar causalidad ni cambiar textos oficiales.
3. **Composición global primero:** definir área útil, columnas, cajas principales, centros ópticos, balance de masa, margen exterior, línea base de encabezados, simetría deseada, secuencia de lectura y ritmo entre slides. Evaluar la composición en relación con el **cuadro descriptivo izquierdo, título, otros paneles y espacio blanco**, no solo cada gráfico aislado.
4. **Geometría explícita del storyboard:** planificar por elemento coordenadas, dimensiones, límites, pares texto/contenedor, anchos de línea, flechas (inicio/fin/sentido), distancias entre nodos, longitudes de conexiones, separación texto-borde y márgenes izquierdo/derecho/superior/inferior. En layouts de simetría definir ejes, distancias invariantes y tolerancias antes de crear.
5. **Tipografía preflight:** prever wrapping real, ancho útil tras padding, interlineado, tamaño mínimo legible, énfasis y etiquetas largas (p. ej., ORGANIZACIÓN). No depender de centrado geométrico cuando el texto se corta o se divide de modo indeseado.
6. **Puerta de maqueta:** mostrar esquema SVG 16:9 cuando proceda, con los ELEMENTOS y sus relaciones exactas; auditar densidad, jerarquía, redundancia, equilibrio y fuente antes de construir. El usuario puede modificar el diseño: su última edición prevalece sobre esta maqueta.

### B. DURANTE LA IMPLEMENTACIÓN (control invariante)
1. Construir en Slides con componentes nativos editables conservando IDs, escalas, colores, paleta y notas. Aplicar la geometría aprobada **al conjunto completo**, no ajustar un nodo olvidando su contexto.
2. Tras cada mutación de posición o tamaño, recalcular y verificar dependencias: texto↔contenedor; flechas↔nodos; longitud de líneas equivalentes; distancia de rótulos↔cajas; simetría superior/inferior; centro del conjunto↔cuadro izquierdo; cobertura y orden de lectura.
3. **Simetría por relaciones, no por intuición:** si dos líneas deben medir lo mismo, fijar sus extremos y exigir longitudes iguales (o una diferencia expresamente justificada). Caso GV.OC-02: cuatro conexiones de 36 unidades, dos arriba y dos abajo; desplazamiento del nodo ORGANIZACIÓN de 9 unidades para equilibrarlas. Diferenciar longitud, orientación y punto de llegada; comprobar el render.
4. **Alineación contextual:** evaluar el centro vertical del gráfico derecho contra el centro vertical del cuadro izquierdo. En GV.OC-05, mover 21 unidades el conjunto de título, dos dependencias, organización y flechas conservó sus relaciones y dejó el centro de las fuentes en 313,69 frente a 313,50 del cuadro izquierdo. No aplicar ese desplazamiento como valor fijo en otras clases.
5. **Identidad compartida:** nodos del mismo nivel, mismo color de borde, grosor, relleno, tipografía, radio y tamaño salvo razón explícita. Caso GV.OC-05: Tecnología y Proveedores deben usar el mismo tratamiento cian; nodos de función/categoría/subcategoría usan jerarquías acordadas.
6. **Conexiones:** usar líneas nativas editables con puntos de inicio/fin efectivos, sentido correcto y terminaciones visualmente conectadas. Líneas que llegan a un nodo pero tienen inclinaciones o longitudes arbitrariamente distintas necesitan justificación o rediseño.
7. **Control de wrapping:** cualquier reducción de ancho, aumento de tamaño, cambio de fuente o reposición exige comprobar el texto dentro del contenedor; si ORGANIZACIÓN se divide en «ORGANIZACIÓ / N», falla de diseño aunque las cajas estén centradas.
8. Preservar integridad de títulos, contenido oficial, notas, láminas aprobadas y modificación manual más reciente; no restaurar elementos eliminados por el usuario.

### C. AUDITORÍA POSTIMPLEMENTACIÓN (independiente)
1. **Semántica:** fuente NIST, categoría/subcategoría, exactitud de relaciones, cobertura didáctica, narración↔pantalla, redundancia y no mezclar causalidad/inclusión/dependencia.
2. **Identidad y jerarquía:** plantilla, paleta, grosor/bordes, uso funcional de amarillo GV, equivalencia entre hermanos, diferencia entre padre/hijos y consistencia de familia entre slides.
3. **Tipografía y legibilidad:** glifos completos y no cortados, saltos de línea apropiados, altura de bloque, padding, 4 márgenes, contraste, fuente y consistencia de tamaños para pares equivalentes.
4. **Alineación local:** comparar centros texto–caja usando tamaño transformado, revisar CENTER/MIDDLE y centro óptico real; registrar Δx/Δy. Para varios niveles de texto evaluar conjunto jerárquico, no centrar cada etiqueta al mismo punto.
5. **Composición contextual:** comparar ejes y balances de TODOS los objetos, el conjunto derecho con el cuadro izquierdo y los márgenes del lienzo; examinar encabezados, intervalos y simetría espacial. Medir conectores iguales: sus longitudes, puntos y orientación; no basta con que existan cuatro líneas.
6. **Evidencia renderizada:** observar de verdad cada slide a tamaño de presentación y la secuencia en contacto; un URL de miniatura o lectura API NO acredita inspección óptica. Volver a renderizar tras cambios, verificar desbordes, ocultamientos, conexiones, simetría y jerarquía.
7. **Regresión:** confirmar IDs, notas, orden, estilo de elementos hermanos, slides no afectadas y que la solución no reintroduce errores previos. Reportar resultados por criterio y severidad, indicando verificado, pendiente o error; no asignar aprobación sin aceptación del usuario.

### Matriz de criterios obligatorios y sus tres evidencias
| Criterio | Antes de diseñar | Implementación | Auditoría |
|---|---|---|---|
| Fuente y precisión NIST | inventario oficial y significado | texto fiel, diagrama semántico | cotejo de enunciados y relaciones |
| Jerarquía y color | niveles/roles, paleta funcional | identidad de padre/hijos y pares | contraste jerárquico sin equivalencias falsas |
| Composición global | ejes, áreas y centro con cuadro izquierdo | posicionar conjunto, no piezas aisladas | balance contextual de toda la slide |
| Simetría/espaciado | distancias y longitudes planeadas | invariantes y extremos medidos | comparación de distancias arriba/abajo |
| Conectores | nodos, extremos, sentido, anclajes | líneas nativas con punta correcta | longitud, orientación y llegada real |
| Texto y márgenes | estimación de wrapping y padding | ajustar contenedor/estilo sin clipping | inspección de glifos, márgenes y líneas |
| Centrado local | texto↔caja identificado | transformaciones y CENTER/MIDDLE | Δx/Δy y centro óptico |
| Editabilidad y notas | objetos protegidos, fuente maestra | shapes/líneas y notas preservadas | lectura nativa y regresión |
| Coherencia entre slides | familia, ritmo y densidad | replicar reglas por función | revisión de todas las slides y redundancia |
| Calidad evidencial | planificar render observable | extraer render actualizado | separar API vs inspección visual y aprobación |
**Bloqueo:** si un criterio estructural o semántico falla en diseño, no pasar a implementación; si falla en implementación, no proclamar auditoría superada; si no se puede inspeccionar el render, declarar QA visual pendiente.

## Auditoría dual y control de representación conceptual — 2026-11-16
La auditoría visual general y la de **representación conceptual** se ejecutan **tanto en la propuesta como tras cada implementación/corrección**. Mostrar tabla con «elemento», «idea pretendida», «lectura del icono sin etiqueta», «riesgo de confusión», «nota 0–10 con un decimal» y «corrección», y puntuación promedio. Evaluar nodos y flechas/relaciones como unidades semánticas; una conexión que solo sugiere transmisión no prueba dependencia.
Umbrales orientativos de representación: ≥9,5 inequívoca; 9,0–9,4 clara; 8,0–8,9 requiere etiqueta; 7,0–7,9 ambigua; <7 incorrecta. Puerta de aprobación: promedio ≥9,0 y cada símbolo principal ≥8,5; no proclamar «aprobado» basándose únicamente en el promedio general.
En paralelo auditar precisión NIST, claridad, calidad visual, distribución, proporciones, geometría, jerarquía, paleta, tipografía, legibilidad, utilidad pedagógica y **ausencia de redundancia**. Separar *calidad prevista en la maqueta* de *calidad observada del render*. Evidenciar la revisión de la captura/render real; los metadatos de miniatura, la exportación por sí sola o el readback API no prueban ausencia de clipping, superposición ni calidad óptica.
**Alineación de rótulos hermanos:** definir misma coordenada de inicio de texto, misma altura de recuadro, `contentAlignment=MIDDLE`, alineación de párrafo coherente y baseline/centro óptico verificados sobre render. Con rótulos largos como «SERVICIOS CRÍTICOS» calcular ancho útil y wrapping; jamás aceptar saltos de línea involuntarios ni compensar automáticamente con reducciones excesivas de fuente.
**Regresión conceptual por slides 48–49:** evitar iconos genéricos que sugieran otro dominio; escudo/candado ≠ privacidad específica; apretón de manos ≠ contrato formal firmado; servidor ≠ criticidad por sí mismo; engranaje ≠ capacidades de forma inequívoca. Preservar símbolos validados por el usuario: contrato firmado, privacidad como ojo con restricción, personas + diálogo para libertades civiles, Capacidades como cuadrado con check. Comparar cambios con decisiones congeladas y prohibir regresiones.

## Patrón gráfico aprobado — foco único y flechas a cajas breves (2026-11-16)
Regla para diapositivas conceptuales con UN objeto central y varias acciones o relaciones: usar un solo gráfico protagonista inequívocamente identificado, con flechas nativas que parten de él hacia cajas de texto corto (verbo y complemento conciso). El gráfico debe hacer explícito QUÉ se caracteriza o gestiona; evitar lupa, estrella, check, documento o tendencia ascendente genéricos si no transmiten la identidad del objeto. Evitar párrafos, ejemplos y adornos en las cajas; desarrollar el significado en la narración. Las flechas representan relaciones reales, no secuencia temporal, aprobación ni causalidad inventadas. Alinear simétricamente ramas, conectores y cajas, con márgenes suficientes, sin clipping, y balancear el conjunto frente a la columna NIST izquierda. Mantener Inter, paleta del curso, figuras oficiales intactas y objetos editables.
Referencia editorial aprobada: GV.RM-07, diapositiva 59: protagonista «OPORTUNIDAD ESTRATÉGICA», ramas «CARACTERIZAR — Beneficios y condiciones» e «INCLUIR — En la discusión de riesgos». La regla es preferente SOLO cuando la semántica lo justifica: no sustituye figuras oficiales NIST, jerarquías, cronologías, comparaciones u otros gráficos que requieran relaciones diferentes.
Puertas obligatorias: (1) planificar foco, etiquetas, sentido semántico de flechas y simetría; (2) implementar con objetos y conexiones nativas, conservar texto oficial y notas; (3) auditar cada símbolo/relación y la composición, texto, desbordes y render real observado. Las dos auditorías independientes siguen obligatorias. Aprobación de propuesta no equivale a aprobación de la slide o de la clase.

## Checklist de cobertura auditora y bloqueo por criterio — 2026-11-16
El inventario anterior es **acumulativo**: estas familias se examinan en su totalidad, nunca como selección discrecional. Registrar matriz con columnas `criterio_id | fase (diseño/implementación/post-render) | alcance (objeto/diagrama/slide/clase) | aplica/justificación | evidencia | nota | estado | reparación`.

| ID | Criterio mínimo obligatorio | Evidencia/prueba de aprobación |
|---|---|---|
| C01 | Exactitud NIST | confrontar contenido y alcance con texto oficial; distinguir norma de ejemplos |
| C02 | Objeto protagonista y adecuación del símbolo | qué representa exactamente, ¿se reconoce sin rótulo? alternativas de lectura |
| C03 | Integridad morfológica del icono | contorno/silueta completa, proporciones, unión de piezas y detalles distintivos, a tamaño real; revisar icono aislado y en contexto |
| C04 | Semántica individual de cada relación | tipo real de vínculo, origen/destino y dirección, ausencia de causalidad o secuencia inventadas |
| C05 | Calidad de dibujo/asset | nitidez, no fragmentación, stroke consistente, encaje en estilo aprobado |
| C06 | Composición global/foco visual | equilibrio respecto del cuadro NIST, jerarquía y lectura de primer vistazo |
| C07 | Geometría y simetría | centros locales/globales, distancias, longitudes iguales cuando corresponde, límites reales |
| C08 | Conectores | punta, anclajes, orden de dibujo, espacio entre extremos y cajas, sin atraviesos |
| C09 | Texto/legibilidad | márgenes, interlineado, alineación, tamaño, wrapping y clipping observado |
| C10 | Paleta e identidad | colores permitidos y usos coherentes; figura oficial preservada |
| C11 | Narración y correspondencia | notes íntegramente conservadas o editadas con autorización; guion y gráfico alineados |
| C12 | Utilidad didáctica | idea central reconocible y sin explicaciones superfluas |
| C13 | Ausencia de redundancia | puntuar independiente repeticiones entre slide, gráfico, narración y slides cercanas |
| C14 | Editabilidad y persistencia | IDs, texto y objetos nativos, lectura de vuelta, sin alterar slides ajenas |
| C15 | Fidelidad maqueta→implementación | comparar forma, proporciones, sentido, textos, cromática y composición con diseño aprobado |
| C16 | Render real + regresión | extraer render actualizado, **abrir/ver los píxeles** a escala de presentación, repetir tras cada corrección |
| C17 | Coherencia de clase y decisiones congeladas | continuidad con slides vecinas, preservar decisiones manuales y aprobaciones explícitas |

**Obligatoriedad:** para todas las filas aplicables, prueba con resultado. Si una fila no aplica, anotar fundamento comprobable. Si un fallo es crítico (falsedad NIST, icono irrecognoscible, flecha invertida, texto cortado, render no examinado), bloquear aprobación aunque los promedios sean altos. Evaluar por símbolo, no solo por conjunto. La escala decimal no es prueba: anclar cada nota a observaciones del render o hechos concretos.

**Momento:** propuesta/revisión (C01–C13,C15 según aplique), construcción/readback (C01–C15,C17), render posterior (C01–C17); cada edición o feedback dispara revalidación de criterios afectados y regresión del conjunto antes de cualquier entrega. Si hay imposibilidad de render, estado `BLOCKED: QA visual pendiente` sin simular observación.

**Caso de calibración GV.RM-07:** la versión inicial de bombilla formada por círculo+rectángulos recibió puntajes conceptuales altos pese a no parecer claramente una bombilla. Eso viola C02/C03/C15/C16; la bombilla debe identificarse sin leer «OPORTUNIDAD ESTRATÉGICA» y tener silueta, cuello y casquillo distinguibles. Se debe reprobar cualquier repetición de ese resultado. En auditoría, verificar primero cada icono aislado, después el diagrama y por último la slide completa. La puntuación por rama/flecha no compensa el fracaso del foco.
