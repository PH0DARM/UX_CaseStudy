# Practica 5 - entregables

- Users. Elección y características de los usuarios reclutados
- Diseño de las pruebas
- Realización del Cuestionario SUS para usuarios y casos A y B.
- Tabla A/B Testing con resultados para A y B
- Eye Tracking para B
- Usability Report del Caso B, con toda la información recabada del caso B


## Paso 4. Pruebas de Evaluación 

### 4.a Reclutamiento de usuarios 
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

### 4.b Diseño de las pruebas 
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

### 4.c Cuestionario SUS
![Método UX](img/Survey.png) 
----


- Me gustaria usar esta pagina de forma frecuente.
- Encontre este sistema innecesariamente complejo.
- El sistema me parecio facil de usar.
- Creo que me haria falta ayuda de un expecialista para ser capaz de utilizar el sistema.
- Encontre el sistema bien integrado.
- Habia muchas inconsistencias en el sistema.
- Me imagino a la mayoria de gente aprendiendo a usar este sistema de forma muy rapida.
- Encuentro el sistema muy incomodo de usar.
- Me senti muy seguro utilizando el sistema.
- Tuve que aprender muchas cosas antes de poder utilizar de forma correcta el sistema

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

El análisis del cuestionario SUS concluye que el Caso A es el ganador indiscutible con una media excelente de 87.5, demostrando ser una interfaz intuitiva y altamente eficiente para resolver tareas básicas como localizar la carta o regresar al inicio, mientras que el Caso B resulta deficiente con una media de 49.0 debido a problemas críticos de navegación e inconsistencias que frustraron incluso a usuarios experimentados. Asimismo, los datos revelan una marcada brecha digital en ambos escenarios: las puntuaciones caen notablemente en los perfiles de la tercera edad con baja experiencia tecnológica (como el 60.0 de P05 en el Caso A y el alarmante 25.0 de P07 en el Caso B).

### 4.d A/B Testing

### 4.e Aplicación del método Eye Tracking 
Para esta prueba de Eye Tracking usamos la aplicación de GazeMapping, se delimitaron los Puntos de Interés (POI) críticos vinculados a nuestras tareas (el acceso a "La Carta" y el botón de "Inicio" / Logotipo). A los usuarios se les guio para realizar búsquedas visuales dirigidas hacia estas zonas.

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


### 4.f Usability Report de B
![Método UX](img/usability-report.png) 
-----

>>> Añadir report de usabilidad para práctica B (la de los compañeros) aportando resultados y valoración de cada debilidad de usabilidad. 
>>> Enlazar aqui con el archivo subido a P4/ que indica qué equipo evalua a qué otro equipo.

>>> Complementad el Case Study en su Paso 4 con una Valoración personal del equipo sobre esta tarea

<br>


>>> Opinión FINAL del proceso de desarrollo de diseño siguiendo metodología UX y valoración (positiva /negativa) de los resultados obtenidos. ¿Qué se puede mejorar? Recuerda que este tipo de texto se debe eliminar del template que se os proporciona 
