# Producción de clases · reglas vigentes desde 2026-11-18

Esta referencia concentra los parámetros operativos del curso NIST CSF 2.0. Prevalece para los puntos que actualiza. Los precedentes históricos conservan su valor como evidencia de los problemas que resolvieron. Aplicar los requisitos C01–C17 de [composición visual](visual-composition.md) junto con estas reglas.

## Elegir un gráfico reconocible

- Partir del enunciado y la narración: **qué se hace, sobre qué y qué detalle deja ver la acción**. Entre representaciones fieles, elegir la que se reconozca más rápido sin rótulos. Equipo, documento, interfaz y escena se evalúan con el mismo criterio.
- Usar un objeto protagonista; una relación puede integrar piezas secundarias si aclaran la acción. Un contenedor pertenece al objeto o facilita su lectura. Retirarlo si aporta solo decoración. Representar objetos según su naturaleza: una credencial digital se reconoce como dato o certificado, y una firma criptográfica como parte de un mensaje digital.
- Tomar la decisión sobre cada rótulo durante el diseño. Probar la versión sin rótulos **internamente**. Integrar texto breve solo si resuelve una ambigüedad. Mostrar al usuario una sola versión final por gráfico.
- Puntuar el **acabado premium** independientemente de la claridad conceptual: silueta reconocible, trazos y proporciones precisos, jerarquía, densidad y aprovechamiento del espacio, contraste y legibilidad en el render. Un panel genérico, bordes de adorno o formas inconexas requieren rediseño aunque encajen en el marco.

## Plantilla determinista de categoría y subcategoría

Las coordenadas parten de la esquina superior izquierda de una diapositiva de 960 × 540 px. Convertir usando el tamaño real de página. La comprobación geométrica cuenta con tolerancia de **±1 px**. En la página estándar de 12 192 000 × 6 858 000 EMU, **1 px = 12 700 EMU**.

| Elemento | X, Y | Ancho × alto | Estilo |
|---|---|---|---|
| Tarjeta izquierda | 74, 173 | 395 × 281 | Centro Y = 313,5. Radio de la plantilla. |
| Gráfico de subcategoría | 542, 193 | 320 × 240 | 4:3, centro Y = 313. Escala proporcional dentro de ese marco. |
| Etiqueta de subcategoría | 102, 194 | 153 × 45 | Fondo suave según función. |
| Código de subcategoría | 109, 200 | 139 × 34 | Inter 22 pt, centrado en ambos ejes. |
| Enunciado de subcategoría | 103, 256 | 340 × 178 | Inter 17 pt, alineado arriba y a la izquierda. |
| Código de categoría | 102, 195 | 340 × 44 | Inter 21 pt, alineado arriba y a la izquierda. |
| Enunciado de categoría | 106, 248 | 330 × 186 | Inter 16 pt, alineado arriba y a la izquierda. |
| Cuadrícula de categoría | Columna derecha | Según número de códigos | Centrar el conjunto de recuadros en Y = 313,5 y mantener alineación y ritmos constantes. |

- Categoría: fondo suave y borde de 36 000 EMU (≈2,83 px). Subcategoría: fondo blanco y borde de 16 500 EMU (≈1,30 px). El enunciado deja un margen inferior de al menos 20 px. Probar el enunciado más largo de la clase, corregir sus saltos o proponer una redacción fiel si hace falta.
- Comprobar el **marco** del PNG en Slides y, por separado, los límites visibles del objeto. Corregir el espacio transparente en el SVG cuando el peso o centro óptico se desvíen. Mantener las coordenadas de inserción.

| Función | Borde y recuadros | Fondo de categoría | Fondo de etiqueta |
|---|---|---|---|
| Gobernar (GV) | `#EBBF4A` | `#FFF9E6` | `#FBF3D9` |
| Identificar (ID) | `#4CAED8` | `#EAF5FA` | `#D4ECF6` |
| Proteger (PR) | `#9695E5` | `#F8F7FF` | `#EAE9FB` |

Para funciones aún sin paleta de desarrollo aprobada, tomar como referencia su sector y fila oficiales, derivar tonos suaves y validarlos en la propuesta. El color funcional de las tarjetas es una convención del curso. Preservar las figuras oficiales y los colores de marca del curso: azul marino `#102B46`, celeste `#00B8D9` y blanco.

## Introducciones de función

Usar las diapositivas **87–89** de Identificar como referencia estable del patrón. La aplicación verificada a Proteger está en **117–119**.

1. Portada de función con arte del curso, nombre y subtítulo.
2. Finalidad: figura oficial de las funciones a la izquierda, sector activo resaltado sin tapar su texto, y propósito y alcance a la derecha. Mantener colores, proporciones y etiquetas de la figura auténtica.
3. Panorama: título, breve línea de orientación, tabla con encabezados y todas las categorías de la función, explicación de uso de los códigos y fuente. Usar el recorte auténtico del NIST. Si se juntan encabezado y filas del original, conservar su escala, colores y alineación.

## Maquetas y producción en Slides

La **maqueta de la diapositiva** es 16:9 y se renderiza para aprobación. El **gráfico de apoyo** de una subcategoría tiene SVG maestro 4:3 (`viewBox="0 0 264 198"` o equivalente proporcional) y PNG transparente. Insertar **un solo PNG por gráfico de apoyo**. El SVG se conserva editable en el espacio de trabajo. En la presentación se editan el marco, el título, el enunciado, las etiquetas de la plantilla y las notas. Conservar un activo oficial auténtico en su formato de importación compatible y en el marco que le corresponda. Reemplazar una imagen únicamente dentro del alcance aprobado.

## Lecturas y auditoría

- Consultar el extracto local por código, por ejemplo `referencia_nist_csf_2_0/nucleo/PR.AA.md` en el espacio de trabajo del curso. El índice local incluye secciones, funciones y categorías. Reutilizar el fragmento para guion y auditoría. Abrir el PDF para extraer o verificar una figura, una tabla o un detalle que dependa de la página original. Reutilizar recortes oficiales verificados.
- Reutilizar la skill y las referencias ya consultadas. Leer en vivo el punto curricular, revisión u objeto necesarios. Trabajar sobre la clase activa. Consultar diapositivas cerradas solo cuando el usuario las indique como referencia, con acceso de lectura. La alteración de clases aprobadas requiere alcance expreso. Al agregar páginas, verificar orden anterior con IDs y consultar el contenido de las nuevas.
- Puntuar de 0,0 a 10,0 con un decimal. Mantener auditorías **conceptual** y **visual** independientes, acabado premium explícito y ausencia de redundancia por separado. Cada criterio puntuable aplicable debe superar **9,0**. Con **9,0 o menos**, corregir, volver a renderizar cuando proceda y repetir los controles afectados. Un criterio sin evidencia queda pendiente o bloqueado. Los promedios sirven para resumir.
- En una corrección puntual, auditar lo afectado y la regresión asociada. Al cerrar la clase, verificar la secuencia completa, notas, geometría, render y criterios de ambas auditorías.

## Aprobación y siguiente paso

En cada puerta de revisión, ofrecer **Aprobado** y **Optimizar** como botones cuando la interfaz los admita. Acompañarlos con el siguiente paso concreto. **Aprobado** ejecuta directamente ese paso. **Optimizar** activa la revisión de los criterios afectados. Mantener separadas las aprobaciones de la propuesta, del render o maqueta y del cierre de la clase. En el cierre verificar **Aprobada** en el Temario y `PROJECT_STATE.md` en GitHub. **Grabada** requiere confirmación independiente. La clase siguiente se inicia por solicitud propia.
