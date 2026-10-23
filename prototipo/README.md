# Prototipo: Taller de Prompts Revisables

## Acerca de esta carpeta

El directorio `prototipo/` contiene un taller práctico autónomo sobre ingeniería de prompts, independiente del repositorio principal. Esta carpeta incluye todos los materiales necesarios para ejecutar el taller de 90 minutos, enfocado en la extracción y validación de requisitos usando modelos de IA.

## Ficheros de esta carpeta

Los siguientes archivos describen:

### 1. `briefing.md`
- **Contenido**: Datos completos del taller (fecha, modelo, público, precio)
- **Propósito**: Define el contexto oficial antes de iniciar las actividades
- **Elementos invariantes**: Fecha 18-Nov-2026, 90 minutos, gratuito, datos sintéticos

### 2. `ejecucion-1.md` ... `ejecucion-4.md`
- **Contenido**: Cuatro fases secuenciales del taller:
  - **Ejecución 1**: Explorar tres enfoques (práctica concreta, revisión de errores, aprendizaje colaborativo)
  - **Ejecución 2**: Redactar correo sobre la actividad (hasta 180 palabras)
  - **Ejecución 3**: Adaptar a aviso interno (hasta 90 palabras)
  - **Ejecución 4**: Revisión editorial (comparar con briefing, detectar problemas)
- **Propósito**: Flujo de trabajo secuencial para completar el taller

### 3. `entorno.md`
- **Contenido**: Configuración del entorno VS Code + Nemotron 3.5 Lightning
- **Restricciones**: Sin herramientas externas, sin publicación, datos sintéticos solo
- **Propósito**: Asegurar que el taller se ejecute en las condiciones correctas

## Conceptos de Prompt Engineering que se ven en esta carpeta

Los siguientes conceptos se ven específicamente en el contexto de este taller práctico:

### 1. Flujo de Trabajo Secuencial de Taller
Este prototipo sigue un flujo fijo de 4 ejecuciones:
- **Fase 1 (Ejecución 1)**: Definir enfoques antes de redactar
- **Fase 2 (Ejecución 2)**: Aplicar el enfoque elegido redactando contenido
- **Fase 3 (Ejecución 3)**: Adaptar el contenido para diferentes formatos (avisos internos)
- **Fase 4 (Ejecución 4)**: Revisar y validar todo el contenido generado

**Riesgo de interpretación**: Saltarse fases o cambiarlas de orden puede comprometer los resultados esperados, ya que cada fase construye sobre la anterior.

### 2. Restricciones de Contenido Específicas
Este taller tiene restricciones de escritura:

- **No inventar beneficios medidos**: Sin afirmaciones de resultados cuantificados
- **No inventar plazas ni certificados**: El taller es gratuito y opcional
- **Sin horario artificial**: Las fechas son fijas, pero los horarios son flexibles
- **Sin urgencia artificial**: Las solicitudes de interés no tienen límite de tiempo
- **Sin firma en correos**: El enfoque está en el contenido, no en la presentación personal

### 3. Enfoques de Comunicación
Este taller enseña tres formas de comunicar el mismo contenido:

- **Enfoque A: Práctica concreta**: Enfocado en la acción y los pasos a seguir
- **Enfoque B: Revisión y detección de errores**: Enfocado en la validación y calidad
- **Enfoque C: Aprendizaje colaborativo**: Enfocado en el aspecto social y el intercambio

Cada enfoque tiene:
- **Idea central**: El propósito principal
- **Apertura original**: Cómo comenzar cada pieza
- **Riesgo de interpretación**: Posibles malentendidos si no se siguen las directrices

### 4. Formatos de Salida Múltiples
A diferencia de los prompts del repositorio que siempre devuelven JSON, este taller practica formatos variados:

- **JSON estructurado**: Para validación de esquemas (conceptos del repositorio principal)
- **Correo electrónico**: Formato profesional con asunto y cuerpo (hasta 180 palabras)
- **Aviso interno**: Formato condensado (hasta 90 palabras)
- **Tabla de revisión**: Estructura pieza, fragmento, problema, evidencia

### 5. Detección de Datos Inventados
Un concepto crítico en este taller (diferente al repositorio principal):

- **Hechos**: Datos presentes en el briefing (fecha, duración, modalidad)
- **Estados**: Compromiso vs no compromiso (respuesta de interés no confirma plaza)
- **Compromisos**: Elementos explícitamente prohibidos (precio, plazas, certificado, enlace)
- **Omisiones críticas**: Elementos que si faltan indicarían un problema

**Tabla de revisión (Ejecución 4)**:
| Pieza | Fragmento | Problema | Evidencia del briefing |
|-------|-----------|----------|-----------------------|
| Correo/Aviso | Cualquier dato no en briefing | Datos inventados | No está en la sección "No indicado" |
| Correo/Aviso | Mención a plazas/certificados | Compromiso prohibido | "No indicado: precio, plazas, certificado" |
| Correo/Aviso | Horario o urgencia | Urgencia artificial | No está definido en el taller |

### 5. Modelo de Revisión entre Pares
Este taller incluye:

- **Comparación entre piezas**: Revisar múltiples ejecuciones (1-4) en busca de consistencia
- **Detección de omisiones**: Identificar qué se prometió vs qué se entregó
- **Evidencia del briefing**: Cada problema debe rastrearse al documento original
- **Sin afirmación de fiabilidad general**: Reconocer problemas sin validar todo el contenido

### 6. Adaptación de Contenido
Concepto único para este prototipo:

- **De correo a aviso interno**: Reducir de 180 palabras a 90 palabras manteniendo información clave
- **Preservar esencia**: Actividad, fecha, modalidad y duración deben sobrevivir a la adaptación
- **Mantener acción**: La solicitud de interés debe conservarse en todas las adaptaciones
- **Prohibido inventar**: Datos, horarios, precios o urgencia artificial

## Estructura de Ejecución

```
prototipo/
├── README.md              # Esta descripción general
├── briefing.md            # Contexto oficial del taller
├── entorno.md             # Condiciones y restricciones
├── ejecucion-1.md         # Fase 1: Explorar enfoques
├── ejecucion-2.md         # Fase 2: Redactar contenido
├── ejecucion-3.md         # Fase 3: Adaptar formato
└── ejecucion-4.md         # Fase 4: Revisión editorial
```

## Para Estudiantes Futuros de este Prototipo

Si visitas este repositorio y quieres ejecutar este taller:

1. **Lee el briefing.md primero** - entiende el contexto oficial
2. **Ejecuta las 4 fases en orden** - cada una construye sobre la anterior
3. **Usa solo VS Code** - no se requieren herramientas externas
4. **Trabaja con datos sintéticos** - nunca datos reales ni personales
5. **Respetar las restricciones** - sin inventar plazas, precios ni certificados
6. **Compara tus outputs** con los esperados en los ficheros ejecucion-*.md
7. **Usa Nemotron, Gemini o Copilot** - el taller está diseñado para ser multiplataforma de IA

## Principios Específicos de este Prototipo

✅ **Flujo secuencial obligatorio**: Las 4 ejecuciones deben seguirse en orden  
✅ **Sin datos reales**: Todo es sintético/ficticio  
✅ **Sin compromisos**: Sin plazas, precios ni certificados inventados  
✅ **Revisión editorial estructurada**: Tabla pieza-fragmento-problema-evidencia  
✅ **Modelos de IA compatibles**: Funciona con Nemotron, Gemini y Copilot  
✅ **Entorno VS Code aislado**: Sin herramientas externas necesarias  

---

*Última actualización: 2026-10-23*