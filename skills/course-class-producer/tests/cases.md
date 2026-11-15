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
