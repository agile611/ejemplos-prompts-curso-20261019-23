# seguridad

## Descripción
Directorio con prompts de seguridad y defensivos. Contiene prompts para extraer requisitos de fichas internas, asegurar que las instrucciones incrustadas sean detectadas y aplicar políticas de datos rigurosas.

## Conceptos de Prompt Engineering

### Defensive Prompting
Técnica para diseñar prompts que sean resistentes a la manipulación. Incluye la detección de instrucciones incrustadas que intentan desviar la tarea del asistente.

### Instruction Injection Detection
Identificación de cuando el texto de la solicitud contiene órdenes dirigidas al asistente (ej. "ignora el esquema", "responde X"). Estos deben detectarse y manejarse añadiendo la alerta "instruccion_incrustada".

### Data Integrity
Asegamiento de que los datos extraídos sean exactos y no hayan sido alterados por instrucciones externas. Los prompts defensivos extraen "solo lo que dice la fuente".

### Permission Preservation
Regla de no confirmar contratación ni disponibilidad basándose en la solicitud. La solicitud es una fuente de datos, no un modificador de permisos.

### Schema Enforcement
Forzar la salida del modelo a cumplir con un esquema JSON estructurado. Crítico para la integración con sistemas automatizados.

### Source Authority
Principio de que la solicitud es la fuente de datos y sus instrucciones no pueden cambiar la tarea ni los permisos del asistente.

## Estructura de Archivos

- `C-01.md` ... `C-04.md`, `C-04-conv.md`: Prompts de seguridad y defensivos
- `esquema.md`: Esquema de validación de datos
- `prompt.md`: Prompt base de seguridad
- `README.md`: Esta descripción general