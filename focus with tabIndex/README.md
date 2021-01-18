## Control del foco con tabIndex
Siempre que sea posible, es conveniente utilizar elementos HTML nativos. La etiqueta del botón, por ejemplo, es muy fácil de usar y tiene soporte de teclado y semántica incorporados. 

Pero hay ocasiones en las que es necesario crear algo que no tiene un elemento nativo correspondiente. En estos casos, es importante recordar agregar un soporte de teclado crucial para que todos sus usuarios puedan acceder a su contenido. 

El primer paso es asegurarse de que un usuario realmente pueda hacer foco sobre el. Para lograr esto, puede usar el atributo tabindex.

### Estados tabIndex
- **tabindex="0"**: Inserta un elemento en el orden natural de la navegación. El elemento puede tomar el foco si se presiona la tecla Tab, y el elemento puede tomar el foco mediante una llamada a su método *focus()*
- **tabindex="-1"**: (Valor negativo) Quita un elemento del orden natural de la navegación, pero el elemento todavía puede tomar el foco mediante una llamada a su método *focus()*.
- **tabindex="5"**: Todo tabindex superior a 0 hace saltar al elemento al principio del orden natural de la navegación. Si existen varios elementos con un tabindex superior a 0, el orden de la navegación comienza desde el valor más bajo que sea mayor que cero y va subiendo desde ahí. El uso de un tabindex superior a 0 se considera un **antipatrón**.