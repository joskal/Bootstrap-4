# Bootstrap-4
## Responsive meta tag
BS est&aacute; desarrollado como **mobile first**, lo que significa que el c&oacute;digo est&aacute; optimizado primeramente para dispositivos m&oacute;viles, escalando gradualmente la resoluci&oacute;n del resto de dispositivos como tablets, laptops y PC's de escritorio.

Debe ser alojado en el \<head>
```html
<meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
```

## layout

<table>
<tr>
<td>.col</td><td>Extra small - Smartphones vertical</td>
<td>&lt;576px</td>
</tr>
<tr>
<td>.col-sm</td><td>Small - Smartphones vertical</td>
<td>min-width: 576px;</td>
</tr>
<tr>
<td>.col-md</td><td>Medium - Tablets</td>
<td>min-width: 768px;</td>
</tr>
<tr>
<td>.col-lg</td><td>Large - Desktops</td>
<td>min-width: 992px;</td>
</tr>
<tr>
<td>.col-xl</td><td>Extra Large - Desktops</td>
<td>min-width: 1200px;</td>
</tr>
</table>

[responsive breakpoints](https://getbootstrap.com/docs/4.0/layout/overview/#responsive-breakpoints)

## Container
La clase **container** es el contenedor principal, donde se alojarán todas las filas y columnas. La clase **container-fluid** ocupa el ancho de la pantalla. Con el container también podemos centrar la página. 

Las filas **row** son grupos horizontales de columnas.
```html
<div class="container">
  <div class="row">
    <div class="col">
      <h2>columna 1</h2>
    </div>
    <div class="col">
      <h2>columna 2</h2>
    </div>
    <div class="col">
      <h2>columna 3</h2>
    </div>
  </div>
</div>
```
[containers](https://getbootstrap.com/docs/4.0/layout/overview/#containers)

## Columnas automáticas
La clase **.col-auto** nos permite establecer un ancho automático segun el contenido de la columna. Hay una clase auto para cada layout: **.col .col-sm-auto .col-md-auto .col-lg-auto .col-xl-auto**

[Variable width content](https://getbootstrap.com/docs/4.0/layout/grid/#variable-width-content)

## Sizing

La clase **w-n** establece un porcentaje de ancho de fila para una columna en concreto. Las clases son: **.w-25 .w-50 .w75 .w-100**

La clase **w-100** actúa también como separador.
```html
<div class="row">
  <div class="col">
    <h2>columna 1</h2>
    <p>Lorem ipsum dolor</p>
  </div>
  <div class="col">
    <h2>columna 2</h2>
    <p>Lorem ipsum dolor</p>
  </div>
  <div class="w-50">
    <h2>columna 3</h2>
    <p>Esta columna ocupa el 50% del ancho de la fila</p>
  </div>
</div>
```
[sizing](https://getbootstrap.com/docs/4.0/utilities/sizing/)

## No-gutters
```html
.no-gutters
```
Esta clase se encarga de eliminar tanto los margins como los paddings laterales de un contenedor.
```html
<div class="row no-gutters">....</div>
```
[No-gutters](https://getbootstrap.com/docs/4.0/layout/grid/#no-gutters)

## Alineación horizontal de columnas
Las clases que se encargan de este tipo de alineación son las siguientes:
```html
  .justify-content-start
  .justify-content-center
  .justify-content-end
  .justify-content-around
  .justify-content-between
```
```html
<div class="row justify-content-start">
  <div class="col-4"> <h2>col #1</h2>justify-content-start </div>
  <div class="col-4"> <h2>col #2</h2> </div>
</div>
<div class="row justify-content-center">
  <div class="col-4"> <h2>col #1</h2>justify-content-center </div>
  <div class="col-4"> <h2>col #2</h2> </div>
</div>
<div class="row justify-content-end">
  <div class="col-4"> <h2>col #1</h2> justify-content-end</div>
  <div class="col-4"> <h2>col #2</h2> </div>
</div>
<div class="row justify-content-around">
  <div class="col-4"> <h2>col #1</h2>justify-content-around </div>
  <div class="col-4"> <h2>col #2</h2> </div>
</div>
<div class="row justify-content-between">
  <div class="col-4"> <h2>col #1</h2>justify-content-between </div>
  <div class="col-4"> <h2>col #2</h2> </div>
</div>
```
[Horizontal alignment](https://getbootstrap.com/docs/4.0/layout/grid/#horizontal-alignment)

## Alineación vertical de columnas
clases:
```html
.align-self-start
.align-self-center
.align-self-end
```
```html
<div class="container">
  <div class="row">
    <div class="col align-self-start">
      One of three columns
    </div>
    <div class="col align-self-center">
      One of three columns
    </div>
    <div class="col align-self-end">
      One of three columns
    </div>
  </div>
</div>
```
[Vertical alignment](https://getbootstrap.com/docs/4.0/layout/grid/#vertical-alignment)

## Offsetting
Consiste en incrementar el margen izquierdo de la columna intercalando columnas vacias.
```html
.offset-1    - .offset-12
.offset-sm-0 - .offset-sm-12
.offset-md-0 - .offset-md-12
.offset-lg-0 - .offset-lg-12
.offset-xl-0 - .offset-xl-12
```
```html
<div class="row">
  <div class="col-2"> <h3>col #1</h3>col-2 </div>
  <div class="col-2 offset-8"><h3>col #2</h3>col-2 offset-8</div>
</div>
<div class="row">
  <div class="col-2 offset-1"> <h3>col #1</h3>col-2 offset-1 </div>
  <div class="col-2 offset-6"><h3>col #2</h3>col-2 offset-6</div>
</div>
```
[offsetting columns](https://getbootstrap.com/docs/4.0/layout/grid/#offsetting-columns)

## Ordenamiento de columnas
La clase .order-* nos permite cambiar el orden de las columnas con facilidad.
```html
.order-0    - .order-12
.order-sm-0 - .order-sm-12
.order-md-0 - .order-md-12
.order-lg-0 - .order-lg-12
.order-xl-0 - .order-xl-12
```
```html
<div class="row">
  <div class="col order-4"><h4>col #1</h4></div>
  <div class="col order-3"><h4>col #2</h4></div>
  <div class="col order-2"><h4>col #3</h4></div>
  <div class="col order-1"><h4>col #4</h4></div>
</div>
```
[Order classes](https://getbootstrap.com/docs/4.0/layout/grid/#order-classes)

## Nesting
Las columnas se pueden anidar entre sí.
```html
<div class="row">
  <div class="col">
    <h3>columna #1</h3>
    <div class="row">
      <div class="col">subcolumna #1</div>
      <div class="col">subcolumna #2</div>
    </div>
  </div>
  <div class="col">
    <h3>columna #2</h3>
    <div class="row">
      <div class="col">subcolumna #1</div>
      <div class="col">subcolumna #2</div>
      <div class="col">subcolumna #3</div>
    </div>
  </div>
</div>
```
[nesting](https://getbootstrap.com/docs/4.0/layout/grid/#nesting)

## Display
Podemos mostrar u ocultar el contenido de las columnas.
```html
d-{value} for xs
d-{layout}{value}
```
{layout} puede ser:
* sm 
* md 
* lg 
* xl


{value} puede ser:
* none
* inline
* inline-block
* block
* table
* table-cell
* table-row
* flex
* inline-flex

```html
<div class="row">
  <div class="col d-block d-sm-none">XS - Extra Small</div>
  <div class="col d-none d-sm-block d-md-none">SM - Small</div>
  <div class="col d-none d-md-block d-lg-none">MD - Medium</div>
  <div class="col d-none d-lg-block d-xl-none">LG - Large</div>
  <div class="col d-none d-xl-block">XL - Extra Large</div>
</div>
```
[Display](https://getbootstrap.com/docs/4.0/utilities/display/)

## Spacing
BS4 dispone de márgenes y paddings adaptables con los que cambiar la apariencia de cualquier elemento. Disponemos de dos prefijos para manejarlos:
* **m** - margin
* **p** - padding

Con estos prefijos se construyen las clases siguientes:
<table>
  <tr>
    <th>margin</th><th>padding</th><th>Side</th>
  </tr>
  <tr>
    <td>mt-0<br>mt-1<br>mt-2<br>mt-3<br>mt-4<br>mt-5<br>mt-auto</td>
    <td>pt-0<br>pt-1<br>pt-2<br>pt-3<br>pt-4<br>pt-5</td>
    <td>top</td>
  </tr>
  <tr>
    <td>mb-0<br>mb-1<br>mb-2<br>mb-3<br>mb-4<br>mb-5<br>mb-auto</td>
    <td>pb-0<br>pb-1<br>pb-2<br>pb-3<br>pb-4<br>pb-5</td>
    <td>bottom</td>
  </tr>
  <tr>
    <td>ml-0<br>ml-1<br>ml-2<br>ml-3<br>ml-4<br>ml-5<br>ml-auto</td>
    <td>pl-0<br>pl-1<br>pl-2<br>pl-3<br>pl-4<br>pl-5</td>
    <td>left</td>
  </tr>
  <tr>
    <td>mr-0<br>mr-1<br>mr-2<br>mr-3<br>mr-4<br>mr-5<br>mr-auto</td>
    <td>pr-0<br>pr-1<br>pr-2<br>pr-3<br>pr-4<br>pr-5</td>
    <td>right</td>
  </tr>
  <tr>
    <td>mx-0<br/>mx-1<br/>mx-2<br/>mx-3<br/>mx-4<br/>mx-5<br/>mx-auto</td>
    <td>px-0<br/>px-1<br/>px-2<br/>px-3<br/>px-4<br/>px-5</td>
    <td>left & right</td>
  </tr>
  <tr>
    <td>my-0<br/>my-1<br/>my-2<br/>my-3<br/>my-4<br/>my-5<br/>my-auto</td>
    <td>py-0<br/>py-1<br/>py-2<br/>py-3<br/>py-4<br/>py-5</td>
    <td>top & bottom</td>
  </tr>

</table>
  

[Spacing](https://getbootstrap.com/docs/4.0/utilities/spacing/#how-it-works)

## Tipografía

Contamos con una serie de clases para alinear el texto.
```html
.text-left
.text-center
.text-right
```
Asimismo también contamos con clases responsive para alinear según el ancho de la pantalla.
```html
<div class="col-12 col-md-8">
  <p class="text-left text-sm-right">Texto alineado a la derecha en small device</p>
  <p class="text-left text-md-right">Texto alineado a la derecha en medium device</p>
  <p class="text-left text-lg-right">Texto alineado a la derecha en large device</p>
  <p class="text-left text-xl-right">Texto alineado a la derecha en extra large device</p>
</div>
```
Clases para cambiar mayusculas y minusculas.
```html
.text-uppercase
.text-lowercase
.text-capitalize
```
Agregar citas blockquote
```html
<blockquote class="blockquote">
  <p class="mb-0">Habla despacio, habla bajito y no hables demasiado</p>
  <footer class="blockquote-footer">John Wayne <cite title="Source Title">actor de cine</cite></footer>
</blockquote>
```
[Typography](https://getbootstrap.com/docs/4.0/content/typography/)

## Imágenes
```html
<div class="row no-gutters">
  <div class="col">
    <img class="img-fluid rounded-circle float-left" src="http://lorempixel.com/200/200/sports" alt="" />
    <img class="img-fluid float-right" src="http://lorempixel.com/200/200/animals" alt="" />
  </div><!-- /.col -->
</div><!-- /.row -->
<div class="row no-gutters">
  <div class="col">
    <figure class="figure">
      <img class="img-fluid rounded" src="http://lorempixel.com/400/400/animals" alt="" />
      <figcaption class="figure-caption"> 
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Necessitatibus, sit?</p>
      </figcaption>
    </figure>
  </div><!-- /.col -->
</div><!-- /.row -->

```
[Images](https://getbootstrap.com/docs/4.0/content/images/)
