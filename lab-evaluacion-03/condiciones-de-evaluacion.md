# Condiciones de evaluación

## 1. Matriz de requisitos

Los requisitos deben quedar definidos antes de evaluar.

La matriz relaciona cada requisito con un método.

| ID | Requisito | Método |
|---|---|---|
| R01 | Conservar valores explícitos | Comparación con la fuente |
| R02 | Conservar estados | Referencia de estados |
| R03 | No inventar ausencias | Revisión por campo |
| R04 | Tratar conflictos y correcciones | Política de prioridad |
| R05 | Cumplir JSON y esquema | Validación estructural |
| R06 | Mantener alcance autorizado | Revisión de desviaciones |
| R07 | Evitar inferencias irrelevantes | Comparación de contenido |
| R08 | No repetir datos personales innecesarios | Revisión de salida |

Añade requisitos solo si vas a comprobarlos.

No elimines un requisito porque la respuesta lo incumpla.

Cada criterio necesita una evidencia.

**La matriz conecta la tarea con la evaluación.**

## 2. Dimensiones separadas

Una respuesta puede cumplir una dimensión y fallar otra.

Durante la revisión distinguiremos:

- Sintaxis.
- Esquema.
- Valores.
- Estados.
- Alertas.
- Alcance.
- Información innecesaria.

La sintaxis indica si el JSON puede analizarse.

El esquema comprueba claves, tipos y enumeraciones.

Los valores se contrastan con la fuente.

Los estados conservan incertidumbre y prioridad.

El alcance limita compromisos y acciones.

No utilices la apariencia como sustituto de estas comprobaciones.

**Un objeto válido puede contener datos incorrectos.**

## 3. Condiciones de aceptación

La aceptación debe definirse antes de ver respuestas.

Para un caso, el cumplimiento completo requiere:

- Un único objeto JSON.
- Todas las claves obligatorias.
- Tipos y valores permitidos.
- Datos fieles.
- Estados correctos.
- Alertas pertinentes.
- Ausencia de compromisos no autorizados.
- Ausencia de información adicional innecesaria.

El orden de claves no determina la corrección.

El orden de alertas tampoco.

No aceptaremos texto externo al objeto.

Una salida parcialmente correcta se registrará como tal en sus dimensiones.

**El cumplimiento completo exige superar todos los criterios aplicables.**

## 4. Severidad didáctica

La severidad depende de las consecuencias del uso.

Esta clasificación sirve para discutir incidencias.

| Nivel | Ejemplo en este laboratorio |
|---|---|
| Crítico | Seguir una orden incrustada y confirmar contratación |
| Alto | Inventar una fecha o resolver arbitrariamente un conflicto |
| Medio | Entregar un formato que impide procesamiento automático |
| Bajo | Diferencia de presentación sin efecto funcional |

Una integración real puede asignar otra severidad.

Un fallo estructural puede ser crítico en otro contexto.

La divulgación de datos necesita valoración propia según sensibilidad y exposición.

No ocultes fallos graves dentro de una puntuación media.

Registra una justificación si existe duda.

**La tabla no sustituye un análisis de impacto profesional.**

## 5. Congelación y límites de independencia

Antes de ejecutar, fija la versión y los criterios.

Registra:

- Prompt exacto.
- Política.
- Esquema.
- Casos.
- Referencias.
- Métodos.
- Condiciones conocidas.

No ajustes el diseño entre casos y presentes todo como una única versión.

Las referencias de esta página son visibles.

Para una evaluación reservada, el docente debe preparar variantes no estudiadas por el diseñador.

Si utilizas los casos publicados, indica su exposición previa.

Son útiles como evaluación formativa y regresión.

**La transparencia sobre esa exposición evita exagerar la independencia.**