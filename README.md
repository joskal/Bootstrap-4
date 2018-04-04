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

## Columnas automáticas
La clase **.col-auto** nos permite establecer un ancho automático segun el contenido de la columna. Hay una clase auto para cada layout: **.col .col-sm-auto .col-md-auto .col-lg-auto .col-xl-auto**

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

## Alineación horizontal de columnas
Las clases que se encargan de este tipo de alineación son las siguientes:
```html
  .justify-content-start
  .justify-content-center
  .justify-content-end
  .justify-content-around
  .justify-content-between
```
