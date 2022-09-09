<H1>CURSO CSS UNI</H1>

- [**_Introduccion_**](#introduccion)
  - [Tipos de CSS](#tipos-de-css)
  - [Selector ID (#)](#selector-id-)
  - [Clases (.)](#clases-)
  - [Selector Universal (\*)](#selector-universal-)
  - [Agrupar Elementos HTML y CSS](#agrupar-elementos-html-y-css)
  - [Sunclases en CSS](#sunclases-en-css)
- [**_COLORES, BORDES Y MAS_**](#colores-bordes-y-mas)
  - [Colores por nombre](#colores-por-nombre)
  - [Colores y Bordes](#colores-y-bordes)
  - [Comentarios](#comentarios)
  - [Manejo de Bordes](#manejo-de-bordes)
  - [Ancho de Bordes](#ancho-de-bordes)
    - [Como aplicar una medida distinta en cada lado?](#como-aplicar-una-medida-distinta-en-cada-lado)
- [**_Codigo de Colores en Bordes_**](#codigo-de-colores-en-bordes)
    - [Como aplicar un color distinto en cada lado?](#como-aplicar-un-color-distinto-en-cada-lado)
  - [Redondeo de bordes](#redondeo-de-bordes)
    - [Dominar las esquinas](#dominar-las-esquinas)
  - [Esquina Redondeada con fondo](#esquina-redondeada-con-fondo)
  - [Esquina redondeada con contorno](#esquina-redondeada-con-contorno)
  - [Borde con imagen de fondo](#borde-con-imagen-de-fondo)
  - [Borde Circular](#borde-circular)
  - [Fondos Multiples](#fondos-multiples)
    - [Cuando la  imagen es grande](#cuando-la--imagen-es-grande)
    - [Cuando queremos sobreponer una imagen encima de otra](#cuando-queremos-sobreponer-una-imagen-encima-de-otra)
    - [Para que la imagen ocupe todo el contenido usaremos](#para-que-la-imagen-ocupe-todo-el-contenido-usaremos)
- [**_BOX MODEL_**](#box-model)
  - [Ancho del Elemento Box Model](#ancho-del-elemento-box-model)
  - [Outline](#outline)
  - [Outline-Offset](#outline-offset)
  - [**_PADDING_**](#padding)
  - [Box Sizing](#box-sizing)
  - [Propiedad Max-Width](#propiedad-max-width)
  - [Propiedad Margin: Auto](#propiedad-margin-auto)
  - [Propiedad **_inherit_**](#propiedad-inherit)
  - [Concepto de margin collapse](#concepto-de-margin-collapse)
- [**_Manejo de colores_**](#manejo-de-colores)
  - [Color por nombre HTML](#color-por-nombre-html)
  - [Manejo de colores **RGB**](#manejo-de-colores-rgb)
  - [Codigo de colores **Hexadecimal**](#codigo-de-colores-hexadecimal)
  - [Codigo de colores **HSL**](#codigo-de-colores-hsl)
- [**_Manejo de fondos_**](#manejo-de-fondos)
- [**Formato de texto**](#formato-de-texto)
- [**Fuentes**](#fuentes)
- [**Estilos de funete**](#estilos-de-funete)
- [Propiedad de Font-Size](#propiedad-de-font-size)
- [Google Fonts](#google-fonts)
- [Efectos con Google Fonts](#efectos-con-google-fonts)
- [**Atributo font**](#atributo-font)
- [Menejo de Iconos](#menejo-de-iconos)
  - [Iconos Bootstrap](#iconos-bootstrap)
  - [Pasos para usar los iconos en Bootstrap](#pasos-para-usar-los-iconos-en-bootstrap)
- [Iconos de Google](#iconos-de-google)
- [Iconos de Ionicons](#iconos-de-ionicons)
- [**Propiedad Display**](#propiedad-display)
  - [Display Block](#display-block)
  - [Display inline](#display-inline)
  - [Display None](#display-none)
- [**Posicionamiento de Elementos**](#posicionamiento-de-elementos)
  - [Centrar Div](#centrar-div)
  - [Posicionamiento Estatico](#posicionamiento-estatico)
  - [Tipos de posicionamiento](#tipos-de-posicionamiento)
  - [Posicionamiento Relativa](#posicionamiento-relativa)
  - [Posicionamiento Fixed (ajustado)](#posicionamiento-fixed-ajustado)
  - [Posicionamiento Absoluta](#posicionamiento-absoluta)
  - [Posicionamiento Sticky (pegajoso)](#posicionamiento-sticky-pegajoso)
  - [Posicionamiento Z-index](#posicionamiento-z-index)
  - [Propiedad Overflow](#propiedad-overflow)
  - [Propiedad Float](#propiedad-float)
  - [Propiedad Display Inline-Block](#propiedad-display-inline-block)
  - [**Menu** con la propiedad Display Inline-Block](#menu-con-la-propiedad-display-inline-block)
- [**Selectores**](#selectores)
  - [Selectores Combinados](#selectores-combinados)
    - [Selectores Decendientes](#selectores-decendientes)
    - [Selector Child](#selector-child)
    - [Selector Sibling (Adyacente)](#selector-sibling-adyacente)
  - [Pseudo Clases](#pseudo-clases)
- [Pseudo Elementos](#pseudo-elementos)
- [Transparencia](#transparencia)
  - [Transparencia en imagenes](#transparencia-en-imagenes)
- [**Gradientes**](#gradientes)

## **_Introduccion_**

### Tipos de CSS

- Inline CSS

```css
<h1 style="color: blue; text-align: center; font-size: 100px">Universidad CSS</h1>
```

- Internal CSS

```css
<style>
h1{
  color:red;
  text-align: right;
  }
</style>
```

- External CSS
  - Esta es la mejor practica

> Podemos usar las teclas Ctrl + Space para selecionar las carpeta del css y despues seleccionar el archivo css

```
<link rel="stylesheet" href="css/estilos.css">
```

### Selector ID (#)

> Este tipo de selector lo usaremos para modificar un elemento html que <span style="color:red">**es unico**</span> dentro de nuestra pagina y no se repite, como por ejemplo el **H1**

```
<h1 id="titulo">Universidad CSS</h1>
```

### Clases (.)

> No usar numeros al inicio y si son dos palabras separar con \_ o -. Eso lo usaremos para <span style="color:red">**reutilizar**</span> en otros elementos de html

> Para agregar otra clase al mismo elemento so hay que dejar un espacio e insrtar el nobre de la segunda clase.

```
<p class="centrar texto_grande">Iniciando el curso de CSS</p>
<p class="centrar">www.globalmentoring.com.mx</p>
```

### Selector Universal (\*)

> Este tipo de selector se aplica a toda nuestra pagina HTML. Como buena practica lo posicionaremos al inicio de nuestro documento css.

```css
* {
  background-color: ghostwhite;
  color: cornflowerblue;
}
```

### Agrupar Elementos HTML y CSS

> Esto para aplicar los mismos estilos a varios elementos html o tambien clases o selctores. Los podemos convinar o agrupar.

```css
h1,
h2,
p,
div {
  color: crimson;
  text-align: center;
}
```

### Sunclases en CSS

> Utilizamos una clase que se aplicara a los elementos de html que sean del mismo tipo que seleccionamos (etiqueta p).

```css
p.centrar {
  text-align: center;
}
```

```html
<p class="centrar">Iniciando el curso de CSS</p>
<p class="centrar">www.globalmentoring.com.mx</p>
```

## **_COLORES, BORDES Y MAS_**

### Colores por nombre

[Pagina de Colores](https://htmlcolorcodes.com/color-names/ "enlase")

> RGB
>
> > R = Red(Rojo)  
> > G = Green(Verde)
> > B = Blue(Azul)

> hsl
>
> > h = hue(color, matiz)  
> > s = saturation(saturacion)
> > l = lightness(iluminacion)

> Los navegadores modernos soportan 140 colores con nombre. Los podemos usar en el código HTML y CSS por nombre, código Hex o el valor RGB.
> [Pagina de los colores](https://htmlcolorcodes.com/es/nombres-de-los-colores/)

### Colores y Bordes

Border se refiere al contorno, y los 10px al ancho de la linea del contorno, solid al tipo de contorno y por ultimo el color del la linea del border.

```css
.rojo {
  border: 10px solid firebrick;
}
```

![Border](img/borderColorCss.png)

![Border](img/borderNavegador.png)

### Comentarios

```css
/*background-color: black;*/
```

### Manejo de Bordes

De esta forma solo modificamos el tipo de borde

```css
.discontinuo {
  border-style: dashed;
}
```

De esta forma solo modificamos el tipo y el grosor dl border

```css
.doble {
  border: 5px double;
}
```

Forma simplificada

```css
.solido {
  border: 10px solid red;
}
```

Forma completa

```css
.surco {
  border-width: 10px;
  border-style: groove;
}
```

De esta forma podemos modificar todos los lados del borde

```css
.mixto {
  border-style: dotted solid dashed double;
}
```

### Ancho de Bordes

#### Como aplicar una medida distinta en cada lado?

```css
.punteado {
  border-style: dotted;
  border-width: 10px 5px 3px 2px;
}
```

Para poder visualizar los hanchos de los bordes podemos usar la consola y desplegar que medidas se estan aplicando.

![Medidas por consola](img/medidasBorde.png)

## **_Codigo de Colores en Bordes_**

#### Como aplicar un color distinto en cada lado?

```css
.punteado {
  border-style: dotted;
  border-width: 10px 5px 3px 2px;
  border-color: crimson hotpink gold lime;
}
```

- Un valor de 1 en la transparencia = color completo.
- Un valor de 0 en la transparencia = complatamente transparente.
- Un valor de .5 en la transparencia = 50% de transparencia.

```css
.discontinuo {
  border-style: dashed;
  border-width: thick;
  /*thin, medium, thick*/
  border-color: hsla(203, 39%, 44%, 1);
  border-color: hsla(203, 39%, 44%, 0);
  border-color: hsla(203, 39%, 44%, 0.5);
}
```

### Redondeo de bordes

> Podemos crear links que parescan botones, pero mas estilizados.

Cuando el `border-radius: 20px;` lleva un unico valor se proporsiona en totas las esquinas

```css
.solido {
  border: solid red;
  border-width: 5px;
  border-radius: 20px;
}
```

#### Dominar las esquinas

```css
#b4 {
  border-radius: 15px 50px 30px 5px;
  background-color: red;
  padding: 20px;
  width: 200px;
  height: 150px;
}
```

- En el border-radius **15px** es la esquina superior izquierda.
- En el border-radius **50px** es la esquina superior derecha.
- En el border-radius **30px** es la esquina inferior derecha.
- En el border-radius **5px** es la esquina inferior izquierda.

Aqui seria de forma simplificada

```css
.redondeado {
  border: 5px solid blueviolet;
  border-radius: 20px 0px 10px 0px;
}
```

> :bulb: **Tip:** Con `border-radios:` <span style="color: yellow"> **Podemos hacer las esquinas redondeadas**</span>

### Esquina Redondeada con fondo

> :bulb: **Tip:** Usaremos `background-color:`

> :bulb: **Tip:** El borde se puede ver hasta que le damos un color y unas medidas.

```css
#b1 {
  border-radius: 25px;
  background-color: greenyellow;
  padding: 20px;
  width: 200px;
  height: 150px;
}
```

### Esquina redondeada con contorno

> :bulb: **Tip:** Usaremos `border:`

```css
#b2 {
  border-radius: 25px;
  border: 2px solid blueviolet;
  padding: 20px;
  width: 200px;
  height: 150px;
}
```

### Borde con imagen de fondo

> :bulb: **Tip:** Usaremos `background-image:`  
> :bulb: **Tip:** Y para darle una dimencion usaremos `background-position:` y para indicar que parte de l imagen se mostrara `left top;`  
> :bulb: **Tip:** si no ocupa todo el tamano que se repita con `background-repeat: repeat;`

```css
#b3 {
  border-radius: 25px;
  background-image: url(fondo.jpg);
  background-position: left top;
  background-repeat: repeat;
  padding: 20px;
  width: 200px;
  height: 150px;
}
```

### Borde Circular

> :bulb: **Tip:** Para hacerlo circular usaremos `border-radius: 50%;` pero utilizaremos % en ves de pixeles

```css
#b5 {
  border-radius: 50%;
  background-color: blue;
  padding: 20px;
  width: 200px;
  height: 150px;
}
```

![bordes](img/bordescolor.png)

### Fondos Multiples

> :bulb: **Tip:** Cuando la imagen es mas pequena que el marco se repite, en ese caso usaremos `no-repeat`

`background: url(img/gato.png) top 40px left 40px / 80px no-repeat;`

backgruound(ruta)(posicion)(dimencion) no-repeat  
valores (top, right,bottom, left, center)
       arriba, derecha, abajo, izquierda, cdntro.

#### Cuando la  imagen es grande

usaremos la dimencion, para hacerlo mas pequeno y para no repetir la imagen solo usarenos no-repiear

#### Cuando queremos sobreponer una imagen encima de otra

Primero llamaremos a la imagen que va estar enciama `background: url(img/plato.png) center/ 180px no-repeat,` y usaremos una coma para ceparar y llamar a la segunda imagen `url(img/mesa.png) center/`lo separamos con diagonal y usaremos cover  para que puedan convivir las 2 imagenes juntas `cover` y por ultimo para no tener ningun problema usaremos `no-repeat;`

#### Para que la imagen ocupe todo el contenido usaremos 

`background-size: contain;`

## **_BOX MODEL_**

El padding y el Margin son transparentes y el border puede tner color.

![Modelo de caja](img/modeloCaja.png)

### Ancho del Elemento Box Model

Debemos tener en cuenta las medidas del contenido + el padding + border + margin

### Outline

Este se encuentra entre el margin y el border,
le podemos dar color y estilo de border. Se puede sobreponer a otros elementos.

```css
outline: 10px outset #a8dadc;
```

### Outline-Offset

Este se inserta entre el border y el Outline, solo se le puede aplicar un solo valor. No se le puede aplicar color.

### **_PADDING_**

Se encuentra entre el border y el contenido.

![Padding](img/padding.png)

![PaddingReloj](img/paddingReloj.jpg)

### Box Sizing

CSS utiliza el box-content, pero no incluye el width ni el padding ni border.

> :bulb: **Tip:** Si no queremos pasarnos de la medida que le indicamos al width debemos utilizar `box-sizing: border-box`

> :bulb: Esta propiedad hace que cuando agregamos margin, padding o border a los elmntos no creesca mas del tamano que le dimos.

![Box-sizing](img/box-sizing.png)

### Propiedad Max-Width

Esta propidad la ocuparemos para que no aparesca la barra de escrol y para indicar hasta donde puede maximo ajustarse. Tambien lo podemos usa en el max-height.
se pueden usar en pixeles o en porsentaje.

`max-width: 100%;`

`max-width: 300px;`

`max-height:100px;`

### Propiedad Margin: Auto

Lo utilizaremos para centrar un elmento.
Con `margin: auto` va atomar automaticamente un por partes iguales el lado izquierdo como el lado derecho quedando asi centrado.

La propiedad de ` 0 auto;` el cero va atomar la parte superior (top) e infrior (bottom) y l auto el lado derecho (right) e izquierdo (left), siempre y cuando sean elementos inline.

`margin: 0 auto;`

![margin auto](img/marginAuto.png)

### Propiedad **_inherit_**

Donde colocamos el inhrit va heredar la propiedad del elemento padre, no olvidar colocar una clase. sin inherit se tomara su valor por default.

![inherit](img/inherit.png)

```css
div {
  padding: 10px 15px 5px 3px;
  border: 1px solid #457b9d;
  margin-left: 100px;
  background-color: #f1faee;
  max-width: 300px;
  box-sizing: border-box;
}

p.interno {
  margin-left: inherit;
}
```

### Concepto de margin collapse

Esto ocurre cuando tenemos dos cajas, y se aplica en los margenes inferior y superior.

El margen se junta con el margn del elemnto inferior, omando un solo margen para los dos,
si el margen del elemento supeior es mayor ese es el que se toma. **_Los margenes no se suman_**

![collapse](img/collapse.png)

## **_Manejo de colores_**

### Color por nombre HTML

[Pagina de Colores por nombre](https://htmlcolorcodes.com/color-names/)

### Manejo de colores **RGB**

![rgb](img/rgb.png)

El rgb tambien maneja el concepto de transparencia, se le conoce como alpha, es significa que se va intigrar con el color de fondo.

Si ponemos el valor de **1** no tenemos transparencia y si ponemos **0** tenemos la mayor transparencia, y para tener el 50% de transparencia usamos el **.5**

- r = Red `rgb(255,0,0)`
- g = Green `rgb(0,255,0)`
- b = Blue `rgb(0,0,255)`
- a = Alpha `rgb(255,0,0,.5)`

```css
.rgb {
  background-color: rgb(131, 56, 236);
}
.rgba {
  background-color: rgba(131, 56, 236, 0.5);
}
```

### Codigo de colores **Hexadecimal**

- Se compone de 6 digitos.
- Se inicia con #.
- Tambien podemos usar transparencia agregando 2 digitos mas
  - `#0090adff` no hay transparencia
  - `#0090ad00` maxima transparencia
  - `#0090ad88` 50% de transparencia
- El primer par corresponde al color rojo `#ff0000` seundo par es verde `#00ff00` y el tercer par es azul `#0000ff.
- Pa simplificar por pares podemos usar solo un numero o letra `#fa2` = `#ffaa22`

### Codigo de colores **HSL**

El hsl tambien maneja el concepto de transparencia, se le conoce como alpha, es significa que se va intigrar con el color de fondo.

Si ponemos el valor de **1** no tenemos transparencia y si ponemos **0** tenemos la mayor transparencia, y para tener el 50% de transparencia usamos el **.5**

- h = Hue `hsl(195, 100%, 50%)` el 195 se toma de una rueda de colores.
- s = Saturation `hsl(85, 100%, 50%)` es un porsentaje que va del 0% al 100%
- l = Lightnees `hsl(20, 50%, 100%)` la iluminacion es un porsentaje que va del 0% al 100%
- a = Alpha `hsl(195,100%,50%,.5)`

![Hue](img/hsl.png)
![hue](img/hue.jpg)

## **_Manejo de fondos_**

```css
body {
  background-color: dodgerblue;
  color: cornsilk;
  background-image: url("/img/fondo.png");
  background-repeat: no-repeat;
}
```

- Aplicar un `background-color: dodgerblue;` a toda nuestra pagina web.
- Aplicar imagen de fondo `background-image: url("/img/fondo.png");`
- Poner un color de fondo paraecido al de la imagen.
- Usaremos `background-repeat: no-repeat;` para que al hacer mas pequena la pagina el fondo no se repita.

De esta forma podemos simplificar

```css
body {
  color: cornsilk;

  background-attachment: fixed;
  background: dodgerblue url("/img/fondo.png") no-repeat right top;
}
```

## **Formato de texto**

1. color y fondo, se recomienda tener un contraste con la fuente.
   1. `color: #ef476f;`
   2. `background-color: #219ebc;`
2. Aliniar el texto.
   1. `text-align: center;`
3. Convertir todo a mayusculas.
   1. `text-transform: uppercase;`
4. Sombra al rededor de la fuente.
   1. `text-shadow: 2px 2px 2px #ced4da;`
5. Separar las letras
   1. `letter-spacing: 3px;`
6. Se parar las palabras.
   1. `word-spacing: 10px;`
7. Justificar texto.
   1. `text-align: justify;`
8. Direccion del texto.
   1. `direction: rtl;`
9. Se usa para elementos de texto pero mas para links
   1. `text-decoration: overline;` Linea encima del texto
   2. `text-decoration: line-through;` texto tachado
   3. `text-decoration: overline underline;`Texto envuelto entre dos lineas.
10. Indentacion
    1. `text-indent: 30px;`
11. Espacio entre lineas.
    1. `line-height: 1.5;`
12. `white-space: normal;` Para que el texto de un enter al final de lo que lo envuelve. `white-space: normal;` no envuelve el contenido en el div.

## **Fuentes**

Tipos de funtes mas representativas.amarillo

- Times New Roman (serif)
- Georgia (serif)
- Arial (sans-serif)
- Verdana (sans-serif)
- Courier New (monospace)
- Lucida Handwriting (cursive)

Para aplicar el tipo de funte utilizaremos `font-family:` nos despliega varias opciones, devido a que algunas no s pueden reconoser por l navegador, por si falla alguna pueda mostrar otra.

> :bulb: **Tip:** Si en el nombre de la funte tenemos espacios utilizaremos comillas.
> :bulb: **Tip:** La fuentes de tipo serif son las que tienen las puntas redondiadas.

```css
.fuente_times {
  font-family: "Times New Roman", Times, serif;
}
```

## **Estilos de funete**

`font-style:`

- italic
- normal
- oblique
- inherit
- initial
- unset

`font-weight:`

- Ancho de la funte
- 100 a 900
- bold (negritas)
- bolder (mas ancho)
- lighter (mas angosta)
- normal

`font-variant:`

- normal
- small-caps (La primera letra en mayuscula, mas alta)
- inherit
- initial
- unset

## Propiedad de Font-Size

`font-size:`

> :bulb: **Tip:** La usaremos para incrementar el tamano de la fuente.

- large
- larger (mas grande)
- medium
- small ( no es responciva)
- smaller (mas pequena)
- x-larger
- x-small
- xx-larger
- xx-small

Tambien podemos utilizar un valor

- pixeles (`16px`)
- 1em (es igual a 16px)
  > :bulb: **Tip:** No es soportardo en verciones anteriores de internet explorer.
- 3vw
  > :bulb: **Tip:** tomo en cuenta el alto y ancho de la pantalla w - weight (ancho) h - height (alto)  
  > :bulb: Es una fuente responciva  
  > :bulb: no esta soportado en todos los navegadores.

## Google Fonts

Aqui podremos encontrar muchas funtes de forma gratuita. [Google Fonts](https://fonts.google.com/)

> :bulb: **Tip:** Hay que considerar que puede tardar mas la pagina para cargarse, amenos que descarguemos la fuente y la incluyamos en la aplicacion web.

Hay dos formas de utilizar las fuentes de google.

- `<link>`
  - > :bulb: **Tip:** Esta va insertada en el documento html
- `@import`
  - > :bulb: **Tip:** Esta va insertada en el documento CSS, se pega en la parte de arriva si la etiqueta style

Para utilizarla en un titulo

usaremos `font-family:` y en la pagina de google copiaremos donde dice **CSS rules to specify families**

Si queremos importar varias fuentes de google solo copiamos otra fuente con `@import` y la pegamos abajo de la primera

> :bulb: **Tip:** Podemos reutilizar la misma linea de codigo para incluir mas fuenstes.

`@import url('https://fonts.googleapis.com/css2?family=Sofia&family=Roboto&display=swap');`  
se agrega && family mas el nombre de la fuente.

## Efectos con Google Fonts

Aqui la [guia](https://developers.google.com/fonts/docs/getting_started)

> :bulb: **Tip:** No lleva 2 en css

@import url('https://fonts.googleapis.com/**css**?family=Sofia|Roboto&effect=shadow-multiple&display=swap');

`https://fonts.googleapis.com/css?family=Rancho&effect=shadow-multiple|3d-float`

## **Atributo font**

Lo podemos hacer de una forma reducida o simplificada.

```css
.fuente_roboto{
    /*
    font-family: 'Roboto', sans-serif;
    font-style: normal;
    font-weight: normal;
    font-variant: small-caps;
    font-size: 20px;
    */
    /*font: font-style font-variant font-weight *font-size/line-heigth *font-family;*/
    font: italic small-caps bolder 20px Roboto, sans-serif;
```

## Menejo de Iconos

### Iconos Bootstrap

Pagina de iconos de [Bootstrap](https://icons.getbootstrap.com/)

### Pasos para usar los iconos en Bootstrap

1. Click en install
2. CDN Link publico. (lo podemos descargar **download** y lo podemos instalar en nuestro proyecto **npm**)
3. Hay 2 opciones
   1. Agregar un `<link>` va en el HTML
   2. Importarla `@import` Va en el CSS
4. Lo pegamos en el HTML
5. Despues elegimos un icono en la pagina y nos dara 3 opciones.
   1. Icon font (HTML)
   2. Code point
   3. Copy HTML (SVG)

Podemos modificar su tamano y color

## Iconos de Google

Pagina de [icons Google.](https://fonts.google.com/icons?selected=Material+Icons&icon.style=Outlined)

Para usarlos.

1. Click en [developer guide](https://developers.google.com/fonts/docs/material_icons)
2. La forma más sencilla de configurar las fuentes de íconos para usarlas en cualquier página web es mediante Google Fonts. Lo único que debes hacer es incluir una sola línea de HTML:

```css
<link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">
```

3. Lo pegamos en el HTML.
4. El nombre del icono se va especificar como el valor de este elemento.

```css
<p>
    <i class="material-icons">search</i>
       Búsqueda
</p>
```

`vertical-align: bottom;` Podemos aliniar el icono con el texto y el parrafo.

## Iconos de Ionicons

Pagina de [ionicons](https://ionic.io/ionicons)

Pasos para usarlos iconos

1. Click en [usage](https://ionic.io/ionicons/usage)
2. Colocar el link antes del `<body>` ya que es un archivo de javascript

```js
<script type="module" src="https://unpkg.com/ionicons@5.5.2/dist/ionicons/ionicons.esm.js"></script>
<script nomodule src="https://unpkg.com/ionicons@5.5.2/dist/ionicons/ionicons.js"></script>
```

3. Usaremos los iconos de esta forma.

```html
<p>
  <ion-icon name="checkmark-done-outline" class="icono_azul"></ion-icon>
  Listo
</p>
```

> :bulb: **Tip:** Por cada link que agreguemos la pagina web se va a demorar mas en cargar.

## **Propiedad Display**

### Display Block

Nos va permitir mostrar o uccultar elementos o tambien modificar la forma en que se muestran algunos elementos HTML

Etiquetas con propiedad display block, van ocupar una nueva linea por completo

```html
<h1>Título</h1>
<div>Div</div>
<p>Párrafo</p>
```

```html
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>
```

![block](img/block.png)

### Display inline

`<span>`  
`<a href="#">Link 1</a>`

Para modificar los elementos de block y se muestren en una sola linea usaremos.

`display: inline;`

![inline](img/inline.png)

### Display None

Con `display: none;`podemos ucultar ese elemento, ya no ocupa el espacio a diferencia de `visibility: hidden;` que mantiene el espacio.

## **Posicionamiento de Elementos**

### Centrar Div

1. Asignar un tamano `width: 50%;`
   1. cuando usamos porcentajes este cambia conforme cambia el tamano de la ventana.
   2. tambien podemos usar `max-width: 50%;`
2. Border `border: 3px solid firebrick;`
3. margin `margin: auto;`
   1. con auto el espacio del lado derecho e izquierdo se vuelve el mismo, y se **centra**.

### Posicionamiento Estatico

### Tipos de posicionamiento

🔴 static  
🔴 relative  
🔴 fixed  
🔴 absolute  
🔴 sticky

> :bulb: **Tip:** Cuando usamos static no podremos utilizr top: left: ...

### Posicionamiento Relativa

Con esta posicion si va a fectar el top: left: botton: right:

`position: relative;`

> :bulb: **Tip:** Si tenemos otros elementos, no afectaran al div, siempre seguira reservando su espacio.

### Posicionamiento Fixed (ajustado)

Es util para menus de navegacion o botones de chat. ya que siempre se va amantener fijo. Se ajusta al <span style="color:red"> **VIEWPORT**</span>

`position: fixed;`

> :bulb: **Tip:** No se reserva su espacio

### Posicionamiento Absoluta

Normalmente la utilizaremos dentro de otro elemnto **DIV**

> :bulb: **Tip:** Si no esta dentro de un DIV este tomara el body.  
> :bulb: El div padre no debe ser de tipo estatic

`position: absolute;`

![positionabsoluta](img/positionabsoluta.png)

### Posicionamiento Sticky (pegajoso)

> :bulb: **Tip:** Para que funcione tenemos que usar top, right , bottom o left

> :bulb: **Tip:** Funsiona de manera relativa hasta el momento que sale de pantalla, entonces se vuelve como un fixed

> :bulb: **Tip:** Consideraciones Si estamos trabajando con safari usaremos una coreccion. `position: -wekit-sticky;` y no funciona en internet explorer.

### Posicionamiento Z-index

Nos sirve para poder mostar elementos por detras o ensima de otros.

`z-index: -1;` se mostrara atras de el primer elemento.  
`z-index: 1;` se mostrara por encima de el primer elemento.

### Propiedad Overflow

Es cuando el texto se sale de nuestro contenedor.

`overflow:visible;` muestra todo lo que sale del elemento. Es la propiedad por default

`overflow: hidden;` Todo lo que se sale se va ocultar.

`overflow: scroll;` Se va amostrar dos barras con scroll para poder ver todo el contenido

`overflow: auto;` Solo va a mostras las varras de scroll necesarias.

> :bulb: **Tip:** Esta propiedad solo se va poder travajar si especificamos un alto (height), ya que al quitar el height se deslplagara todo el contenido en el elemento div

> :bulb: **Tip:** Lo podemos configurar para el ejex o eje y con `overflow-x: o overflow-y:` y podemos usarlo con las propiedades anteriores.

### Propiedad Float

Con esta propiedad podemos colocar mas elementos en la misma linea. Cuado ya no caben se pasan ala siguiente linea

`float: left;` `float: right;`

> :bulb: **Tip:** Para poder a gregar mas elentos en otra linea, cortando la propiedad de float usaremos `clear: both;` para limpiar los dos lados o left, right para elegir que lado limpiar

### Propiedad Display Inline-Block

Con esta propiedad `display: inline-block;` podemos controlar el alto (height y padding) de los elementos incluso si son de tipo inline. Con esto va adquirir las dos caracteristicas, inline y block y asi poder aplicar las propiedades

### **Menu** con la propiedad Display Inline-Block

Con esta propiedad podemos usar una lista como un meno sin necesidad de flotar los elementos.

## **Selectores**

### Selectores Combinados

#### Selectores Decendientes

> :bulb: **Tip:** Una ves que selecciones un elemento se va aplicar el estilo que hemos configurado para todos los elementos decendientes sin importar si son elementos directos e indirectos. Aun que esten dentro de otra equiqueta s les va aplicar las propiedades que asignemos.

```css
div.contenedor.descendiente p {
  background-color: #fdffb6;
}
```

> :bulb: **Tip:** Solo necesitamos ponr la clase un espacio y las etiquetas que queremos afeactar.

#### Selector Child

> :bulb: **Tip:** Para afectar solo a los hijos de un div utilizarmos div.la clase espacio > p. para dejar fuera a otros parrafos que esten dentro de otra etiqueta que asu ves estan dentro del div.

```css
div.contenedor.hijo > p {
  background-color: #ffc6ff;
}
```

#### Selector Sibling (Adyacente)

> :bulb: **Tip:** Se usa el signo +, va afectar al parrafo que se encuentre ensegida del div con la clase que seleccionamos, pero solo va a fectar a ese parrafo.

```css
div.contenedor.adyacente + p {
  background-color: #caffbf;
}
```

> :bulb: **Tip:** selector hermano, se leciona al que esta almismo nivel

```css
div.contenedor.hermano ~ p {
  background-color: #9bf6ff;
}
```

### Pseudo Clases

<details>
<summary> Que es la PseudoClase?</summary>
Esuna palabra clave que se anade alos selectores y que especifica un estado especial del elemento seleccionado.
</details>

> :bulb: **Tip:** Las pseudo clases nos van a permitir manipular ciertos estado de nuestro de nuestros elementos HTML

Podemos cambiar el color de fondo al pasar el mause un div. Esto con <span style="color:red"> **:hover**</span>

```css
div.contenedor:hover {
  background-color: #457b9d;
  color: #f1faee;
}
```

Podemos ocultar y mostrar al pasar el mause un parrafo. Esto con <span style="color:red"> **:hover**</span>

```css
div.contenedor.oculto p{
    display: none;
}
div.contenedor.oculto:hover p{
    display: block;
    background-color: #a8dadc;
    color: #023e8a;
    padding: 15px;
```

> :bulb: **Tip:** Otra pseudo clase es `first-child`

```css
div.contenedor.primero p:first-child {
  font-variant: small-caps;
}
```

## Pseudo Elementos

<details>
<summary> Que es un PseudoElemento</summary>
Se anaden a los selectores, pero no describen un estado especial sino que, permiten <span style="color:red"> **anadir estilos a una parte concreta del documento.**</span>
</details>

Funciona cuando seleccionamos el texto con el mause

```css
div.contenedor p::selection {
  color: red;
  background-color: yellow;
}
```

Funciona cuando seleccionamos el texto con el mause, pero solo en la primera linea del parrafo, funciona de forma dinamica, si hacemos zoom solo aplicara para la primera linea.

```css
div.contenedor p::first-line {
  font-variant: small-caps;
  color: red;
}
```

Funciona para cambiar la primera letra de cada parrafo que este dentro del div

```css
div.contenedor p::first-letter {
  font-size: 1.5em;
}
```

Funciona para agregar palabras o signos al principio o al final del parrafo.

```css
div.contenedor p::before {
  content: "- ";
}

div.contenedor p::after {
  content: " -";
}
```

## Transparencia

### Transparencia en imagenes 

> :bulb: **Tip:** Lo podemos usar para una galeria de imagenes

``` css
img{
    opacity: 0.5;
}
img:hover{
    opacity: 1.0;
}
```

## **Gradientes**


