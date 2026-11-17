# Historial de cambios

## Maquetas SVG visibles y redundancia funcional — 2026-11-14

- Creada `references/editorial-redundancy-svg.md` con la decisión aprobada de no penalizar automáticamente la apertura panorámica cuando cumple una función didáctica distinta del desarrollo.
- Incorporadas instrucciones a `SKILL.md`, las siete skills especializadas y `references/visual-composition.md`: narración completa auditada → pantalla → storyboard → maquetas SVG 16:9 **visibles** → aprobación editorial → construcción nativa → QA y aceptación visual.
- Precisado uso de figuras institucionales auténticas y pertinencia visual (imagen de procedimiento solo cuando se explica el procedimiento). Las maquetas muestran marcadores de activos, no pseudofiguras NIST.
- Añadidos casos RED-01–03, SVG-01–03 y STATE-01–02 en tests; registro en `FEEDBACK.md`.
- **Estado:** actualización documental completada. Pruebas contra la clase 4.4 y render visual final aún pendientes. Ningún cambio a Google Sheets o Slides en esta operación.


## Diseño preventivo y QA geométrico — 2026-11-14

- Añadida `references/visual-composition.md` con puertas obligatorias **prevención → construcción controlada → QA visual/estructural y regresión**.
- Actualizadas las skills raíz, plantilla, lección, construcción, producción y mejora para evitar decoración gratuita, planificar distribución antes de construir y revisar transformaciones de flechas/contornos.
- Nuevos casos de regresión `VIS-01`–`VIS-09`: economía visual, recálculo de espacios, columnas, conectores, contornos, color, preservación de notas y verificación visual.
- Registrada evidencia de las diapositivas 7, 9, 10 y 11 en `FEEDBACK.md`. Las pruebas de regeneración futura no se declaran ejecutadas.

## Corrección del flujo de clases — 2026-11-13
- Requisito de aprobación previa: **propuesta completa (narración + pantalla + diseño) → auditoría → revisión y aprobación del usuario → construcción**.
- Tras aprobación, añadir las diapositivas al **Google Slides acumulativo existente** del curso NIST CSF 2.0, no crear un deck nuevo por clase.
- Clase 4.1 aprobada inmutable y plantilla maestra de referencia inmutable.
- La presentación separada generada por error para 4.2 se considera borrador no aprobado y no sustituye el archivo acumulativo.
- Auditoría de narración, composición y no regresión después de añadir cada clase.


## Consolidación de clase aprobada 4.1 — 2026-11-13
- Incorporado como caso de regresión el resultado aprobado de «Introducción al NIST CSF 2.0», sin alterar el Google Slides.
- Identidad de portada del curso preservada; dos líneas semánticas, segunda completa en celeste, sin cortar «NIST CSF 2.0».
- Paleta del deck maestro exacta: #102B46 / #00B8D9 / #FFFFFF; fuente Inter; elementos de desarrollo equilibrados y verificados.
- Prioridad de recursos oficiales verificables en diapositivas específicas, con excepción expresa de la portada de clase.
- Figuras técnicas no se adelantan si su significado corresponde a clases posteriores; evolución editable y propósitos sin falsa secuencia.
- En cada regeneración, sustituir íntegramente las notas y realizar lectura de vuelta literal; bloquear aprobación si hay restos o duplicaciones.
- Entrega en Google Slides nativo; no producir PDF/PPTX no solicitados. Respetar el estado de aprobación y las ediciones manuales.
- Se incorporan pruebas de regresión y registro del feedback aprobado.


## Course Curriculum Builder 0.5.0 — 2026-11-13
- Regla obligatoria de granularidad competitiva: en Udemy la estructura pública muestra secciones y clases; los puntos de contenido del sistema son internos.
- Identificar brechas de visibilidad frente a las clases publicadas por la competencia cuando se proporcionen URLs.
- Evaluar la promoción de puntos a clases por autonomía didáctica, profundidad, interés y valor visible; sin microclases ni copia mecánica.
- Mantener trazabilidad normativa, promesa educativa y auditoría con nuevo criterio 15.
- No modificar temarios existentes sin aprobación de los cambios propuestos.


