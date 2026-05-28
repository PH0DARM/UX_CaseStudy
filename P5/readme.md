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

# Usability Report: Caso B (DIU3.RESCUE)

<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRF017nhV-TFmNER2OM8UbXtdN6xwAKBYrv0i6onNfKu6Yn0BV0RK6aiOroeXl73LSY-B0&usqp=CAU" alt="usability report logo" style="height:150px" />

### Evaluación de usabilidad del proyecto: DIU3.RESCUE
**Fecha de evaluación:** 28 de mayo de 2026  
**Enlace al repositorio evaluado:** [DIU3.RESCUE GitHub](https://github.com/Practicas-DIU3-RESCUE)  

**Realizado por:** Informe realizado por el equipo de diseño del **Caso A (PAYA)**. Nuestra experiencia aplicando metodologías de co-evaluación cruzada nos ha permitido contrastar la robustez arquitectónica de una interfaz ajena con datos empíricos, identificando áreas de mejora fundamentales para el diseño inclusivo.

---

## 1. RESUMEN EJECUTIVO (Executive Summary)

* **Objetivo:** Evaluamos la usabilidad y la eficiencia de la interfaz de usuario del Caso B (DIU3.RESCUE) con el fin de diagnosticar puntos de fricción, fallos en el flujo de navegación habitual y barreras cognitivas que impidan una experiencia de usuario óptima.
* **Metodología:** Hemos aplicado un enfoque mixto combinando pruebas de usabilidad basadas en escenarios, análisis psicométrico estandarizado mediante el **Cuestionario SUS** y análisis biométrico del comportamiento visual mediante mapas de calor generados con **Eye Tracking (GazeMapping)**.
* **Principales Hallazgos:**
    1.  **Brecha Digital Penalizante:** El sistema carece por completo de adaptabilidad para la tercera edad o usuarios con baja competencia TIC (ej. participante P07 con una puntuación SUS crítica de 25.0).
    2.  **Inconsistencia del Modelo Mental:** Elementos habituales de navegación confunden incluso a nativos digitales (ej. P10, con experiencia TIC Alta, valoró el sistema con un insuficiente 50.0).
    3.  **Zonas de Silencio en Elementos Críticos:** El análisis biométrico demuestra que el logotipo superior no posee la *affordance* adecuada para ser interpretado como botón de retorno.
* **Resultado Global:** El Caso B obtiene una **Media SUS Final de 49.0**, lo que cataloga lingüísticamente al sistema como **"Deficiente" (No Aceptable)**, situándose muy lejos del estándar de usabilidad (68 puntos).

---

## 2. Metodología y Reclutamiento

* **Perfil de los Participantes:** Se evaluó a un subgrupo de 5 usuarios (P06 a P10) balanceado demográficamente. La edad promedio se sitúa en **47.2 años** (rango de 20 a 84 años), con niveles de destreza tecnológica variados (1 Alta, 3 Media, 1 Baja).
* **Escenario de la Prueba:** Cada participante se enfrentó de forma autónoma a dos tareas consecutivas sin asistencia técnica previa:
    * *Tarea 1:* Localizar de manera intuitiva el menú de productos ("La Carta").
    * *Tarea 2:* Retornar de forma inmediata a la Home o pantalla de inicio tras la consulta.
* **Herramientas Empleadas:** Software de tracking ocular **GazeMapping**, plantillas estandarizadas SUS y herramientas automáticas de accesibilidad.

---

## 3. Resultados del Cuestionario SUS (Datos Cuantitativos)

El análisis matemático multivariable de las respuestas del SUS arroja una severa deficiencia estructural en el Caso B:

* **Puntuación Media Final del Caso B:** 49.0 / 100 (*Deficiente*)
* **Puntuación Media Final del Caso A (Control):** 87.5 / 100 (*Excelente*)

### Análisis de Ítems Críticos
Las mayores penalizaciones en el Caso B se concentraron en las preguntas negativas del test:
* **Ítem 2 ("Sistema innecesariamente complejo"):** Puntuaciones inusualmente elevadas (4 y 5 sobre 5), provocadas por una mala distribución visual del catálogo.
* **Ítem 6 ("Muchas inconsistencias en el sistema"):** Los usuarios manifestaron confusión debido a que las transiciones de las páginas rompen las convenciones básicas de la navegación web.

---

## 4. Análisis de Eye Tracking (Datos Biométricos)

A través de las métricas visuales extraídas de las sesiones con **GazeMapping**, se obtuvieron las siguientes conclusiones empíricas:

* **Dispersión en Heatmaps:** Durante la *Tarea 1*, los fijaciones visuales de los usuarios del Caso B no fueron directas. Se observan rutas de escaneo caóticas en la cabecera, lo que confirma que el etiquetado actual no se alinea con el modelo mental esperado.
* **Zonas de Silencio:** El logotipo de Rescue (cuadrante superior izquierdo) funcionó como una zona de silencio absoluta durante la *Tarea 2*. Los usuarios no fijaron la mirada en él para regresar al inicio, recurriendo en su lugar a la búsqueda de botones de texto explícitos que a menudo estaban ocultos.
* **Hallazgo Clave:** El 80% de los usuarios ignoró las zonas de interacción preferentes (*Call To Action*) debido a una jerarquía visual plana y a la falta de contrastes lumínicos definidos.

---

## 5. Auditoría de Accesibilidad

La prueba con la usuaria P07 (84 años, TIC Baja) destapó barreras que coinciden con las directrices de accesibilidad técnica de la normativa WCAG:

* **Puntuación Automática Estimada:** ~52/100 en herramientas de validación de contraste.
* **Principales Barreras:**
    1.  **Deficiencia de Contraste:** La relación de contraste texto-fondo de los menús secundarios es inferior a 4.5:1, dificultando la lectura a personas con fatiga o limitaciones visuales.
    2.  **Rigidez del Layout:** El diseño se desmaqueta o corta texto esencial al forzar el zoom del navegador, impidiendo el uso de herramientas de asistencia nativas del sistema operativo.

---

## 6. Conclusiones y Recomendaciones (Actionable Insights)

Para transformar estas vulnerabilidades en oportunidades de optimización, se detallan las siguientes soluciones prioritarias:

| **Prioridad** | **Hallazgo** | **Recomendación de Mejora** |
| :--- | :--- | :--- |
| **Alta (Crítica)** | El SUS indica alta complejidad y el Eye Tracking muestra dispersión caótica e incapacidad para localizar "La Carta" eficientemente. | **Reestructuración de la Arquitectura de Información:** Simplificar el menú de navegación principal de la cabecera utilizando términos estándar y limpios. Incrementar los tamaños de tipografía activa. |
| **Media** | Los usuarios sénior o con competencias medias sufren fatiga visual extrema debido a la ilegibilidad y la falta de feedback dinámico. | **Ajuste de Contraste WCAG:** Modificar la paleta de colores cromática de las fuentes tipográficas para cumplir con el estándar de contraste y añadir animaciones de estado (*hover*/*focus*). |
| **Baja** | El logotipo corporativo superior actúa como "Zona de Silencio" y no es reconocido como un atajo funcional hacia la pantalla principal. | **Affordance e Hipervínculo Estándar:** Modificar el contenedor del logotipo para que sea visualmente interactivo, asegurando que enlace de manera unívoca a la raíz del sitio web (`/index.html`). |

---

## 5.f Opinión y Valoración Personal del Proceso (Equipo Caso A)

**Valoración del Proceso UX:** La implementación del diseño guiado por metodologías UX ha demostrado ser un elemento crítico y diferenciador. El contraste empírico entre el Caso A y el Caso B evidencia que las decisiones estéticas no deben suplantar nunca a la usabilidad. La metodología nos ha permitido descubrir debilidades de forma objetiva (mediante biometría y métricas estandarizadas) que a simple vista en un análisis heurístico convencional podrían haber pasado desapercibidas.

**¿Qué se puede mejorar?** Para futuras iteraciones, es recomendable ampliar la muestra del panel de usuarios a perfiles con discapacidades motoras o visuales severas para robustecer la auditoría de accesibilidad. Asimismo, integrar métricas de rendimiento puras (como la Tasa de Éxito en Tarea y el Tiempo por Tarea en segundos) complementaría los mapas de calor de Eye Tracking, proporcionando un marco de análisis tridimensional indiscutible (comportamiento visual, rendimiento técnico y satisfacción percibida).



