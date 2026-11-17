# Pruebas de regresión — Course Class Producer

No ejecutadas inicialmente. Ejecutar con un curso real y registrar evidencia.

1. **Clase por ID:** input `3.1`, resolver título y puntos desde Sheet vigente; no confundir sección con clase.
2. **Clase por nombre:** coincidencia única; respetar texto exacto y notas del usuario.
3. **Edición de Sheet:** cambia un punto antes de producir; actualizar narración y relaciones, sin usar copia obsoleta.
4. **Sin template aprobado:** generar narración y storyboard si procede; no construir slides definitivas con una plantilla inventada.
5. **Sin estilo gráfico:** usar activos oficiales/formas nativas cuando proceda; no declarar ilustraciones con prompt maestro no aprobado.
6. **Narración extensa:** agregar slides sin recortar puntos para cumplir una duración arbitraria.
7. **Notas no editables:** registrar bloqueo; no declarar producción completa.
8. **Salida completa:** verificar URL real, 16:9, cada slide, notas, matrices y ausencia de omisiones.
9. **Actualización posterior:** corregir una slide sin regenerar injustificadamente todo el curso.
10. **Cambios de reglas:** no alterar las skills globales a partir de comentarios locales sin aprobación.

Estado de cada test: `Ejecutada y conforme / Ejecutada con fallos / No ejecutada`.


11. **Puerta SVG obligatoria:** antes de Slides comprobar vista previa SVG 16:9 visible, guion íntegro, pantalla, geometría y aprobación editorial explícita.
12. **Estado Aprobada:** maqueta editorial aceptada o Slides creadas sin aceptación final no pueden activar la casilla de clase aprobada.
13. **Redundancia contextual:** una apertura que enumera componentes y su finalidad no se considera automáticamente un duplicado del desarrollo.
14. **Clase 4.4:** pantalla incluye seis funciones solo enumeradas; no anticipar 4.5–4.7 ni confundir figura oficial de perfiles con proceso de cinco pasos.

**Nuevos casos registrados el 2026-11-14: no ejecutados.**


15. **STATE-APPROVE-01 — aprobación y persistencia:** una clase identificada inequívocamente recibe «esta clase está aprobada»; marcar solo G=TRUE, preservar H y otras filas, releer; anotar revisión, IDs y siguiente clase en `PROJECT_STATE.md`, releer GitHub. Rechazar éxito parcial presentado como completo.
16. **STATE-APPROVE-02 — idempotencia y estado de grabación:** repetir aprobación de clase ya aprobada no debe añadir cambios innecesarios ni convertir H a TRUE. Una maqueta editorial aprobada no activa G.
17. **STATE-APPROVE-03 — fallo parcial:** si Sheets se guarda y GitHub falla, reportar exactamente el estado, reintentar tras relectura segura sin repetir escrituras ciegas.
18. **VIS-REFERENCE-01 — foco referenciado:** al copiar un elemento de foco de una slide aprobada, comprobar que imagen base y proporción coinciden; conservar coordenadas relativas y contrastar miniatura/render. Si el resaltado queda desplazado, rechazar como fallo aunque el objeto esté presente.

**Casos 15–18 definidos el 2026-11-14; no equivalen a pruebas ejecutadas. El cierre efectivo de 5.1 documentado en `PROJECT_STATE.md` es evidencia operacional específica de lectura/escritura de estado, no ejecución automática de toda esta batería.**


19. **ALIGN-CONTAINER-01 — centro vertical real:** caja azul y etiqueta de una línea con `contentAlignment=MIDDLE` pero caja de texto desplazada 4 unidades: detectar `Δy`, ajustar solo traslación, conservar escala original, releer `Δy≈0`. No declarar render validado sin inspección visible.
20. **ALIGN-CONTAINER-02 — centro horizontal real:** etiqueta con `paragraphStyle.alignment=CENTER` pero su elemento está 8 unidades a la derecha del centro del contenedor: corregir `Δx` sin variar anchura, tipografía ni estilo.
21. **ALIGN-CONTAINER-03 — preservación de texto compuesto:** un cuadro contiene título y subtítulo en zonas superior/inferior: no exigir que ambos tengan el mismo centro que la caja principal; auditar el conjunto y su centro óptico en render.
22. **ALIGN-CONTAINER-04 — escala y regresión:** texto con tamaño intrínseco 3.000.000 EMU y `scaleY=0,1736`; al trasladar con ABSOLUTE, conservar `scaleX/scaleY` y verificar que no crece ni invade otros bloques.
23. **ALIGN-CONTAINER-05 — revisión de clase completa:** tras corregir una etiqueta, auditar pares texto/contenedor de todas las slides de la clase activa y comprobar que notas y diapositivas anteriores permanecen sin cambios. Casos 19–23 definidos, NO ejecutados como batería automatizada.

