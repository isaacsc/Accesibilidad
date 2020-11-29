La navegación por teclado es especialmente importante tanto para los usuarios con discapacidad motora como para los usuarios con discapacidad visual que dependen de un lector de pantalla. Un error de UI muy común es sacar elementos del DOM fuera del viewport manteniendo sus nodos "enfocables". Un menú desplegable o una modal son ejemplos clásicos.

La propiedad HTMLElement **inert** es un booleano que, cuando está presente, hace que el navegador "ignore" los eventos de entrada del usuario para el elemento, incluidos los eventos de foco y los eventos de tecnologías de asistencia. El navegador también puede ignorar la búsqueda de páginas y la selección de texto en el elemento. 

Actualmente este atributo esta en fase de desarrollo([uso mediante flags](https://developer.mozilla.org/en-US/docs/Web/API/HTMLElement/inert)) en los navegadores por lo que es necesario usar polyfill.

WICG inert polyfill
[https://github.com/wicg/inert](https://github.com/wicg/inert)