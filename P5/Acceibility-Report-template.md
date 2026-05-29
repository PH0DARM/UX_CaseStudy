# Accesibility Report (template)

<img src="https://img.uxcel.com/cdn-cgi/image/format=auto/practices/wcag-principles-overview-1742315821212/a-1742315821212-2x.jpg" alt="usability Download png" style="height:200px" />

Cabe destacar como aviisamos en clase que para la usabilidad como los integrantes de Rescue no tenian en el repositorio la pagina lanzada, tuvimos que hacerlo con unos mockups incompletos los cuales tenian subidos, sin embargo con como para el estudio de accesibilidad necesitamos poder acceder a la pagina usaremos el lanzamiento que estos hicieron de la pagina mas tarde por lo que no coincidira la accesibilidad con la usabilidad.

## 1. Ficha Técnica del Informe

Antes de entrar en detalles, define el alcance.

- **Nombre del proyecto:** Diseño B DIU3.RESCUE
- **Normativa de referencia:** WCAG 2.1 — Nivel AA / Norma UNE-EN 301549
- **Herramientas utilizadas:** Lighthouse, WAVE.
- **Fecha de la auditoría:** 29 de mayo de 2026

## 2. Puntuaciones Globales (Métricas Automáticas)

### Lighthouse de la pagina principal

| Métrica          | Resultado          |
| ---------------- | ------------------ |
| Accesibilidad    | 90/100             |

Un 90 en la categoría de Accesibilidad de Lighthouse significa que tu web está en la zona verde (excelente), lo que demuestra el diseño cumplen con la gran mayoría de los estándares internacionales para que personas con discapacidades (visuales, motoras o cognitivas) puedan navegar sin barreras. Esto implica que el sitio cuenta con un buen contraste de color, etiquetas HTML semánticas correctas y compatibilidad con lectores de pantalla o navegación por teclado. Sin embargo hay algun aspecto a mejorar como que los elementos de encabezado no aparecen en orden secuencial descendente.

### WAVE por pagina

Hemos tenido problema y es que todos los enlaces de la pagina mandan a la misma pagina pero a diferentes alturas por lo que los valores de el analisis saldran exactamente iguales y no hay mas paginas accesibles aparte de esa.

| Pagina    | AIM Score  | Errores       |  Error Contraste  | Alertas | Features
| --------- | ---------- | ------------- | ----------------- | ------- | --------
| Inicio    | 6.9        | 1             | 5                 | 5       | 3
| Pide vota | 6.9        | 1             | 5                 | 5       | 3
| Salon Fama| 6.9        | 1             | 5                 | 5       | 3
| Creadores | 6.9        | 1             | 5                 | 5       | 3

Tras el analisis de las paginas analizafos por AIM se obtuvo una puntuacion por encima de 6 por lo que refleja un nivel decente de accesibilidad, por otro lado el fallo principal de la pagina es la falta de contenido en algunos enlaces ya que estos no redirigen a ningun lado o simplemente no funcionan lo cual a nivel de accesibilidad puede resultar confuso y el agrupar todo el contenido de esta en una sola pagina a nivel de organizacion no es lo mas correcto

## 3. Análisis por Principios (POUR)

Para que el informe sea profesional, agrupa los fallos según los 4 principios de la accesibilidad:

<img src="https://cdn.sanity.io/images/r115idoc/production/e745ae232e5e6760c1392354021aed4eecc4627d-1920x1080.png" alt="usability Download png" style="height:200px" />

### A. Perceptible

Hallazgo ACC-01 — Contraste en elementos destacados (Rojo y Gris)
WAVE detectó 5 errores de contraste debido al uso de texto rojo corporativo y descripciones en gris medio sobre el fondo oscuro de la interfaz.

Criterio WCAG: 1.4.3 — Contraste mínimo (Nivel AA). Ratio mínimo: 4.5:1.

Impacto: Usuarios con baja visión o daltonismo no podrán leer correctamente el eslogan principal ("NOSOTROS LA COCINAMOS"), la etiqueta "EDICIÓN DE MARZO" ni los textos secundarios.

