# Composición visual preventiva y validación — NIST CSF 2.0

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
