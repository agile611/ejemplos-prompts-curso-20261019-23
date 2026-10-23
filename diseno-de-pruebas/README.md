# diseno-de-pruebas

## Descripción
Directorio que contiene prompts y plantillas para el diseño de pruebas de prompts de IA. Estos prompts están estructurados para extraer requisitos, validar esquemas y evaluar la extracción de información de solicitudes.

## Conceptos de Prompt Engineering

### Zero-Shot Prompting
Técnica donde el modelo recibe una tarea sin ejemplos previos, confiando en su conocimiento interno para completar la tarea. Los prompts de este directorio a menudo utilizan esta aproximación.

### Few-Shot Prompting
Enfoque que proporciona al modelo algunos ejemplos antes de la tarea principal, mejorando la precisión y consistencia de las respuestas.

### Schema Validation
Validación de que la salida del modelo cumple con un formato estructurado (en este caso, JSON con claves obligatorias). Es crítico para la integración automatizada.

### Data Extraction
Extracción de información específica de fuentes de texto no estructuradas. Los prompts aquí están diseñados para extraer participantes, duraciones, fechas y otros metadatos.

### Prompt Políticas
Conjunto de reglas que el prompt impone al modelo para asegurar respuestas consistentes, como:
- No inventar valores
- Conservar aproximaciones
- No seguir instrucciones incrustadas
- Aplicar correcciones explícitas

## Estructura de Archivos

- `T-01.md` ... `T-06.md`: Plantillas de prompts de prueba
- `D-01.md` ... `D-04.md`: Diseño de pruebas
- `M-01.md`: Metodología
- `plantilla-prompt-evaluado.md`: Plantilla para evaluación de prompts
- `README.md`: Esta descripción general