## Course Curriculum Builder 0.4.0 — 2026-11-13
- Añadido análisis competitivo **opcional** a partir de enlaces de cursos de Udemy aportados por el usuario.
- Matriz de evidencia pública, comparación curricular y oportunidades de diferenciación sin copiar temarios.
- Jerarquía: fuente oficial obligatoria y decisiones aprobadas por el usuario prevalecen sobre la competencia.
- Quinta pestaña opcional `Análisis competitivo`, manteniendo las cuatro pestañas base.
- Nuevo criterio 14 de auditoría competitiva y enlaces iniciales de referencia para NIST CSF 2.0.


## Course Class Producer 0.1.0 — 2026-11-13
- Creada la skill orquestadora `skills/course-class-producer/SKILL.md`.
- Entrada mínima: clase por nombre/ID en el contexto de un curso existente.
- Fuente de verdad: Google Sheets vigente, incluidos cambios del usuario; secuencia obligatoria hasta Slides final.
- Puertas de control para narración completa, paleta/template/estilo aprobados, storyboard, gráficos, notas y auditoría.
- Manifiesto de estados `references/run-manifest.md` y 10 casos de prueba.
- Prohibido declarar producción completa cuando no se haya verificado la incorporación real de notas.

## Course Slide Builder 0.1.0 — 2026-11-13
- Creada `skills/course-slide-builder/SKILL.md` para transformar guion auditado en diapositivas Google Slides 16:9 editables.
- Planificador de unidades visuales: sin imponer una slide por punto curricular.
- Correspondencia obligatoria Puntos → Narración → Slides y Pantalla → Narración.
- Integración de plantillas y estilo de ilustración aprobados; uso fiel de recursos oficiales.
- Narración por diapositiva en notas del presentador, con verificación; audio reproducible es fase independiente.
- Plantilla `references/slide-plan-template.md`, ocho pruebas de regresión y auditoría integral.


## Course Image Style Builder 0.1.0 — 2026-11-13
- Nueva skill `skills/course-image-style-builder/SKILL.md`.
- Análisis exhaustivo de referencias visuales: composición, geometría, perspectiva, profundidad, iluminación, materiales, iconografía y espacios negativos.
- Integración de la paleta aprobada con precedencia sobre los colores de la imagen de referencia.
- Salida: `course-image-style.md` por curso con prompt maestro y reglas de aplicación para cada recurso.
- Aprobación obligatoria del sistema visual y verificación con dos conceptos distintos cuando exista generador disponible.
- Plantilla de salida `references/output-template.md` y seis casos de prueba definidos en `tests/cases.md`.


## Course Skill Improver 0.1.0 — 2026-11-13
- Creada `skills/course-skill-improver/SKILL.md`, centrada en aprendizaje por feedback sin reentrenamiento.
- Clasificación de cambios locales, preferencias contextuales y reglas permanentes.
- Flujo: comparar → diagnosticar → proponer diff → aprobar → versionar → probar regresiones.
- Archivos `FEEDBACK.md`, `references/feedback-record.md` y `tests/cases.md`.
- Prohibición de modificar reglas permanentes sin aprobación explícita y protección de datos en repositorio público.


## Course Lesson Builder 0.2.0 — 2026-11-13
- Cobertura completa y obligatoria de todos los puntos de contenido de la clase en la narración.
- Orden obligatorio: puntos curriculares → narración auditada → texto en pantalla derivado de la narración.
- El texto en pantalla queda íntegramente explicado por la narración, pero la narración no necesita figurar completa en pantalla.
- Dos matrices: puntos → segmentos de narración y texto visible → segmentos de narración.
- Auditoría obligatoria de cobertura, correspondencia semántica y calidad didáctica; hallazgos críticos bloquean aprobación.
- Entregable conjunto: narración y propuesta de textos en pantalla, sin generar Google Slides por defecto.


