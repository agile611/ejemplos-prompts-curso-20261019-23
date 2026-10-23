# refinamiento-y-versionado

## Descripción
Directorio que documenta la evolución de los prompts a través de 4 versiones (v-0.1 a v-0.4). Demuestra cómo se han ido refinando las reglas de manejo de contradicciones y correcciones de participantes.

## Conceptos de Prompt Engineering

### Version Control for Prompts
Gestión sistemática de cambios en prompts a lo largo del tiempo. Este directorio muestra la evolución desde v-0.1 hasta v-0.4, documentando cómo las reglas han sido ajustadas.

### Policy Refinement
Ajuste progresivo de las políticas dentro de un prompt. Ejemplos incluyen:
- v-0.1: Regla simple de "cualquier diferencia = conflicto"
- v-0.2: Se requiere identificación explícita de sustitución
- v-0.3: Estados formalizados (indicado, no_indicado, contradictorio)
- v-0.4: Correcciones explícitas autorizadas por la fuente

### Contradiction Handling
Estrategias para manejar cifras diferentes en la misma solicitud:
- ¿La fuente identifica una que sustituye a otra?
- ¿No hay prioridad explícita? → usar "contradictorio"
- ¿Promediar? → No está permitido
- ¿Elegir la última? → No está permitido

### State Management
Gestión de estados en la extracción de datos:
- `exacto`: Número vigente y exacto
- `aproximado`: Estimación conservada
- `no_indicado`: Fuente sin número
- `contradictorio`: Cifras sin resolver

### Correction Protocol
Protocolo para cuando la fuente proporciona una corrección:
- Debe identificar claramente qué dato sustituye
- La mera posición posterior no concede prioridad automática
- La corrección debe ser explícita y autorizada por la fuente

## Estructura de Archivos

- `contexto.md`: Contexto general del laboratorio
- `v-0.1/`: Versión 0.1 (CH-01, F-01, plantilla-prompt)
- `v-0.2/`: Versión 0.2 (CH-01, F-01, plantilla-prompt, R-01, R-02, R-03)
- `v-0.3/`: Versión 0.3 (CH-01, F-01, plantilla-prompt, R-01, R-02, R-03)
- `v-0.4/`: Versión 0.4 (ADD-01, CH-01, F-01, plantilla-prompt, R-01, R-02, R-03)
- `README.md`: Esta descripción general