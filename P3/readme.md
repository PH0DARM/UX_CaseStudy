- Moodboard (diseño visual + logotipo)   
- Landing Page
- Mockup: LAYOUT HI-FI
- Publicación del Case Study

## Paso 3. Mi UX-Case Study (diseño)

### 3.a Moodboard
![Moodboard](Moodboard.png)

Con este tablero se ha querido transmitir una identidad de marca que fusiona la tradición japonesa con la energía del pop art moderno, específicamente a través de la estética del anime. El objetivo es proyectar una personalidad joven, vibrante y cercana, donde la elección de colores (verde para la frescura y naranja para la calidez) busca evocar un ambiente orgánico pero lleno de vida. Al incluir referencias visuales de comunidad y cultura, se intenta decir al usuario que este no es solo un lugar de comida rápida, sino un espacio con alma, historia y un lenguaje propio que entiende y celebra sus mismos gustos.

### 3.b Landing Page
![LandingPage](LandingPage.png) 

En la landing page, el mensaje central que se ha querido transmitir es la unión a través de la gastronomía, utilizando el ramen como el hilo conductor de una experiencia social auténtica. A través de una jerarquía visual limpia y un mensaje directo ("El sabor que nos une"), se busca eliminar cualquier barrera entre el cliente y el restaurante, transmitiendo una sensación de transparencia, calidad y pasión. El diseño no solo vende un producto, sino que invita a formar parte de una comunidad, asegurando al usuario que encontrará un espacio acogedor donde la tradición se sirve con un toque moderno y una facilidad de uso impecable.

### 3.c Guidelines
# Guía de Arquitectura y Componentes: Ramen Pa'ya (V3)

## 1. Concepto y Propuesta de Valor
**Ramen Pa'ya** es una experiencia híbrida que combina la gastronomía japonesa auténtica con una comunidad activa de fans del anime. Bajo el lema **"Menos scroll, más roll"**, la interfaz prioriza la conexión real entre usuarios y una facilidad de uso excepcional.

## 2. Identidad Visual

### 2.1 Paleta de Colores
Se han seleccionado tonos que equilibran la frescura de los ingredientes con la calidez de la cultura japonesa:

| Muestra | Color | Uso en la Interfaz |
| :--- | :--- | :--- |
| #1A4A3A | **Verde Marino (#1A4A3A)** | Navegación, botones primarios y fondos de sección. |
| #D35400 | **Naranja Koi (#D35400)** | CTAs críticos, acentos visuales y fechas de eventos. |
| #FDF5E6 | **Crema Hueso (#FDF5E6)** | Fondo general (Background) para evitar la fatiga visual. |
| #333333 | **Gris Carbono (#333333)** | Textos principales y trazos de ilustraciones. |

### 2.2 Tipografía
* **Poppins (Bold/Regular):** Utilizada para todos los encabezados (H1-H4) y etiquetas de botones para transmitir modernidad y legibilidad.
* **Noto Sans JP:** Empleada en textos de párrafo y contenido secundario para aportar un toque cultural japonés y optimizar la lectura de caracteres especiales.

## 3. Layout Global y Navegación
La estructura se basa en tres áreas constantes para garantizar la consistencia:

1.  **Navbar (Sticky):** Contiene el logotipo, enlaces centrales (Carta, Reservas, Eventos, Comunidad, Contacto) y el acceso a "Mi Cuenta".
2.  **Área de Contenido:** Espacio dinámico para las diferentes secciones.
3.  **Footer:** Información legal, políticas de privacidad y copyright.

## 4. Anatomía de Páginas y Componentes

### 4.1 Página de Inicio (Home)
Presenta un patrón de **Hero Section** con texto descriptivo a la izquierda e imagen de impacto a la derecha. El botón **"Ver la carta"** destaca como el CTA primario. Incluye también una fila de tarjetas para **Eventos Destacados**.

### 4.2 Carta Digital (Navigation Tabs)

Utiliza un sistema de pestañas para la categorización eficiente del menú:

| Componente | Comportamiento |
| :--- | :--- |
| **Tabs de Categoría** | Filtro rápido (Entrantes, Ramen, etc.) que refresca el contenido sin recargar la página. |
| **List Item (Plato)** | Contenedor horizontal con imagen, título y descripción. |

### 4.3 Formulario de Reserva
Diseñado con campos de gran tamaño para facilitar la interacción:
* **Input de Número:** Para la selección de comensales.
* **Date & Time Picker:** Selectores específicos para fecha y hora (intervalos de 30 min).
* **Botón de Acción:** De ancho completo para optimizar el uso en dispositivos móviles.

### 4.4 Dōjin Club (Community Feed)
Espacio de interacción social que combina un **Post Composer** (para publicar texto e imágenes) con un **Feed de Actividad** y una barra lateral de tendencias.

### 4.5 Perfil de Usuario (Dashboard)
Organizado mediante widgets que muestran el avatar, métricas rápidas (puntos, reseñas, visitas) y un historial de actividad reciente.

## 5. Estados de Componentes
* **Hover State:** Las tarjetas se elevan con una sombra sutil y los botones oscurecen su color un 10%.
* **Empty States:** Ilustraciones estilo anime con mensajes motivadores cuando no hay contenido disponible.
* **Loading State:** Spinners personalizados con la forma de un cuenco de ramen girando.

## 6. Adaptabilidad (Responsive Design)
El diseño se adapta de una grilla de 3 o 4 columnas en escritorio a formatos verticales optimizados para dispositivos móviles.


### 3.d Mockup
![Método UX](img/mockup.png) 
----

>>> Consiste en tener un Layout en acción. Un Mockup es un prototipo HTML que permite simular tareas con estilo de IU seleccionado. Muy útil para compartir con stakeholders
>>>

### 3.e Conclusion

<br>