## Course Curriculum Builder 0.3.0 — 2026-11-13
- Cobertura integral obligatoria de todas las referencias utilizadas como base curricular: sin resúmenes sustitutivos ni omisiones.
- Inventario exhaustivo de unidades formativas de las fuentes, incluidos apartados, tablas, figuras y prácticas pertinentes.
- Nueva matriz bidireccional de trazabilidad fuente → sección/clase/punto de contenido.
- Auditoría exhaustiva de cobertura, no por muestreo; omisiones críticas bloquean declarar el temario completo.
- El temario puede ampliarse para sostener el alcance y debe informar restricciones de acceso o duración.
- El Google Sheets pasa a cuatro pestañas: Temario, Puntos de contenido, Matriz de cobertura y Auditoría.


## Course Lesson Builder 0.1.0 — 2026-11-13
- Nueva skill modular `skills/course-lesson-builder/SKILL.md`.
- Entrada prioritaria: clase concreta, puntos de contenido y contexto actual del Google Sheets.
- Primera salida: guion de narración docente completo, natural, riguroso y listo para revisión.
- Mapa de cobertura, estimación de duración, fuentes y auditoría obligatoria con 13 criterios.
- Extensible en el futuro a texto en pantalla, prácticas y recursos, sin generarlos por defecto.


## Course Curriculum Builder 0.2.0 — 2026-11-13
- Auditoría obligatoria tanto de borrador como de entrega final.
- 13 criterios independientes: técnica, cobertura, pedagogía, títulos, conversión, SEO, móvil, viabilidad y fuentes.
- Nueva pestaña `Auditoría` en Google Sheets, con hallazgos, evidencia, severidad y ajustes.
- Resumen de auditoría incluido siempre en la respuesta; sin puntuaciones inventadas.

## Course Curriculum Builder 0.1.0 — 2026-11-13
- Nueva skill `skills/course-curriculum-builder/SKILL.md` para temarios editables de tres niveles.
- Criterios editoriales para títulos claros, didácticos y orientados a conversión honesta.

## 0.2.0 — 2026-11-13
- Nueva skill modular `skills/course-slide-template/SKILL.md` para futuros cursos Udemy.
- Interpretación del tema como paso obligatorio antes de recomendar identidad visual.
- Paleta base: color principal oscuro potente, secundario luminoso afín, blanco puro.
- Propuesta de tipografía contextual, sin imponer Inter.
- Estructura fija: apertura de clase con elemento gráfico y título; desarrollo blanco con título y barra separadora.
- Vista previa y **aprobación explícita antes de generar** la plantilla.
- Estética tech con presencia visual, evitando sobrecarga, saturación y mala legibilidad.

## 0.1.0 — 2026-11-13
- Estructura inicial de la skill NIST CSF.
- Prompt de ilustración reconstruido, pendiente de validación literal.
- Reglas de composición, precisión NIST y auditoría; enlaces de referencia.
## Figuras oficiales pequeñas en introducción panorámica — 2026-11-14

- Corregida la slide 02 de clase 4.4: tres imágenes oficiales pequeñas (Núcleo, Perfiles y Tiers), no números decorativos.
- Creada propuesta V4 en `proposals/class-4.4-componentes-del-marco-v4.md`.
- Actualizados skill principal, subskills pertinentes, referencias editoriales/visuales, feedback y estado; agregados casos de prueba OFF-01–04.
- Norma y propuesta escritas, **pruebas visuales/activos definitivos/maquetas SVG y aprobación editorial pendientes**. No se modificaron Google Slides ni casillas de Sheets.