24. **HIER-GVOC-01 — categoría/subcategorías:** la panorámica GV.OC diferencia el cuadro principal por área, amarillo tenue y borde más grueso, mientras GV.OC-01…05 mantienen exactamente fondo blanco, borde amarillo y peso visual homogéneo. Rechazar jerarquía ambigua o destacado arbitrario.
25. **MANUAL-EDIT-01 — versión manual vigente:** tras una edición del usuario en la slide 45, regenerar o corregir no reintroduce el acento interior ni el rótulo que quitó; partir siempre del estado vivo.
26. **TEXT-MARGIN-01 — margen vs. wrapping:** al aumentar márgenes laterales reduciendo ancho útil, recalcular líneas y altura efectiva del enunciado oficial; rechazar clipping aunque el objeto de texto siga contenido geométricamente.
27. **CONNECT-GVOC-01 — enlaces a nodos:** en GV.OC-02, las conexiones entre partes interesadas y organización no terminan en vacío ni atraviesan etiquetas; comprobar extremos en render y nativa.
28. **INCLUDE-GVOC-01 — relación no causal:** en GV.OC-03, «INCLUYE» y sus líneas sitúan privacidad/libertades civiles como parte de requisitos aplicables, no como resultado de ellos.
29. **CONNECT-GVOC-02 — dependencia doble:** en GV.OC-05, existen dos conectores nativos editables con puntas orientadas hacia Organización y terminaciones perceptibles en los nodos correctos; no aceptar solo glifos de flecha ni líneas desconectadas.
30. **QA-EVIDENCE-01 — clases de evidencia:** guardar y releer propiedades/nota acredita mutación estructural; sin render actual realmente inspeccionado, el estado es `pendiente de validación visual`, no `aprobada`.
**Casos 24–30 documentados el 2026-11-15; pendientes de ejecución como batería automatizada.**

31. **PRE-DESIGN-01 — problema anticipado:** el storyboard de GV.OC-02 propone líneas de 27 arriba y 45 abajo sin justificación. La puerta A lo rechaza antes de Slides; incluir eje y longitud prevista.
32. **IMPLEMENT-INVARIANT-01 — modificación de nodo:** al mover «ORGANIZACIÓN», recalcular simultáneamente las cuatro líneas y verificar `longitud superior = longitud inferior` (ejemplo 36/36). Rechazar correcciones aisladas.
33. **FULL-COMPOSITION-01 — gráfico aislado vs diapositiva:** GV.OC-05 tiene nodos correctamente equilibrados entre sí, pero su centro total no coincide con el cuadro descriptivo izquierdo; detectar en fase A, corregir conjunto en fase B y verificar ambas alineaciones en fase C.
34. **IDENTITY-3PHASE-01 — nodos hermanos:** Tecnología y Proveedores difieren de color de borde; prevenir en maqueta, igualar en Slides, contrastar estilos y render.
35. **WRAP-3PHASE-01 — etiqueta larga:** «ORGANIZACIÓN» desborda en dos líneas; bloquear diseño por ancho útil insuficiente, evitar al implementar y detectar en render sin confundir caja centrada con texto legible.
36. **CONNECT-3PHASE-01 — longitud y destino:** hay cuatro líneas con igual color pero extremos y longitudes desiguales o flotantes; validar cálculo, API y render en las tres puertas.
37. **CATEGORY-3PHASE-01 — jerarquía NIST:** categoría y cinco subcategorías visualmente idénticas; impedir en storyboard, usar padre amarillo suave/borde más grueso e hijos blancos/borde amarillo, comprobar que los cinco hijos siguen equivalentes.
38. **QA-GATES-01 — trazabilidad:** cada criterio tiene evidencia de plan previo, lectura nativa después de implementación e inspección del render; si falta evidencia de una fase, no declarar las tres completadas.
39. **MANUAL-3PHASE-01 — preservar decisión del usuario:** nueva corrección no restaura etiquetas/acento eliminados manualmente; verificar estado vivo en las tres fases.
**Casos 31–39 documentados como regresión el 2026-11-15; NO constituyen una batería de pruebas ejecutada.**

44. **FOCO-UNICO-GVRM07 — objeto explícito:** la diapositiva 59 debe identificar visual y textualmente «OPORTUNIDAD ESTRATÉGICA» como protagonista; rechazar lupa, estrella o gráfico de crecimiento genéricos que no identifiquen qué se caracteriza.
45. **RAMAS-GVRM07 — relaciones no secuenciales:** dos ramas nativas desde el mismo objeto hacia «CARACTERIZAR — Beneficios y condiciones» e «INCLUIR — En la discusión de riesgos»; comprobar que las flechas no impliquen pasos obligatorios, aprobación ni causalidad falsa.
46. **FOCO-VISUAL — no sobrecarga:** sustituir bloques explicativos redundantes por texto corto y mantener la narración detallada en las notas. Revisión de simetría y espacio frente al panel NIST izquierdo.
47. **FOCO-QA — distinguir evidencias:** comprobar geometría/conectores por API y clipping, legibilidad y equilibrio en render realmente observado; la ausencia de render impide declarar QA visual final aprobado.
**Casos 44–47 documentados el 2026-11-16, no ejecutados como batería automatizada.**
