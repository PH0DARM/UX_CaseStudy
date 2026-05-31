# Practica 4: Exportación + Documentación 

## 4.a Exportación a HTML/React

[Enlace exportado](https://bot-excel-33662561.figma.site)


## 4.b Documentación con Storybook

En este apartado se ha llevado a cabo la documentación, visualización y aislamiento del sistema de diseño de la aplicación web Ramen Pa'ya utilizando Storybook.

A través de esta herramienta, se han organizado y testeado de manera independiente tanto los componentes atómicos como las páginas completas de la plataforma. Esto permite verificar de forma aislada la consistencia visual, la interactividad de los elementos (como botones y formularios de registro/reserva) y la accesibilidad de las diferentes interfaces antes de su integración y despliegue final.

## 4.c Puntos fuertes y debiles

### Puntos Fuertes

El enfoque "Ramen + Cultura Anime/Manga" está perfectamente integrado. El uso de ilustraciones de fondo en el login, el foro "Dōjin Club", los talleres de manga y el avatar de perfil crean una experiencia inmersiva muy atractiva para el público objetivo.

La paleta cromática se mantiene unificada en todas las pantallas. La tipografía y el estilo de las tarjetas (cards) dan mucha cohesión al diseño, permitiendo que se adapte a la vision de todo tipo de publicos.

### Puntos Debiles

La pantalla de la carta es extremadamente larga. Si el usuario está abajo del todo (en bebidas) y quiere volver a entrantes, tendrá que hacer muchísimo scroll.

En la sección de Reservas, el texto blanco "Tu mesa te espera" y los campos del formulario están situados directamente sobre una fotografía oscura de un local. Si la imagen cambia o en ciertas pantallas brilla mucho, se puede perder legibilidad.

Los formularios de inicio de sesión y registro tienen los campos muy separados verticalmente dentro de la tarjeta blanca, dejando demasiado aire flotando en medio

## 4.d Conclusiones

Por un lado, la exportación a HTML/React (5.a) ha permitido materializar la interfaz en un entorno web real, trasladando con éxito toda la lógica y funcionalidad del sitio (desde la navegación por la carta hasta la interactividad en los formularios de reserva, login y el foro de la comunidad). Por otro lado, la arquitectura de documentación en Storybook (5.b) dota a la plataforma de un sistema de diseño perfectamente aislado, testeado y modular.

En definitiva, la combinación de un código final completamente operativo junto a una biblioteca de componentes perfectamente documentada no solo asegura la fidelidad visual del producto actual, sino que garantiza la mantenibilidad, escalabilidad y eficiencia de la aplicación ante futuras actualizaciones del software.
