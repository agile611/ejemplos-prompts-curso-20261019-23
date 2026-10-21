# Plantilla Prompt Refinamiento y versionado

## Esquema del laboratorio

Utilizaremos un objeto JSON pequeño.

Debe contener únicamente estas claves.

participantes:
  entero no negativo o null

estado:
  exacto | aproximado | no_indicado | contradictorio

evidencia:
  fragmento literal breve de la fuente

alertas:
  lista que puede contener participantes_contradictorios
La lista estará vacía si no hay contradicción pendiente.

No se permiten alertas duplicadas.

El esquema se mantendrá entre versiones.

La comparación modifica una política, no la estructura.

## Política objetivo

La política correcta se define antes de ejecutar.

Sus reglas son:

Número inequívoco: conservarlo.
Aproximación explícita: marcar aproximado.
Número ausente: utilizar null y no_indicado.
Cifras incompatibles sin prioridad: utilizar null y contradictorio.
Corrección explícita: utilizar el valor que sustituye al anterior.
Posición posterior sin corrección: no concede prioridad por sí sola.
La evidencia debe permitir revisar la decisión.

Si hay conflicto, debe incluir ambos valores.

Si hay corrección, debe incluir su formulación.

La referencia representa esta política, no el comportamiento inicial.

## Limitación versión 0.1

La versión inicial trata todas las cifras diferentes del mismo modo.

No distingue una corrección explícita.

Su regla puede entrar en conflicto con la política objetivo.

Esa limitación es observable en el texto.

No necesitamos atribuir una causa interna al modelo.

El prompt puede producir una respuesta aceptable pese a la omisión.

También puede seguir literalmente la regla incompleta.

Por eso ejecutaremos el caso afectado.

Si no aparece el fallo, no debemos inventarlo.

La omisión sigue siendo una cuestión de diseño.

Una deficiencia documental y un fallo de ejecución son evidencias distintas.