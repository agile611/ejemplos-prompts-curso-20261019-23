# prompt 0.4

Extrae el número de participantes de la solicitud.

Devuelve únicamente JSON con:
participantes, estado, evidencia y alertas.

Utiliza únicamente la fuente.
Conserva aproximaciones.

El campo estado solo puede tener uno de estos valores:
- "indicado": hay un número de participantes vigente, exacto
  o aproximado, sin contradicciones pendientes.
- "no_indicado": la fuente no proporciona un número de participantes.
- "contradictorio": hay cifras diferentes que no quedan resueltas
  mediante una sustitución explícita en la fuente.

No utilices otros valores para estado.
Una aproximación no cambia el estado: conserva la aproximación
en participantes y utiliza "indicado" si no hay contradicción pendiente.

Si no hay número, utiliza participantes: null y estado: "no_indicado".

Si hay cifras diferentes, aplica una corrección
solo cuando la fuente identifica que sustituye al valor anterior.
No elijas una cifra únicamente por aparecer después.

Si después de aplicar las sustituciones explícitas quedan
cifras incompatibles, utiliza participantes: null,
estado: "contradictorio"
y alertas: ["participantes_contradictorios"].

En los demás casos, alertas será una lista vacía.

Formato de salida:
- Devuelve un único objeto JSON válido.
- No uses bloques de código, delimitadores Markdown ni texto
  antes o después del objeto JSON.
- Usa las claves en este orden:
  participantes, estado, evidencia, alertas.
- No añadas otras claves.

Regla para evidencia:
- evidencia será siempre una cadena de texto.
- Copia íntegramente el contenido de SOLICITUD.
- No resumas, reformules, omitas ni selecciones fragmentos.
- Sustituye cada secuencia de espacios, tabulaciones o saltos
  de línea por un único espacio.
- Elimina los espacios al principio y al final.
- Conserva las palabras, cifras, mayúsculas y puntuación originales.
- Aplica únicamente el escapado necesario para que la cadena
  sea válida en JSON.

Problema:
La regla trata cualquier diferencia como conflicto pendiente.

Requisito:
Aplicar correcciones explícitas autorizadas por la fuente.

Hipótesis:
Una distinción entre corrección y mera aparición posterior
resolverá F-01 sin elegir arbitrariamente en conflictos reales.


## SOLICITUD

El primer mensaje indicaba 12 participantes.

Corrección confirmada:
Serán 15 participantes.
La cifra de 15 sustituye a la anterior.
