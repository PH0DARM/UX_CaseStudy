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

El test expone una marcada brecha digital, ya que los perfiles jóvenes y con alta experiencia TIC completaron las tareas con fluidez, mientras que los usuarios de la tercera edad con competencias bajas experimentaron una severa frustración, hundiendo las puntuaciones.

<br>

### 5.d A/B Testing

A continuacion se realiza una comparacion directa entre ambos sistemas

| Metrica     | Caso A PAYA | Caso B Rescue     
| ----------- | ----------  | -------------- 
| Media SUS   |      87.5   | 49.0              
| Eval Lingui |  Excelente  | Deficiente               
| Max Score   |     100.0   | 67.5               
| Min Score   |     60.0    | 25.0    

El análisis del cuestionario SUS concluye que el Caso A es el ganador indiscutible con una media excelente de 87.5, demostrando ser una interfaz intuitiva y altamente eficiente para resolver tareas básicas como localizar la carta o regresar al inicio, mientras que el Caso B resulta deficiente con una media de 49.0 debido a problemas críticos de navegación e inconsistencias que frustraron incluso a usuarios experimentados

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
![Método UX](img/usability-report.png) 
-----

>>> Añadir report de usabilidad para práctica B (la de los compañeros) aportando resultados y valoración de cada debilidad de usabilidad. 
>>> Enlazar aqui con el archivo subido a P4/ que indica qué equipo evalua a qué otro equipo.

>>> Complementad el Case Study en su Paso 4 con una Valoración personal del equipo sobre esta tarea

<br>


>>> Opinión FINAL del proceso de desarrollo de diseño siguiendo metodología UX y valoración (positiva /negativa) de los resultados obtenidos. ¿Qué se puede mejorar? Recuerda que este tipo de texto se debe eliminar del template que se os proporciona
>>>
# Práctica 5: Pruebas de Evaluación de Usabilidad y Usability Report

Este documento contiene el informe completo de la Evaluación de Usabilidad y el Análisis Comparativo entre la propuesta del **Caso A (PAYA)** y el caso asignado **Caso B (DIU3.RESCUE)**, estructurado en formato Markdown para su integración directa en GitHub.

---

