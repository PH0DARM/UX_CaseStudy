# Usability Report

### Evaluación de usabilidad del proyecto DIU3.RESCUE
[Enlace a GITHUB del proyecto DIU3.RESCUE](https://github.com/Practicas-DIU3-RESCUE/UX_CaseStudy). Informe realizado por Equipo DIU1.PA'YA 

## 1 RESUMEN EJECUTIVO  (Executive Summary)

### Objetivo
El objetivo de este informe es evaluar la usabilidad del sistema DIU3.RESCUE mediante la aplicación de diferentes técnicas de evaluación centradas en el usuario. Se pretende identificar problemas de navegación, accesibilidad y experiencia de usuario que puedan afectar a la interacción con la plataforma.

### Metodología
La evaluación se llevó a cabo utilizando tres técnicas complementarias:
 - Cuestionario System Usability Scale (SUS) para medir la percepción subjetiva de usabilidad.
 - Análisis Eye Tracking mediante GazeMapping para estudiar la atención visual de los usuarios.
 - Auditoría de accesibilidad basada en herramientas automáticas y revisión manual.

### Principales Hallazgos
 - Los usuarios encontraron dificultades para orientarse durante la navegación y localizar determinadas funcionalidades.
 - Algunos elementos importantes de la interfaz recibieron poca atención visual durante las pruebas.
 - La puntuación SUS obtenida refleja una percepción de usabilidad inferior a la recomendada para aplicaciones con una buena experiencia de usuario.
  
### Resultado Global
DIU3.RESCUE obtuvo una puntuación media SUS de 49.0 puntos. Según la interpretación estándar de la escala SUS, este resultado indica una usabilidad deficiente y pone de manifiesto la necesidad de realizar mejoras en distintos aspectos de la interfaz.

## 2. Metodología y Reclutamiento

### Perfil de los participantes
La evaluación se realizó con usuarios de diferentes edades, ocupaciones y niveles de experiencia tecnológica. Los participantes presentaban perfiles variados, desde estudiantes universitarios con alta experiencia digital hasta personas de edad avanzada con competencias tecnológicas más limitadas.

Esta diversidad permitió analizar el comportamiento de distintos tipos de usuarios ante las funcionalidades ofrecidas por el sistema.

### Escenario de la prueba
Los participantes realizaron dos tareas principales:

#### Tarea 1. Consulta de la carta
El usuario debía localizar y acceder a la sección correspondiente al menú de productos.

#### Tarea 2. Retorno a la página principal
Una vez finalizada la tarea anterior, el usuario debía regresar a la página de inicio utilizando los mecanismos de navegación disponibles.


Durante las pruebas se observaron tiempos de ejecución, errores de navegación, dudas de orientación y comportamiento visual.

### Herramientas
 - Tally para la recogida de respuestas del cuestionario SUS.
 - GazeMapping para la obtención de mapas de calor y análisis visual.
 - Lighthouse y WAVE (Web Accessibility Evaluation Tool) como herramientas de evaluación de accesibilidad.


## 3. Resultados del Cuestionario SUS (Datos Cuantitativos)

[Aquí se muestran datos del análisis multivariable de SUS] 

- **Comparativa A vs. B:** Un gráfico de barras comparando la puntuación final de ambos diseños.
- **Desglose por ítems:** Identifica qué preguntas del SUS tuvieron peor puntuación (por ejemplo, si la pregunta 2 sobre "complejidad" fue muy alta en el Diseño B).

Valoración numérica del SUS - 


## 4. Análisis de Eye Tracking (Datos Biométricos)

[Presenta la evidencia visual del comportamiento del usuario]

- **Heatmaps (Mapas de calor):** Incluye las capturas de GazeMapping. Comenta si los usuarios miraron los **POI** (Puntos de Interés) definidos.
- **Zonas de Silencio:** Identifica elementos importantes que fueron totalmente ignorados.
- **Hallazgo clave:** Ejemplo: "El 80% de los usuarios ignoró el botón de CTA debido a su ubicación en el margen inferior".

## 5. Auditoría de Accesibilidad

Sintetiza el cumplimiento técnico y normativo.

- **Puntuación Automática:** (Lighthouse/WAVE).
- **Principales barreras:** Lista los errores críticos (contraste, falta de etiquetas, etc.) y cómo afectan a los usuarios con discapacidad.

## 6. Conclusiones y Recomendaciones (Actionable Insights)

No te limites a decir qué está mal; di cómo arreglarlo. Clasifica las recomendaciones por prioridad:

| **Prioridad**      | **Hallazgo**                                                 | **Recomendación de Mejora**                                  |
| ------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| **Alta (Crítica)** | Ej. El SUS indica alta complejidad y el Eye Tracking muestra confusión en el menú. | Simplificar la arquitectura de información y aumentar el tamaño de las fuentes. |
| **Media**          | Ej. Los usuarios no ven el botón de registro rápidamente.        | Cambiar el color del CTA a uno de mayor contraste según WCAG. |
| **Baja**           | Ej. El logo no redirige a la home.                               | Añadir el enlace estándar al logotipo en la cabecera.        |



