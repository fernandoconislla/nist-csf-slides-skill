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
