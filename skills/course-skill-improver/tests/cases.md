# Pruebas iniciales — Course Skill Improver

Este archivo especifica **casos de prueba**, no afirma que se hayan ejecutado.

## Caso 1 — Corrección puntual de título
**Entrada:** el usuario cambia el nombre de una clase en un Google Sheets.
**Esperado:** comparar versiones, proponer una regla condicional cuando proceda; no actualizar todas las skills automáticamente.
**Fallo:** convertir una edición aislada en requisito universal.

## Caso 2 — Cobertura de NIST CSF 2.0
**Entrada:** feedback que solicita títulos más breves y comerciales en `course-curriculum-builder`.
**Esperado:** mantener íntegramente la cobertura del estándar aunque los títulos se acorten.
**Fallo:** eliminar subcategorías para mejorar legibilidad o conversión.

## Caso 3 — Narración y texto en pantalla
**Entrada:** corregir exceso de texto en pantalla.
**Esperado:** recortar texto visual sin eliminar explicación narrativa ni introducir hechos no narrados.
**Fallo:** dejar un texto visible no explicado por la narración.

## Caso 4 — Identidad visual
**Entrada:** un curso solicita paleta tecnológica intensa.
**Esperado:** proponer tonos compatibles con el tema, mantener blanco puro en slides de desarrollo, no sobrecargar.
**Fallo:** aplicar neón automáticamente a todos los cursos o sustituir el blanco en desarrollo.

## Caso 5 — Ausencia de aprobación
**Entrada:** el usuario comparte feedback para diagnóstico sin aceptar una propuesta de regla.
**Esperado:** solo entregar análisis y diff propuesto; no modificar el SKILL.md de destino.
**Fallo:** commit permanente sin confirmación.

## Caso 6 — Cambios contradictorios
**Entrada:** dos ejemplos implican pautas opuestas.
**Esperado:** identificar condiciones de aplicación o pedir decisión editorial.
**Fallo:** reemplazar silenciosamente la regla previa.

## Protocolo
Para cada ejecución registrar: fecha, skill objetivo, commit previo, input, output anterior, output regenerado, criterios, estado, evidencia y commit nuevo. Los resultados no ejecutados se marcan `No ejecutada`; no se declaran éxitos basados solo en inspección de instrucciones.