## 2026-11-14 — Resiliencia operativa y foco documental fuerte
- Ejecutada corrección sobre slides 27–31 de 4.6 en el deck nativo: doble contorno marino (6,5 pt) + cian (3 pt) y chips cian explicativos. La fuente NIST auténtica y notas se preservan. Revisión Slides `QtyPp6rt-svPiQ`; export PDF de 31 páginas, inspección visual de cinco páginas y contacto.
- Incorporada regla de reintentos seguros (hasta 3 rutas técnicas distintas con detección de efectos parciales, sin mutaciones ciegas) en raíz, builder, producer, improver y referencia visual.
- Añadidos casos RETRY/FOCUS y criterio auditor independiente «Fuerza del foco visual».
- **No marcar clase 4.6 aprobada ni grabada sin aceptación expresa.**

## 2026-11-14 — Corregida oclusión de focos fuertes en 4.6
- Slides 29–31: reemplazados 4 pares de marcos marino/cian por 4 pares de marcadores laterales editables, sin invadir códigos NIST. Se preservan chips y notas.
- Se ejecutó el protocolo de reintento tras revisión de Slides desactualizada: lectura de nuevo revisionId y segunda escritura exitosa.
- Render PDF actualizado inspeccionado; añadida regla de área tipográfica libre y pruebas OCC-01..03 / RETRY-04. Estado no aprobado.

## 2026-11-14 — Aprobación clase 4.7 y consolidación de skills
- **Google Sheets Temario G17=TRUE; H17=FALSE**, comprobado por lectura de vuelta tras aceptación expresa. La clase 4.7 queda aprobada y no grabada.
- Presentación nativa conservada con **40 diapositivas**, 4.7 en páginas 32–40, nueve narraciones; revisión verificada del deck antes de cerrar: VnwO_6-31Cb71Q.
- Consolidación de 8 skills especializadas y raíz: diferencia entre figura oficial y recorte de texto, Perfil Comunitario independiente, panorama vs una slide por Tier, tabla 2 gobernanza+gestión, foco sin ocultar letras, no-duplicidad de contenidos, matriz de estado aprobado/grabado y protocolo de reintento.
- Regresión 4.7 documentada y readback de GitHub requerido; ningún cambio adicional en el deck a raíz de aprobación.


## 2026-11-14 — Actualización de skills: aprobación de clase y foco visual de referencia

- Regla explícita y accionable de **cierre tras aprobación de clase** añadida en `SKILL.md` y `course-class-producer`: sincronización de `Aprobada` en Sheets, preservación de `Grabada`, registro en `PROJECT_STATE.md`, lectura de vuelta, estado parcial ante errores y ninguna producción automática de la clase siguiente.
- `course-skill-improver` registra el aprendizaje de la aprobación 5.1 y la corrección de alineación del foco 19→42 sobre imágenes base con geometrías diferentes.
- Casos de regresión STATE-APPROVE-01…03 y VIS-REFERENCE-01 añadidos como **definidos, no ejecutados**. El cierre 5.1 fue comprobado antes de esta actualización.


## 2026-11-15 — Regresión de centrado en clase 5.2
- Reparados los objetos nativos de las diapositivas 46 y 49 de la presentación acumulativa: «GESTIÓN DE RIESGOS» y «PARTES EXTERNAS» quedaron con diferencia vertical geométrica `Δy=0` respecto a sus cajas respectivas, confirmada con lectura de vuelta. No se cambiaron textos normativos ni notas.
- Incorporado protocolo universal de emparejamiento texto–contenedor, cálculo de centros con transformaciones efectivas, distinción de alineación textual vs geométrica vs óptica y conservación de escalas al actualizar transformaciones.
- Actualizados raíz, referencia visual, builder, producer y casos de regresión ALIGN-CONTAINER-01…05. Casos documentados, **no ejecutados como batería automatizada**. Render visual final pendiente; no se declara aprobación de la clase.

