# lab-evaluacion-03

## Descripción
Directorio de laboratorio para la evaluación 03. Contiene prompts convergentes, fichas de requisitos y registros de entorno para la evaluación de sistemas de prompts de IA.

## Conceptos de Prompt Engineering

### Convergent Prompting
Enfoque para crear prompts que converjan en salidas consistentes entre diferentes modelos (Nemotron, Gemini, Copilot). La plantilla `prompt-comun-conv-merged.md` aglutina instrucciones de múltiples plantillas para lograr consistencia.

### Prompt Convergence
El proceso de que múltiples modelos produzcan salidas idénticas o muy similares cuando se les da la misma entrada. Los desafíos incluyen:
- Diferentes formatos de salida (JSON formateado vs compacto)
- Variaciones en la inclusión de alertas
- Consistencia en la aplicación de políticas

### Prompt Merging
Combinación de instrucciones de múltiples plantillas en una sola. La plantilla `prompt-comun-conv-merged.md` fusiona características de `prompt-comun-conv-T-04.md` y `prompt-comun-conv-T-07.md`.

### Schema Adherence
Medición de qué tan estrictamente el modelo sigue el esquema JSON especificado. Los problemas comunes incluyen:
- Orden diferente de claves
- Alertas adicionales o faltantes
- Formato de número variado

### Context Preservation
Mantener el contexto de la solicitud a lo largo de la extracción de requisitos. Las políticas prohíben añadir datos personales, comentarios fuera del esquema o inferencias no documentadas.

## Estructura de Archivos

- `prompt-comun-conv-T-04.md`: Plantilla base T-04
- `prompt-comun-conv-T-07.md`: Plantilla base T-07
- `prompt-comun-conv-merged.md`: Plantilla convergente (aglutina T-04 y T-07)
- `T-01.md` ... `T-07.md`: Prompts de prueba y casos
- `FIA-44.md`, `FIA-45.md`: Fichas de fiabilidad
- `registro-de-entorno.md`: Registro de configuración del entorno
- `README.md`: Esta descripción general