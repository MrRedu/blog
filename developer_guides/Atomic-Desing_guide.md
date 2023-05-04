# **Atomic Desing**

## **⚛️ Los 5 niveles del Atomic Design ⚛️**
![image](https://user-images.githubusercontent.com/73679190/236111663-e53c9e72-5ee4-43ea-b808-21411379dac3.png)

- ### Nivel 1: **Átomos**

Un átomo es la unidad de partículas más pequeña que puede existir.

Aplicado al diseño, hablamos de átomos cuando hablamos de elementos UI que por sí solos tienen alguna funcionalidad: botones, cards, avatares, inputs de formulario… pero también las tipografías, paleta de colores, espaciados, párrafos…

Ejemplos:
1. Tipografía; heading(1, 2, 3...), párrafos del body, labels <br>
2. Iconos, botones, campos del formulario, paleta cromática <br>
3. Avatares, etiquetas

Cada uno de ellos, tiene sus propias variaciones que representan estados: seleccionados, con foco, deshabilitados, hover, etc.

![image](https://user-images.githubusercontent.com/73679190/236111711-bee75020-a3cc-485e-91cb-8e19c5d14094.png)

- ### Nivel 2: **Moléculas**

Una molécula es una unión de dos o más átomos.

Del mismo modo, una molécula en Atomic Design es la unión de diferentes átomos para formar un elemento UI más complejo.

Ejemplos:
1. Un campo de formulario con un botón de enviar y un label <br>
2. Un rectángulo con un avatar, nombre y ubicación del usuario (es decir, avatar con texto en un área determinada) <br>
3. Un icono junto con un texto que ocupa una área determinada.

![image](https://user-images.githubusercontent.com/73679190/236111766-63545367-fa57-4cf1-b2e0-b5b9bddcb09b.png)

- ### Nivel 3: **Organismos**

Cuando llegamos al tercer nivel estamos hablando de elementos que son más complejos, ya que son sumas de los niveles anteriores.

**No debemos perder de vista que estamos hablando de elementos de UI formados por moléculas (que a su vez son átomos) y que, por encima de todo, pueden repetirse.**

En este sentido, podríamos considerar un organismo una unión de moléculas. 

Ejemplos:
1. Cuando juntamos los rectángulos con el avatar y los nombres
2. Cuando unimos los iconos y texto para crear una navegación de una aplicación

![image](https://user-images.githubusercontent.com/73679190/236111785-56ba154c-f191-48cc-9e30-83bc50f8bfd8.png)

- ### Nivel 4: **Plantillas**

En esencia, lo que consideraríamos “plantillas” dentro del *Atomic Design* no dejarían de ser los *wireframes*: una unión de distintos organismos que forman una página o una aplicación.

Se trata de un entregable de alta o alta fidelidad que no termina de ser el diseño final. Para que nos entendamos, se trata del “esqueleto” de la aplicación o página web.

- ### Nivel 5: **Páginas**

Este es el último nivel del *Atomic Design*. Son en realidad el diseño final que ya contiene las imágenes y otros detalles que hacen que ese archivo ya esté listo para el desarrollo o, en su defecto, test con usuarios o el equipo.

<hr>

## ¿Para qué sirve el Atomic Design y ventajas?

La metodología del Atomic Design es muy útil porque nos obliga a coger cada diseño y diseccionarlo para poder separar cada átomo.

Esto nos ayudará a plantear los elementos de interfaz básicos con los que trabajar. Con esta base, después podrán ir creando fácilmente las moléculas, organismos y, finalmente, el diseño final.

El Atomic Design obliga a plantear bien de inicio el “sistema de diseño”, con las tipografías, jerarquías, paleta de colores, etc. que se necesitarán en un momento dado.

Ayuda a planificar y, lo que es todavía mejor, permite generar un sistema que en un futuro podrá asumir fácilmente el diseño de nuevas funcionalidades, ya que probablemente ya estarán los átomos creados y solo habrá que “combinarlos” de otro modo para crear moléculas y organismos distintos

Las ventajas del Atomic Design son claras:

- Facilita la creación de la guía de estilo
- Permite hacer más rápido los prototipos, puesto que los elementos ya existirán
- Hace más rápido el proceso de actualizar el diseño del producto y/o añadir nuevas funcionalidades, ya que los cambios no harán que se deba programar todo desde cero.
- Menos componentes hará el diseño y el código más consistentes y eficientes.
- Permite reutilizar átomos para crear cualquier diseño que se requiera.

<hr>

## Aclaración:
Esto no es más que un copy/paste de la página que está más abajo. El único fin es tener una guía más cercana para completar el proyecto aplicando esta metodología. Ninguna imagen es de mi propiedad.
## Webgrafía
- [Atomic Desing](https://www.uifrommars.com/atomic-design-ventajas/)