## 2026-11-15 — Aprendizajes posteriores de la clase 5.2
- Consolidada la jerarquía categoría GV.OC (fondo amarillo tenue, borde amarillo grueso) frente a subcategorías GV.OC-01…05 (blanco, bordes amarillos iguales), respetando las modificaciones manuales del usuario en la diapositiva 45.
- Registrados riesgos de margen nominal vs. desbordamiento tipográfico después de reducir el ancho de la caja de definición; relaciones de partes interesadas e inclusión de privacidad; y preferencia por conectores nativos con comprobación real de puntos extremos y semántica de flechas.
- Actualizados `SKILL.md`, `course-slide-builder`, `course-class-producer`, `references/visual-composition.md`; añadidos casos de regresión HIER/MANUAL/TEXT/CONNECT/INCLUDE/QA 24–30.
- Evidencia: últimas reparaciones de Google Slides guardadas y releídas con notas preservadas; **render actual no validado visualmente**, casos añadidos pero no ejecutados. La clase 5.2 sigue pendiente de aprobación explícita.

## 2026-11-15 — Modelo de diseño preventivo para TODOS los criterios refinados
- Política transversal: no esperar a la auditoría para detectar problemas visuales. Criterios obligatorios desde **planificación previa**, con invariantes verificables **durante implementación**, y revisión integral **durante auditoría**.
- Actualizada `references/visual-composition.md` con protocolo A/B/C, matriz de 10 familias de criterios y pruebas del contexto global: un gráfico aislado puede estar bien pero mal alineado con el panel izquierdo.
- `course-slide-builder`, `course-class-producer`, raíz y `course-skill-improver` reciben reglas de control geométrico y semántico, prioridad de modificaciones manuales y separación de evidencia API/render.
- Regresión específica de GV.OC-02: cuatro líneas desiguales (27 arriba/45 abajo) → 36/36 al mover 9 unidades el nodo central. Regresión GV.OC-05: composición derecha centrada verticalmente frente al cuadro izquierdo, además de simetría interna.
- Añadidos escenarios PRE-DESIGN/IMPLEMENT/FULL-COMPOSITION/IDENTITY/WRAP/CONNECT/CATEGORY/QA/MANUAL 31–39. **Casos escritos, no ejecutados como batería automatizada.** No se modificaron slides ni el estado de aprobación al actualizar las skills.

## 2026-11-16 — Regla gráfica aprobada: un protagonista y cajas breves
- Aprendizaje de la iteración GV.RM-07, slide 59: un solo gráfico central reconocible, flechas hacia cajas de texto corto, sin párrafos ni iconos secundarios que compitan con el foco. Objeto explícito («OPORTUNIDAD ESTRATÉGICA») y dos ramas («CARACTERIZAR» / «INCLUIR»).
- Actualizados la skill raíz, referencia de composición y skills course-slide-builder, course-class-producer y course-skill-improver; se conserva el protocolo de tres puertas y las auditorías conceptual y visual independientes.
- Excepciones: no imponer este patrón a figuras oficiales NIST, jerarquías, comparaciones o secuencias para las que resulte incorrecto.
- Añadidos casos de regresión 44–47. Son pruebas documentadas, no una batería automatizada ejecutada. Las modificaciones de skills no alteran Google Slides ni implican aprobación final de clase.

## 2026-11-16 — Cero omisiones y evaluación correcta de cada criterio
- Reforzado protocolo integral de auditoría ante fallo de reconocimiento de bombilla GV.RM-07: inventario obligatorio C01–C17, matriz por fase/objeto con evidencia, estados PASS/FAIL/BLOCKED/NO APLICA y bloqueo por fallo crítico sin compensación por promedios.
- Eventos de revalidación: propuesta/revisión SVG, aprobación editorial, cada cambio en Slides, final de slide y clase, modificaciones manuales, observación del usuario o cambio de criterios aplicables.
- Añadidas pruebas inequívocas de **reconocimiento sin etiqueta, integridad de silueta, escala real, fidelidad maqueta-render**, además del control de render observado y regresión.
- Root, referencia, builder, producer e improver sincronizados; casos de regresión 48–54 añadidos pero NO ejecutados automáticamente. Ninguna diapositiva fue modificada por esta actualización.
