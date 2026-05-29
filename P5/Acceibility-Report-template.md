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

Hallazgo ACC-04 — Enlaces vacíos o redundantes (Suspicious/Broken link)
Asociado a 1 de las alertas de WAVE en la cabecera, se detecta que los logotipos superiores o elementos del menú actúan como enlaces hacia la misma página de inicio sin una separación ni descripción clara.

Criterio WCAG: 2.4.4 — Propósito de los enlaces (Nivel A).

Impacto: Usuarios que navegan con teclado o lectores de pantalla pasarán dos veces por el mismo destino de forma repetitiva, ralentizando su navegación y generando confusión.

Recomendación: Eliminar los enlaces duplicados adyacentes o unificar el logotipo y el texto bajo un único contenedor interactivo con un destino claro.

Hallazgo ACC-05 — Ausencia de indicador de foco visual (Focus Visible sospechoso)
Al evaluar el diseño general, los botones como "¡Que gane la mejor!" y "Pedir ahora" no muestran en sus estados por defecto un contorno de alto contraste preparado para la selección mediante teclado.

Criterio WCAG: 2.4.7 — Foco visible (Nivel AA).

Impacto: Un usuario que navegue sin ratón utilizando la tecla Tab no sabrá visualmente en qué botón o sección de la pantalla está posicionado en cada momento.

Recomendación: Asegurar por CSS que todos los elementos interactivos muestren un anillo de enfoque claro y llamativo al recibir el foco (usando :focus o :focus-visible con un color contrastado como el blanco).


### C. Comprensible

Hallazgo ACC-09 — Consistencia en la navegación y etiquetas
La estructura de navegación superior ("Inicio", "Pide y Vota", "Salón de la Fama") y los botones de acción deben mantener un comportamiento predecible en todo el sitio web.

Criterio WCAG: 3.2.3 — Navegación consistente (Nivel AA).

Impacto: Si al cambiar de sección el menú se mueve de lugar o los botones cambian drásticamente su diseño o nombre para realizar la misma acción, se rompe la carga cognitiva del usuario, generando desorientación.

Recomendación: Mantener exactamente el mismo orden, diseño y nomenclatura en el encabezado (Header) y pie de página (Footer) en todas las páginas del proyecto.


### D. Robusto

WAVE detectó un uso elevado de elementos dinámicos (15 etiquetas ARIA). Estas etiquetas sirven para explicar a las tecnologías asistivas qué hace un componente cuando cambian cosas en la pantalla sin recargar la página.

Criterio WCAG: 4.1.2 — Nombre, función, valor (Nivel A).

Impacto: Si estos atributos ARIA están mal programados, quedan desactualizados o apuntan a elementos incorrectos, el lector de pantalla le dará información falsa a un usuario invidente sobre el estado real de la web (por ejemplo, anunciará que un menú está "cerrado" cuando en realidad visualmente ya está "abierto").

Recomendación: Verificar manualmente con un lector de pantalla que cada uno de los 15 atributos ARIA (como aria-expanded, aria-hidden o aria-live) cambie su estado correctamente en el código cuando el usuario interactúe con la web.

## 4. Tabla de Hallazgos y Prioridades

## 4. Tabla de Hallazgos y Prioridades

| ID | Prioridad | Páginas afectadas | Criterio WCAG | Error detectado | Recomendación técnica |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **ACC-01** | 🔴 Alta | Carta, Pedir Online | 1.4.3 Contraste | Texto sobre tarjetas rojas y grises sin contraste suficiente sobre el fondo oscuro. | Cambiar texto a un tono más claro/brillante, o fondo a `#FFFFFF`. |
| **ACC-02** | 🔴 Alta | Todas | 1.1.1 Contenido no textual | Elemento interactivo / campo de texto en cabecera sin etiqueta descriptiva (`label`). | Añadir `aria-label="Iniciar sesión"` o `aria-label="Buscar"` según corresponda. |
| **ACC-03** | 🟠 Media | Reseñas | 1.3.1 / 3.3.2 | Campos de formulario y opiniones sin etiquetas explícitas o con saltos de jerarquía en títulos. | Añadir la etiqueta `<label>` asociada a cada input y reestructurar títulos secuencialmente. |
| **ACC-04** | 🟠 Media | Todas | 2.4.6 Encabezados | Títulos visuales no marcados en orden secuencial descendente (`<h1>` / `<h2>` / `<h3>`). | Implementar una jerarquía estricta de headings en el HTML sin saltarse niveles intermedios. |
| **ACC-05** | 🟠 Media | Todas | 1.3.1 Info y relaciones | Estructura sin regiones semánticas principales ni landmarks definidos (`<main>`, `<nav>`, `<footer_>`). | Añadir las etiquetas nativas de landmarks de HTML5 para delimitar las zonas de la página. |
| **ACC-06** | 🟡 Baja | Pedir Online | 2.4.4 Propósito de enlaces | Enlace redundante o vacío en logotipos superiores de cabecera sin texto descriptivo. | Eliminar el enlace duplicado adyacente o añadir un atributo `aria-label` explícito. |
| **ACC-07** | 🟡 Baja | Reserva | 3.2.4 Identificación consistente | Selector de hora configurado en formato AM/PM para una interfaz española. | Cambiar las opciones de selección del componente nativo a formato horario de 24h. |
| **ACC-08** | 🟡 Baja | Todas | 3.2.4 Identificación consistente | Presencia de 3 bloques de texto subrayados en el cuerpo de la web que no son enlaces. | Eliminar el subrayado decorativo de los textos no enlazados para evitar confusión. |

## 5. Conclusiones y Declaración de Conformidad

Resume el estado actual:

- **¿Es el sitio accesible?** (Ej: "El sitio cumple parcialmente con el nivel AA, pero presenta barreras críticas en el proceso de compra").
- **Próximos pasos:** Lista de 3 acciones inmediatas para mejorar la puntuación.













