# **ITCSS** (Inverted triangle CSS)
Es una arquitectura de trabajo que se basa en un triángulo invertido, dividiendo las propiedades CSS en función de su especifidad e importancia.

Estandariza las mejores prácticas para una forma de trabajar que facilita el Desarrollo Web con hojas de estilo CSS y que facilita su crecimiento y adaptabilidad a medio y largo plazo,

![image](https://user-images.githubusercontent.com/73679190/236115111-b060ee9d-b6e9-46b2-b662-053f07fa872f.png)

En el lado izquierdo, se muestra la estructura aconsejable con los nombres de las carpetas: Settings, Tools, Generic, Elements, Objects, Components y Utilities. El triángulo representa el alcance y características del código CSS que iría en cada una de esas carpetas, prestando atención a criterios como Magnitud, Especificidad y Claridad.

Aunque exista muchas estructuras aconsejable, realmente no existe una estructura de carpetas por defecto, y la profundidad de la especifidad depende de cada equipo.

No requiere de procesadores como SASS o LESS

- Primer ejemplo:
1. Settings -> Declararemos las variables y los preprocesadores, y las situaremos en esta carpeta.
2. Tools -> Los mixins y funciones, junto con los preprocesadores, irán en esta carpeta.
3. Generic -> El código genérico del proyecto, el reset de CSS, el Normalize o tus propios estilos, son los que incluiremos en esta carpeta.
4. Element -> Para  los estilos que afectan a los elementos del HTML. No incluiremos el estilo para las clases.
5. Object -> Aquí sí, incorporaríamos las clases y colocaríamos todo lo relacionado con el layout.
6. Components -> Todo lo que afecte a los diferentes bloques de nuestro documento, navegador, botones, recuadros de utilidades, migas de pan, cabecera, buscador, botones sociales, etc., debería de ir en esta carpeta. Dependiendo de las necesidades que tenga el proyecto, la carpeta 'Components' tendrá más o menos ajustes, como es lógico
7 -> Utilities. Para finalizar, en esta carpeta colocaríamos utilidades que sobrescriban estilos significativos (incompatibilidades con navegadores, por ejemplo).

- Segundo ejemplo:
1. Settings -> Variables, font-family, resets...
2. Generics -> Estilos génericos por defecto
3. Tools -> Funciones, Media queries, Mixins, etc...
4. Elements -> Elementos HTML (botones, inputs, etc)
5. Components -> Estrutura de elementos (Sidebar, modal, header, sections, articles)
6. Overs -> Sobreescritura de estilos (se permite usar !importan, aunque es bastante cuestionable el uso del mismo)

### Salida CSS (CSS output)
El orden de las carpetas que hemos puesto es el que tendrá el código CSS resultante. La línea azul que aparece en la derecha del triángulo y donde pone CSS Output, nos indica que las primeras dos carpetas señaladas no tienen salida, es decir, no se crea código CSS. Es decir, se usarán con el resto de las carpetas, pero no tendrán sentido hasta que no se utilicen.

### Características del código por carpetas
La parte centrar del triángulo tiene las tres características que dispone el código CSS:

- Magnitud. El código que tenemos en las carpetas superiores tienen una mayor magnitud que las inferiores. Por ejemplo, si en Settings definimos el color rojo en una variable CSS, este afectará a todos los elementos que utilicen esa variable.
- Claridad. Si bajamos en la lista de carpetas tendremos más claridad sobre dónde se usan los estilos.
- Especificidad. Obtendremos una mayor especificidad del código a medida que bajamos en la lista de carpetas, por lo tanto deberá ser mayor la fuerza del selector y por tanto sus propiedades de estilo.



<!-- TODO: Vulgarizar el cotenido -->
