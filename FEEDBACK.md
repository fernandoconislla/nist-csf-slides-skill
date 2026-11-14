# Registro de decisiones de producción

## 2026-11-13 · Clase 4.1 NIST CSF 2.0 (aprobada por el usuario)

**Alcance:** reglas reutilizables de Google Slides para las skills de plantilla, narración, slides y producción; decisiones de color y portada específicas del curso NIST CSF.

**Problemas observados y resueltos:** primera portada con corte antinatural en «NIST CSF» / «2.0»; aplicación parcial de la paleta; elementos descentrados; falta de recursos gráficos; uso de ilustraciones genéricas en contenido NIST específico; reiteraciones de narración por `insertText` sin limpieza de notas; entregas PDF/PPTX no solicitadas; auditoría prematura sin inspección suficiente.

**Decisiones aprobadas:** 
- La portada sigue la identidad gráfica estable del curso. Dos líneas: «Introducción al» blanco / «NIST CSF 2.0» íntegra celeste. Conservar imagen protagonista.
- Los contenidos específicos usan recursos oficiales auténticos, sin alterar diagramas; los conceptos abstractos admiten iconos y gráficos editables.
- Diapositiva 3: evolución en línea de tiempo. Diapositiva 4: cuatro propósitos con iconos, sin falsa secuencia obligatoria.
- Google Slides nativo editable como entregable; notas por slide completas y reemplazadas íntegramente en cada regeneración.
- Verificación visual, estructural y narrativa antes de declarar listo; respetar ajustes manuales y el estado de aprobación de una clase.

**Referencia del caso aprobado:** «Clase 4.1 · Introducción al NIST CSF 2.0», cuatro diapositivas, aprobada explícitamente por el usuario el 2026-11-13. Enlace a Google Slides disponible en el contexto de producción; no publicarlo en este archivo sin confirmar su configuración de acceso.

**Prueba:** ver `tests/cases.md`. Cambios de instrucciones verificados en GitHub; las reglas se evaluarán en próximas regeneraciones reales. No asumir mejora ejecutiva probada solo por cambio textual.

## 2026-11-14 · Refinamiento visual NIST CSF 2.0 (diapositivas 7, 9, 10 y 11)

**Solicitud aprobada:** actualizar skills pertinentes para aplicar criterios **antes, durante y después** de generar, no solo como corrección posterior.

**Observaciones:** (a) separadores adicionales sin función en las diapositivas 9 y 10; (b) eliminación posterior dejó huecos que exigieron redistribuir contenido; (c) rectángulos de diapositiva 11 incompletos y flecha deformada por transformaciones; (d) color funcional de ⇄ celeste y rótulo azul marino; (e) miniaturas generadas pero inspección visual no acreditada.

**Causa probable:** contrato preventivo insuficiente y comprobaciones geométricas incompletas; no confundir con causa demostrada. Los desplazamientos exactos fueron correcciones locales.

**Alcance:** principios reutilizables a `references/visual-composition.md`; instrucciones breves en template, lesson, builder, producer y root; regla de aprendizaje en improver; pruebas VIS-01 a VIS-09. Conservar decisiones editoriales y notas aprobadas, sin modificar presentación.

**Validación:** lecturas GitHub y pruebas estáticas de presencia/consistencia; reejecución visual con nueva clase **pendiente**.



## 2026-11-14 · Redundancia funcional y restauración de maquetas SVG — clase 4.4

**Retroalimentación aprobada:** la diapositiva de apertura puede resumir qué es y para qué sirve cada uno de los tres componentes del NIST CSF 2.0, aunque luego las siguientes amplíen la explicación. La repetición es una **orientación pedagógica intencional**, no un defecto sustantivo automáticamente. El usuario recordó el proceso previo de mostrar **maquetas SVG visibles** antes de generar Google Slides.

**Corrección de criterio:** diferenciar repetición léxica, repetición conceptual sin aporte, repetición funcional y anticipación indebida del temario de clases siguientes. Las notas de redundancia antes expuestas (7,1/10 y 8,8/10) fueron juicios editoriales provisionales, no resultados de pruebas ni puntuaciones universales.

**Cambios de reglas:** referencia `references/editorial-redundancy-svg.md`; instrucciones coherentes en la skill raíz, las siete skills especializadas y `references/visual-composition.md`; casos RED/SVG/STATE. Maquetas: narración auditada → texto visible → storyboard → SVG 16:9 visible → aprobación editorial → Google Slides editable → QA renderizado y aceptación visual final.

**Clase 4.4:** propuesta de cinco diapositivas, panorámica de 3–5 minutos, todavía **NO APROBADA / NO GRABADA**. Respetar seis funciones enumeradas y categorías/subcategorías mencionadas sin desarrollarlas. Evitar explicación de tipos de perfiles y tiers reservada a 4.7. Priorizar figuras NIST reales y oportunas.

**Validación:** cambios de GitHub verificables con lectura de vuelta; pruebas estáticas definidas, regresión editorial y visual de la clase 4.4 **pendiente de ejecución**. No se ha modificado el deck acumulativo ni marcado la casilla de aprobación.
