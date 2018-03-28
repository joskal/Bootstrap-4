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
<td>&le;543px</td>
</tr>
<tr>
<td>col-sm</td><td>Small - Smartphones vertical</td>
<td>&ge;544px &le;767px</td>
</tr>
<tr>
<td>.col-md</td><td>Medium - Tablets</td>
<td>&ge;768px &le;991px</td>
</tr>
<tr>
<td>.col-lg</td><td>Large - Desktops</td>
<td>&ge;992px &le;1199px</td>
</tr>
<tr>
<td>.col-xl</td><td>Extra Large - Desktops</td>
<td>&ge;1200px</td>
</tr>
</table>

## Container
El **container** es el contenedor principal, donde se alojarán todas las filas y columnas. Con el container también podemos centrar la página.

Las filas **row** son grupos horizontales de columnas.