## 5.a Reclutamiento de Usuarios
Caso asignado (Caso B): [DIU3.RESCUE](https://github.com/Practicas-DIU3-RESCUE)

Para llevar a cabo las pruebas de usabilidad y el análisis comparativo entre nuestra propuesta (Caso A) y el caso asignado (Caso B), se ha seleccionado un grupo de usuarios con perfiles diversos. El proceso de reclutamiento se basa en una estrategia de muestreo mixto que combina la co-evaluación por pares (intra-testing con compañeros de clase) y pruebas con usuarios externos:

* **Reclutamiento de Co-evaluación (Grupo de clase / Intra-testing):** Se han seleccionado 3 participantes de nuestro propio grupo de clase. Al compartir el mismo contexto, su función principal será la evaluación del Caso A (nuestra propia propuesta).
* **Reclutamiento de Usuarios Externos:** Se han reclutado participantes adicionales ajenos a la asignatura (familiares, amigos o usuarios potenciales) para asegurar la objetividad y diversidad de destrezas digitales.

### Tabla de Asignación de Participantes

| Usuarios | Sexo / Edad | Ocupación | Exp. TIC | Caso Asignado |
| :--- | :---: | :--- | :---: | :---: |
| **P01** | M / 22 | Estudiante | Alta | A |
| **P02** | M / 20 | Estudiante | Alta | A |
| **P03** | H / 21 | Estudiante | Alta | A |
| **P04** | M / 19 | Estudiante | Media | A |
| **P05** | H / 92 | Jubilado | Baja | A |
| **P06** | H / 20 | Estudiante | Media | B |
| **P07** | M / 84 | Jubilada | Baja | B |
| **P08** | M / 56 | Farmacéutica | Media | B |
| **P09** | H / 54 | Policía | Media | B |
| **P10** | M / 22 | Estudiante | Alta | B |

---

## 5.b Diseño de las Pruebas
Se trata de pruebas de corta duración que pueden ser supervisadas o no supervisadas. Hemos diseñado dos tareas específicas que cada usuario deberá resolver en el caso que le haya sido asignado:

### Tarea 1: Visualización y consulta de la carta
* **Objetivo:** Evaluar la facilidad para encontrar el menú de productos de la página.
* **Acción del usuario:** El participante deberá navegar por la interfaz hasta localizar y abrir la sección de "La Carta".
* **Métricas a observar:** Tiempo empleado, claridad en el etiquetado del menú de navegación y número de clics necesarios.

### Tarea 2: Retorno a la página de inicio
* **Objetivo:** Validar los mecanismos de orientación y la consistencia de la navegación de la web.
* **Acción del usuario:** Una vez realizada la Tarea 1, el participante deberá regresar a la pantalla principal del sitio.
* **Métricas a observar:** Uso del logotipo como enlace de retorno vs. uso del botón "Inicio" en el menú, y detección de si el usuario se siente desorientado en el proceso.

---

## 5.c Cuestionario SUS (System Usability Scale)

Los ítems evaluados en el cuestionario estandarizado SUS son:
1. Me gustaría usar esta página de forma frecuente.
2. Encontré este sistema innecesariamente complejo.
3. El sistema me pareció fácil de usar.
4. Creo que me haría falta ayuda de un especialista para ser capaz de utilizar el sistema.
5. Encontré el sistema bien integrado.
6. Había muchas inconsistencies en el sistema.
7. Me imagino a la mayoría de la gente aprendiendo a usar este sistema de forma muy rápida.
8. Encuentro el sistema muy incómodo de usar.
9. Me sentí muy seguro utilizando el sistema.
10. Tuve que aprender muchas cosas antes de poder utilizar de forma correcta el sistema.

### Tabla de Resultados Cuantitativos

| Usuarios | Método / Caso | SUS Score | Evaluación Lingüística |
| :--- | :---: | :---: | :--- |
| **P01** | A | 92.5 | Excelente |
| **P02** | A | 100.0 | Excelente |
| **P03** | A | 87.5 | Excelente |
| **P04** | A | 97.5 | Excelente |
| **P05** | A | 60.0 | Suficiente |
| **P06** | B | 67.5 | Suficiente |
| **P07** | B | 25.0 | Muy Deficiente |
| **P08** | B | 42.5 | Deficiente |
| **P09** | B | 60.0 | Suficiente |
| **P10** | B | 50.0 | Suficiente |

* **Media Final del Caso A:** 87.5
* **Media Final del Caso B:** 49.0

> **Conclusión del Test SUS:** El test expone una marcada brecha digital, ya que los perfiles jóvenes y con alta experiencia TIC completaron las tareas con fluidez, mientras que los usuarios de la tercera edad con competencias bajas experimentaron una severa frustración, hundiendo las puntuaciones en el Caso B.

---

## 5.d A/B Testing
A continuación se realiza una comparación directa entre ambos sistemas basada en los datos recopilados:

| Métrica | Caso A (PAYA) | Caso B (RESCUE) |
| :--- | :---: | :---: |
| **Media SUS** | 87.5 | 49.0 |
| **Evaluación Lingüística** | Excelente | Deficiente |
| **Puntuación Máxima (Max Score)** | 100.0 | 67.5 |
| **Puntuación Mínima (Min Score)** | 60.0 | 25.0 |

**Análisis Comparativo:** El análisis del cuestionario SUS concluye que el Caso A es el ganador indiscutible con una media excelente de 87.5, demostrando ser una interfaz intuitiva y altamente eficiente para resolver tareas básicas como localizar la carta o regresar al inicio. Por el contrario, el Caso B resulta globalmente deficiente con una media de 49.0 debido a problemas críticos de navegación e inconsistencias de diseño que frustraron incluso a usuarios experimentados.

---

## 5.e Aplicación del Método Eye Tracking
Para esta prueba de Eye Tracking usamos la aplicación de **GazeMapping**. Se definieron los Puntos de Interés (POI) vinculados a nuestras tareas (el acceso a "La Carta" y el botón de "Inicio" / Logotipo). A los usuarios se les guió para realizar búsquedas visuales dirigidas hacia estas zonas.

A continuación, se exponen de forma comparativa los mapas de calor obtenidos para cada participante durante la realización de las dos pruebas fijadas:

### Mapas de Calor por Participante

#### Participante 1
* **Prueba 1 (Buscar la Carta):** `![U1 Carta](eye_tracking/P01_1.png)`
* **Prueba 2 (Volver al Inicio):** `![U1 Inicio](eye_tracking/P01_2.png)`

#### Participante 2
* **Prueba 1 (Buscar la Carta):** `![U2 Carta](eye_tracking/P02_1.png)`
* **Prueba 2 (Volver al Inicio):** `![U2 Inicio](eye_tracking/P02_2.png)`

#### Participante 3
* **Prueba 1 (Buscar la Carta):** `![U3 Carta](eye_tracking/P03_1.png)`
* **Prueba 2 (Volver al Inicio):** `![U3 Inicio](eye_tracking/P03_2.png)`

#### Participante 4
* **Prueba 1 (Buscar la Carta):** `![U4 Carta](eye_tracking/P04_1.png)`
* **Prueba 2 (Volver al Inicio):** `![U4 Inicio](eye_tracking/P04_2.png)`

#### Participante 5
* **Prueba 1 (Buscar la Carta):** `![U5 Carta](eye_tracking/P05_1.png)`
* **Prueba 2 (Volver al Inicio):** `![U5 Inicio](eye_tracking/P05_2.png)`

#### Participante 6
* **Prueba 1 (Buscar la Carta):** `![U6 Carta](eye_tracking/P06_1.png)`
* **Prueba 2 (Volver al Inicio):** `![U6 Inicio](eye_tracking/p06_2.png)`

#### Participante 7
* **Prueba 1 (Buscar la Carta):** `![U7 Carta](eye_tracking/P07_1.png)`
* **Prueba 2 (Volver al Inicio):** `![U7 Inicio](eye_tracking/P07_2.png)`

#### Participante 8
* **Prueba 1 (Buscar la Carta):** `![U8 Carta](eye_tracking/P08_1.png)`
* **Prueba 2 (Volver al Inicio):** `![U8 Inicio](eye_tracking/P08_2.png)`

#### Participante 9
* **Prueba 1 (Buscar la Carta):** `![U9 Carta](eye_tracking/P09_1.png)`
* **Prueba 2 (Volver al Inicio):** `![U9 Inicio](eye_tracking/P09_2.png)`

#### Participante 10
* **Prueba 1 (Buscar la Carta):** `![U10 Carta](eye_tracking/P10_1.png)`
* **Prueba 2 (Volver al Inicio):** `![U10 Inicio](eye_tracking/P10_2.png)`

---



