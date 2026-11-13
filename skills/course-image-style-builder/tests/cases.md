# Pruebas de regresión — Course Image Style Builder

Las pruebas se definen aquí y **no se consideran ejecutadas** por el mero hecho de publicarlas.

## Caso 1 — Referencia con colores distintos del curso
**Entrada:** referencia naranja/negra y paleta aprobada azul oscuro, celeste, blanco.
**Esperado:** preservar geometría/perspectiva/acabados observados, adaptar colores a la paleta del curso.
**Fallo:** adoptar naranja como cuarto color obligatorio o recolorear un logotipo oficial protegido.

## Caso 2 — Referencia sin imagen adjunta
**Entrada:** solo título `NIST CSF 2.0: Implementación y Auditoría de Ciberseguridad`.
**Esperado:** proponer dirección conceptual, no atribuir propiedades observadas a imagen inexistente, no declarar un prompt final aprobado.
**Fallo:** inventar un análisis de imagen.

## Caso 3 — Conceptos diferentes, estética estable
**Entrada:** misma línea gráfica aprobada; concepto A gestión del riesgo, concepto B niveles del CSF.
**Esperado:** iconografía y composición variable, perspectiva/iluminación/geometría/colores constantes.
**Fallo:** duplicar una misma composición o generar estilos incompatibles.

## Caso 4 — Fondo blanco en diapositiva de desarrollo
**Entrada:** imagen que debe colocarse sobre blanco #FFFFFF.
**Esperado:** contorno/contraste suficiente, espacios negativos y recorte correcto.
**Fallo:** figura indistinguible sobre blanco o una escena de fondo completo que altera el template.

## Caso 5 — Figura oficial de NIST
**Entrada:** ilustración de apoyo que necesita un gráfico o logotipo NIST.
**Esperado:** no deformar estructura ni recolorear el activo oficial sin autorización/fuente; sugerir inserción del gráfico oficial.
**Fallo:** recrear de memoria una infografía técnicamente incorrecta.

## Caso 6 — Retroalimentación de un curso
**Entrada:** el usuario ajusta volumen o sombras en un curso específico.
**Esperado:** versionar el prompt de ese curso; no cambiar todas las identidades ni la skill global sin aprobación.
**Fallo:** aplicar la preferencia a todos los cursos.

## Protocolo de ejecución
Guardar fecha, imagen utilizada, prompt maestro, conceptos A/B, salidas, observaciones por criterio, fallo/aprobación y versión. En ausencia de generación real, registrar `No ejecutada / No verificable`, no `Cumple`.
