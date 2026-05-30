# Accesibility Report

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

| ID | Principio POUR | Prioridad | Páginas Afectadas | Criterio WCAG | Error Detectado | Recomendación Técnica |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **ACC-01** | Perceptible | 🔴 Alta | Inicio (General) | 1.4.3 Contraste (AA) | 5 errores de contraste en texto rojo corporativo y descripciones gris medio sobre fondo oscuro. | Cambiar el texto rojo por un tono más claro/brillante, o usar blanco (`#FFFFFF`). Aumentar el brillo de los textos grises pequeños. |
| **ACC-02** | Perceptible | 🔴 Alta | Cabecera | 1.1.1 Contenido no textual (A) | 1 error crítico. Icono interactivo o campo de texto en la zona superior carece de etiqueta/descripción. | Añadir un atributo `aria-label` en el HTML que describa la función exacta (ej. `aria-label="Iniciar sesión"`). |
| **ACC-03** | Perceptible | 🟡 Media | Inicio (General) | 1.3.1 Información y relaciones (A) | Saltos de jerarquía incorrectos en los encabezados (alertas amarillas en WAVE). | Corregir las etiquetas HTML para que sigan un orden numérico estricto y lógico (`<h1>` -> `<h2>` -> `<h3>`) sin saltar niveles. |
| **ACC-04** | Operable | 🟡 Media | Cabecera | 2.4.4 Propósito de los enlaces (A) | Enlaces vacíos o redundantes. Los logotipos o menús actúan como enlaces duplicados hacia el inicio. | Eliminar enlaces duplicados adyacentes o unificar el logotipo y el texto bajo un único contenedor interactivo. |
| **ACC-05** | Operable | 🔴 Alta | General (Botones) | 2.4.7 Foco visible (AA) | Los botones "¡Que gane la mejor!" y "Pedir ahora" no muestran un contorno de alto contraste al navegar con teclado. | Asegurar por CSS un anillo de enfoque claro y llamativo al recibir el foco usando las pseudoclases `:focus` o `:focus-visible`. |
| **ACC-06** | Comprensible | 🟢 Baja | Todas (Navegación) | 3.2.3 Navegación consistente (AA) | Necesidad de asegurar consistencia en el menú superior y botones para no romper la carga cognitiva. | Mantener exactamente el mismo orden, diseño y nomenclatura en el Header y Footer a lo largo de todo el sitio web. |
| **ACC-07** | Robusto | 🟡 Media | Elementos Dinámicos | 4.1.2 Nombre, función, valor (A) | Uso elevado de elementos dinámicos (15 etiquetas ARIA) con riesgo de desactualización si se programan mal. | Verificar manualmente con lector de pantalla que los atributos (como `aria-expanded` o `aria-live`) cambien de estado correctamente. |

## 5. Conclusiones y Declaración de Conformidad

El sitio web cumple parcialmente con el nivel AA de las WCAG 2.1. Aunque la puntuación automatizada de Lighthouse arroja un notable 90/100, la auditoría detallada desvela barreras que impiden una conformidad total.

La solución de diseño web en una sola página (One-Page) cuenta con una buena base semántica, pero adolece de problemas críticos en la percepción del color (textos corporativos rojos que se pierden en el fondo oscuro) y fallos de operabilidad por teclado (ausencia de indicador de foco). Además, la presencia de enlaces interactivos que no conducen a un contenido real o secundario frustra la experiencia del usuario que depende de tecnologías asistivas.

Próximos Pasos (Acciones Inmediatas)
Para solventar las barreras identificadas y consolidar el nivel AA, se deben priorizar las siguientes tres acciones de forma urgente:

Garantizar la Navegación por Teclado: Implementar mediante CSS las reglas de :focus-visible en todos los elementos interactivos (botones de compra y votación) para asegurar que el foco sea perfectamente visible.

Corregir la Paleta de Contraste: Modificar el código de color de los eslóganes y textos críticos bajo fondo oscuro, sustituyendo el rojo corporativo actual y el gris atenuado por variantes que superen el ratio mínimo exigido por el nivel AA.

Complertar la pagina: Completar los enlaces de la pagina para que estos tengan una redireccion y no haya enlaces los cuales no redirijan a ningun lado ya que esto para un usuario puede ser frustante.











