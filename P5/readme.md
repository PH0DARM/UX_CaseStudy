# Practica 5 

## Paso 5. Pruebas de Evaluación 

### 5.a Reclutamiento de usuarios 
Caso asignado (caso B): [DIU3.RESCUE](https://github.com/Practicas-DIU3-RESCUE)

Para llevar a cabo las pruebas de usabilidad y el análisis comparativo entre nuestra propuesta (Caso A) y el caso asignado (Caso B), se ha seleccionado un grupo de usuarios con perfiles diversos.

El proceso de reclutamiento se basa en una estrategia de muestreo mixto que combina la co-evaluación por pares (intra-testing con compañeros de clase) y pruebas con usuarios externos:

  * Reclutamiento de Co-evaluación (Grupo de clase / Intra-testing): Se han seleccionado 3 participantes de nuestro propio grupo de clase. Al compartir el mismo contexto, su función principal será la evaluación del Caso A (nuestra propia propuesta).

  * Reclutamiento de Usuarios Externos: Se han reclutado participantes adicionales ajenos a la asignatura (familiares, amigos o usuarios potenciales).

A continuación, se detalla la asignación de cada participante:


| Usuarios  | Sexo/Edad  | Ocupación     |  Exp.TIC    | Caso
| --------- | ---------- | ------------- | ----------- | -----
| P01       | M / 22     | Estudiante    | Alta        | A 
| P02       | M / 20     | Estudiante    | Alta        | A 
| P03       | H / 21     | Estudiante    | Alta        | A 
| P04       | M / 19     | Estudiante    | Media       | A  
| P05       | H / 92     | Jubilado      | Baja        | A 
| P06       | H / 20     | Estudiante    | Media       | B 
| P07       | M / 84     | Jubilada      | Baja        | B 
| P08       | M / 56     | Farmaceútica  | Media       | B 
| P09       | H / 54     | Policía       | Media       | B 
| P10       | M / 22     | Estudiante    | Alta        | B 

<br>

### 5.b Diseño de las pruebas 
Se trata de pruebas de corta duración que pueden ser supervisadas o no supervisadas. Hemos diseñado dos tareas específicas que cada usuario deberá resolver en el caso que le haya sido asignado:

**Tarea 1: Visualización y consulta de la carta**
 * Objetivo: Evaluar la facilidad para encontrar el menú de productos de la página.

 * Acción del usuario: El participante deberá navegar por la interfaz hasta localizar y abrir la sección de "La Carta".

 * Métricas a observar: Tiempo empleado, claridad en el etiquetado del menú de navegación y número de clics necesarios.

**Tarea 2: Retorno a la página de inicio**
 * Objetivo: Validar los mecanismos de orientación y la consistencia de la navegación de la web.

 * Acción del usuario: Una vez realizada la Tarea 1, el participante deberá regresar a la pantalla principal del sitio.

 * Métricas a observar: Uso del logotipo como enlace de retorno vs. uso del botón "Inicio" en el menú, y si el usuario se siente desorientado en el proceso.

<br>

### 5.c Cuestionario SUS
Para medir la percepción subjetiva de la usabilidad de ambos sistemas, hemos usado el System Usability Scale (SUS), un instrumento estandarizado que consta de 10 preguntas con respuestas en una escala de 5 puntos (desde "Totalmente en desacuerdo" hasta "Totalmente de acuerdo").

El cuestionario fue desarrollado de forma online utilizando la plataforma Tally. Para su construcción, tomamos como base la plantilla sugerida y la ampliamos integrando al inicio las preguntas de perfil demográfico, lo que nos ha permitido contextualizar las respuestas de manera precisa.

[Acceso al Cuestionario](https://tally.so/r/EkN5AB)

#### Procesamiento de los datos y resultados obtenidos
Para la fase de análisis, los datos de las respuestas de los usuarios se recopilaron desde Tally y se procesaron manualmente aplicando el algoritmo de cálculo estandarizado de la escala SUS detallado en la metodología de [UsabilityGeek](https://usabilitygeek.com/how-to-use-the-system-usability-scale-sus-to-evaluate-the-usability-of-your-website/):

 * Para las preguntas impares (afirmaciones positivas): Se resta 1 a la puntuación otorgada por el usuario (X - 1).
 * Para las preguntas pares (afirmaciones negativas): Se resta la puntuación otorgada por el usuario al número 5 (5 - X).
 * Puntuación final: Se suman los valores obtenidos en las 10 preguntas y el resultado se multiplica por 2.5 para normalizar la puntuación en un rango de 0 a 100.

Tras realizar este cálculo para cada uno de los participantes obtuvimos la siguiente tabla:

| Usuarios  | Metodo     | SUS Score     |  Evaluacion Linguistica     
| --------- | ---------- | ------------- | ----------- 
| P01       |     A      | 92.5          | Excelente       
| P02       |     A      | 100.0         | Excelente       
| P03       |     A      | 87.5          | Excelente        
| P04       |     A      | 97.5          | Excelente       
| P05       |     A      | 60.0          | Suficiente        
| P06       |     B      | 67.5          | Suficiente      
| P07       |     B      | 25.0          | Muy Deficiente       
| P08       |     B      | 42.5          | Deficiente       
| P09       |     B      | 60.0          | Suficiente       
| P10       |     B      | 50.0          | Suficiente 

- Media Final del caso A: 87.5
- Media Final del caso B: 49.0

#### Análisis y conclusiones
Los resultados obtenidos muestran diferencias muy significativas entre ambos sistemas evaluados. El Caso A alcanzó una puntuación media SUS de 87.5, situándose dentro del rango de “excelente usabilidad”, mientras que el Caso B obtuvo una media de 49.0, una valoración claramente inferior a la media recomendada en la escala SUS.

Al relacionar estos resultados con el perfil demográfico y el nivel de experiencia tecnológica de los participantes, se observa una clara influencia de las competencias digitales en la interacción con la interfaz. Los usuarios jóvenes y con mayor experiencia TIC completaron las tareas con rapidez y seguridad, percibiendo el sistema como intuitivo y fácil de utilizar. Esto se refleja especialmente en las puntuaciones elevadas obtenidas por el Caso A.

Sin embargo, en el Caso B se observaron mayores dificultades de uso en varios perfiles de usuarios, independientemente de su nivel de experiencia tecnológica. Entre los principales problemas detectados destacan la falta de claridad en algunos elementos de navegación, la escasa intuición de determinadas funciones y la ausencia de mecanismos de orientación suficientemente visibles. Estas dificultades provocaron momentos de confusión y aumentaron el tiempo necesario para completar las tareas propuestas.

Aunque los usuarios con menor experiencia tecnológica fueron quienes encontraron más barreras durante la interacción, algunos participantes con experiencia media e incluso alta también manifestaron problemas de usabilidad en el Caso B, lo que evidencia deficiencias generales en el diseño de la interfaz y no únicamente limitaciones derivadas del perfil de los usuarios.

En conclusión, el análisis confirma que el Caso A ofrece una experiencia de uso más accesible, intuitiva y consistente que el Caso B. Además, pone de manifiesto la importancia de diseñar interfaces centradas en la diversidad de usuarios, priorizando la claridad visual, la orientación durante la navegación y la simplicidad en la interacción para garantizar una experiencia satisfactoria para todos los perfiles.

<br>

### 5.d A/B Testing
A continuación realizamos una comparación directa entre ambos sistemas:

| Metrica     | Caso A PAYA | Caso B Rescue     
| ----------- | ----------  | -------------- 
| Media SUS   |      87.5   | 49.0              
| Eval Lingüística |  Excelente  | Deficiente               
| Max Score   |     100.0   | 67.5               
| Min Score   |     60.0    | 25.0    

El análisis del cuestionario SUS concluye que el Caso A es el ganador indiscutible con una media excelente de 87.5, demostrando ser una interfaz intuitiva y altamente eficiente para resolver tareas básicas como localizar la carta o regresar al inicio, mientras que el Caso B resulta deficiente con una media de 49.0 debido a problemas críticos de navegación e inconsistencias que frustraron incluso a usuarios experimentados.

<br>

### 5.e Aplicación del método Eye Tracking 
Para esta prueba de Eye Tracking usamos la aplicación de GazeMapping, se definieron los Puntos de Interés (POI) vinculados a nuestras tareas (el acceso a "La Carta" y el botón de "Inicio" / Logotipo). A los usuarios se les guió para realizar búsquedas visuales dirigidas hacia estas zonas.

A continuación, se exponen de forma comparativa los mapas de calor obtenidos para cada participante durante la realización de las dos pruebas fijadas.

**Participante 1**
| Prueba 1: Buscar la Carta | Prueba 2: Volver al Inicio |
| :---: | :---: |
| ![U1 Carta](eye_tracking/P01_1.png) | ![U1 Inicio](eye_tracking/P01_2.png) |

**Participante 2**
| Prueba 1: Buscar la Carta | Prueba 2: Volver al Inicio |
| :---: | :---: |
| ![U1 Carta](eye_tracking/P02_1.png) | ![U1 Inicio](eye_tracking/P02_2.png) |

**Participante 3**
| Prueba 1: Buscar la Carta | Prueba 2: Volver al Inicio |
| :---: | :---: |
| ![U1 Carta](eye_tracking/P03_1.png) | ![U1 Inicio](eye_tracking/P03_2.png) |

**Participante 4**
| Prueba 1: Buscar la Carta | Prueba 2: Volver al Inicio |
| :---: | :---: |
| ![U1 Carta](eye_tracking/P04_1.png) | ![U1 Inicio](eye_tracking/P04_2.png) |

**Participante 5**
| Prueba 1: Buscar la Carta | Prueba 2: Volver al Inicio |
| :---: | :---: |
| ![U1 Carta](eye_tracking/P05_1.png) | ![U1 Inicio](eye_tracking/P05_2.png) |

**Participante 6**
| Prueba 1: Buscar la Carta | Prueba 2: Volver al Inicio |
| :---: | :---: |
| ![U1 Carta](eye_tracking/P06_1.png) | ![U1 Inicio](eye_tracking/p06_2.png) |

**Participante 7**
| Prueba 1: Buscar la Carta | Prueba 2: Volver al Inicio |
| :---: | :---: |
| ![U1 Carta](eye_tracking/P07_1.png) | ![U1 Inicio](eye_tracking/P07_2.png) |

**Participante 8**
| Prueba 1: Buscar la Carta | Prueba 2: Volver al Inicio |
| :---: | :---: |
| ![U1 Carta](eye_tracking/P08_1.png) | ![U1 Inicio](eye_tracking/P08_2.png) |

**Participante 9**
| Prueba 1: Buscar la Carta | Prueba 2: Volver al Inicio |
| :---: | :---: |
| ![U1 Carta](eye_tracking/P09_1.png) | ![U1 Inicio](eye_tracking/P09_2.png) |

**Participante 10**
| Prueba 1: Buscar la Carta | Prueba 2: Volver al Inicio |
| :---: | :---: |
| ![U1 Carta](eye_tracking/P10_1.png) | ![U1 Inicio](eye_tracking/P10_2.png) |

<br>

### 5.f Usability Report de B

[Usability Report](Usability-Report-template.md)

| Herramienta |Pagina               | Resultado     
| ----------- | ------------------- | -------------- 
| Lighthouse  |  Creadores          | 4.0     
| WAVE AIM    |  Principal          | 4.0           
| WAVE AIM    | Votaciones del mes  | 5.0               
| WAVE AIM    |   Salón de la Fama  | 4.0              
| WAVE AIM    |  Creadores          | 6.0   
| WAVE AIM    |  Perfil de Creador  | 5.8