Recomendación: Cambiar el texto rojo por un tono más claro/brillante que contraste sobre negro, o usar blanco (#FFFFFF) para asegurar la lectura. Aumentar el brillo de los textos grises pequeños.

Hallazgo ACC-02 — Control de formulario sin etiqueta (Missing form label)
WAVE detectó 1 error crítico (icono rojo 'X') en la zona superior de la interfaz, donde un elemento interactivo o campo de texto carece de descripción.

Criterio WCAG: 1.1.1 — Contenido no textual (Nivel A).

Impacto: Los lectores de pantalla solo reproducirán la palabra "botón" o "campo de texto", impidiendo que un usuario invidente sepa para qué sirve ese elemento.

Recomendación: Añadir un atributo aria-label en el código HTML que describa la función exacta del botón (por ejemplo: aria-label="Iniciar sesión" o aria-label="Buscar").

Hallazgo ACC-03 — Saltos de jerarquía en encabezados (Skipped heading level)
Entre las 5 alertas amarillas, la herramienta detectó que la estructura de los títulos de la página salta niveles de forma incorrecta en el código.

Criterio WCAG: 1.3.1 — Información y relaciones (Nivel A).

Impacto: Desorienta a los usuarios que navegan usando el mapa de voz de un lector de pantalla, ya que la información parece desorganizada o fragmentada.

Recomendación: Corregir las etiquetas HTML para que sigan un orden numérico estricto y lógico (pasar de $H1$ a $H2$, y luego a $H3$), sin saltarse ningún nivel intermedio

### B. Operable

- **Hallazgo:** "Indicador de foco invisible en el menú".
- **Impacto:** Un usuario que navega con teclado no sabe dónde está situado.
- **Solución:** Definir un estilo CSS para `:focus` con alto contraste.



### C. Comprensible

- **Hallazgo:** "Los mensajes de error de formulario no son claros".
- **Impacto:** El usuario no sabe cómo corregir el campo para avanzar.
- **Solución:** Vincular el error con el input mediante `aria-describedby`.



### D. Robusto

- **Hallazgo:** "IDs duplicados en el código HTML".
- **Impacto:** Los lectores de pantalla pueden saltarse contenido o confundir elementos.
- **Solución:** Validar el HTML y asegurar identificadores únicos.



El informe deberá organizar los resultados en esta 4 categorias: 

| **Categoría**    | **Qué analizar (Ejemplos)**                                  |
| ---------------- | ------------------------------------------------------------ |
| **Perceptible**  | Contraste de colores, texto alternativo en imágenes (`alt`), subtítulos. |
| **Operable**     | Navegación por teclado, tiempo suficiente para leer, evitar destellos. |
| **Comprensible** | Idioma de la página definido, formularios claros, errores fáciles de corregir. |
| **Robusto**      | Código limpio (HTML válido) para que los lectores de pantalla funcionen. |

Un ejemplo de resultado sería: 

* **Perceptible:**  
  * Error detectado: **Falta de contraste en el botón de reservar**.
  * **Criterio WCAG incumplido:** "Criterio 1.4.3 - Contraste mínimo".
  * **Impacto:** "Los usuarios con visión baja no pueden identificar la acción principal".
  * **Recomendación de mejora:** "Cambiar el color del texto de gris claro a negro (#000000)".

El informe debería dar una **valoracion general de accesibilidad** e incluir al menos **2-3 resultados identificados y clasificados adecuadamente**. 





## 4. Tabla de Hallazgos y Prioridades

Organiza los errores técnicos de forma que el equipo sepa qué arreglar primero.

| **ID**     | **Prioridad** | **Criterio WCAG**          | **Error detectado**                  | **Recomendación Técnica**     |
| ---------- | ------------- | -------------------------- | ------------------------------------ | ----------------------------- |
| **ACC-01** | **Crítica**   | 1.4.3 Contraste            | Texto gris sobre fondo blanco.       | Cambiar a color #333333.      |
| **ACC-02** | **Alta**      | 1.1.1 Contenido no textual | Icono de "Cerrar" sin etiqueta.      | Añadir `aria-label="Cerrar"`. |
| **ACC-03** | **Media**     | 2.4.1 Evitar bloques       | No hay enlace "Saltar al contenido". | Implementar un *Skip Link*.   |


## 5. Conclusiones y Declaración de Conformidad

Resume el estado actual:

- **¿Es el sitio accesible?** (Ej: "El sitio cumple parcialmente con el nivel AA, pero presenta barreras críticas en el proceso de compra").
- **Próximos pasos:** Lista de 3 acciones inmediatas para mejorar la puntuación.













