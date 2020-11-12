---
description: >-
  Con esta función podemos modificar de forma dinámica las propiedades de los
  controles para dar apariencia de forma dinámica las aplicaciones editadas
---

# Modify Control

Consta de 3 elementos 

1. Data to send
2. Element
3. Property to modify

![](../../../.gitbook/assets/image%20%28311%29.png)

## Data to send

Se refiere a la información con el que un control o campo  va a modificar algunas de sus propiedades.

## Element

Sirve para elegir algún control o campo para ser modificado

## Property to modify

Este apartado permite saber que propiedades están disponibles dependiendo del tipo de elemento que se eligió previamente

## Propiedades de los controles

### Containers

{% tabs %}
{% tab title="Container" %}
| Propiedad | Descripción | Tipo de valores que acepta la propiedad |
| :--- | :--- | :--- |
| backgroundImage | Permite cambiar el fondo del contenedor sustituyéndolo por una imagen | Direcciones de imágenes del dispositivo, internet o firebase |
| style,height.value | Permite cambiar la altura del contenedor en pixeles | Números enteros |
| isHidden | Permite mostrar u ocultar el contenedor | true o false |
| scrollToCategory |  |  |
| style.alignItems | Permite alinear los controles dentro del contenedor |  flex-start o flex-end |
| style.background | Permite cambiar el color de fondo del contenedor por un color solido | Un valor de un color, generalmente de la paleta de colores |
| style.borderColor | Permite agregar un color solido a los bordes del contenedor | Un valor de un color, generalmente de la paleta de colores |
| style.width.value | Permite cambiar el ancho del contenedor en porcentaje | Números enteros o con decimales |
{% endtab %}

{% tab title="Swiper" %}
| Propiedad | Descripción | Tipo de valores que acepta la propiedad |
| :--- | :--- | :--- |
| currentIndex | Permite seleccionar la posición de una vista en especifico en el swiper | Números enteros correspondientes al numero de vistas |
| style.alignItems | Permite alinear los controles dentro del swiper | flex-start o flex-end |
| style.background | Permite cambiar el color de fondo del swiper por un color solido | Un valor de un color, generalmente de la paleta de colores |
{% endtab %}
{% endtabs %}

### Form elements

{% tabs %}
{% tab title="Field" %}
<table>
  <thead>
    <tr>
      <th style="text-align:left">Propiedad</th>
      <th style="text-align:left">Descripci&#xF3;n</th>
      <th style="text-align:left">Tipo de valores que acepta la propiedad</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">disabled</td>
      <td style="text-align:left">Permite habilitar o deshabilitar la edici&#xF3;n del texto dentro del
        field</td>
      <td style="text-align:left">true o false</td>
    </tr>
    <tr>
      <td style="text-align:left">focus</td>
      <td style="text-align:left">Permite enfocar el field para tenerlo listo para comenzar a ingresar texto</td>
      <td
      style="text-align:left">true</td>
    </tr>
    <tr>
      <td style="text-align:left">secure-text-entry</td>
      <td style="text-align:left">Mostrar o no el texto en modo seguro</td>
      <td style="text-align:left">true o flase</td>
    </tr>
    <tr>
      <td style="text-align:left">value</td>
      <td style="text-align:left">Permite cambiar el valor del texto</td>
      <td style="text-align:left">
        <ol>
          <li>texto</li>
          <li>n&#xFA;meros</li>
          <li>objetos</li>
          <li>arreglos</li>
        </ol>
      </td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="Text" %}
<table>
  <thead>
    <tr>
      <th style="text-align:left">Propiedad</th>
      <th style="text-align:left">Descripci&#xF3;n</th>
      <th style="text-align:left">Tipo de valores que acepta la propiedad</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">style.background</td>
      <td style="text-align:left">Permite cambiar el color de fondo del texto por un color solido</td>
      <td
      style="text-align:left">Un valor de un color, generalmente de la paleta de colores</td>
    </tr>
    <tr>
      <td style="text-align:left">style.color</td>
      <td style="text-align:left">Permite cambiar el color del texto</td>
      <td style="text-align:left">Un valor de un color, generalmente de la paleta de colores</td>
    </tr>
    <tr>
      <td style="text-align:left">text</td>
      <td style="text-align:left">Permite cambiar el valor del texto</td>
      <td style="text-align:left">
        <p></p>
        <ol>
          <li>texto</li>
          <li>n&#xFA;meros</li>
          <li>objetos</li>
          <li>arreglos</li>
        </ol>
      </td>
    </tr>
  </tbody>
</table>
{% endtab %}

{% tab title="Button" %}
| Propiedad | Descripción | Tipo de valores que acepta la propiedad |
| :--- | :--- | :--- |
| label | Permite cambiar el texto del botón | Texto |
| name | Permite cambiar el nombre del botón | Texto |
| style.background | Permite cambiar el color de fondo del botón por un color solido | Un valor de un color, generalmente de la paleta de colores |
{% endtab %}

{% tab title="Switch" %}
| Propiedad | Descripción | Tipo de valores que acepta la propiedad |
| :--- | :--- | :--- |
| name | Permite cambiar el nombre del switch  check | texto |
| value | Permite cambiar el valor del switch o check | true o false |
{% endtab %}

{% tab title="Picker" %}
| Propiedad | Descripción | Tipo de valores que acepta la propiedad |
| :--- | :--- | :--- |
| item | Permite cambiar lo indicadores que se muestran en una lista desplegable | texto |
| name | Permite cambiar el nombre del botón | texto |
| value | Perite cambiar el valor de los items | texto |
{% endtab %}

{% tab title="Radio" %}
| Propiedad | Descripción | Tipo de valores que acepta la propiedad |
| :--- | :--- | :--- |
| items | Permite cambiar lo indicadores que se muestran en una lista | texto |
{% endtab %}

{% tab title="Slider" %}
| Propiedad | Descripción | Tipo de valores que acepta la propiedad |
| :--- | :--- | :--- |
| value | Permite cambiar el valor del indicador | Números enteros |

{% hint style="info" %}
La propiedad **value** no se encuentra ****como propiedad en el picker pero se puede escribir 
{% endhint %}
{% endtab %}
{% endtabs %}

### Media

{% tabs %}
{% tab title="Image" %}
| Propiedad | Descripción | Tipo de valores que acepta la propiedad |
| :--- | :--- | :--- |
| src | Permite cambiar el fondo por una imagen | Direcciones de imágenes del dispositivo, internet o firebase |
{% endtab %}

{% tab title="Camera view" %}
| Propiedad | Descripción | Tipo de valores que acepta la propiedad |
| :--- | :--- | :--- |
| takePhoto |  |  |
{% endtab %}

{% tab title="Map" %}
| Propiedad | Descripción | Tipo de valores que acepta la propiedad |
| :--- | :--- | :--- |
| linearRoutes | Muestra una linea recta entre puntos | Un objeto de la base de datos o un arreglo |
| markers | Indica los puntos guardados en un grupo de Geo Fire, debe especificarse que tipo de información es la que se va a mostrar | El objeto que retorna la función Query Fire Geolocation |
| nearLocation |  |  |
| Region | Modifica y muestra el punto de localización en el mapa | Un objeto con los valores latitude y longitude, con sus respectivas coordenadas |
| Region\|Latitude | Modifica la latitud del mapa | Números enteros con  siete cifras después del punto |
| Region\|Longitude | Modifica la longitud del mapa | Números enteros con siete cifras después del punto |
| routes | Muestra la ruta optima desde un punto A a un punto B | Números enteros con siete cifras después del punto |
| Show user location |  |  |
| zoom | Acerca o aleja la vista del mapa entre menor sea el digito, el zoom será más alto | Números enteros o enteros con decimales o milésimas |

{% hint style="info" %}
**routes:** para marcar la tura se necesitan 4 modify control cada una especificando la latitud y longitud del destino

NOMBRE\_QUE\_DE\_DES\_A\_LA\_RUTA.origin.latitude NOMBRE\_QUE\_DE\_DES\_A\_LA\_RUTA.origin.longitude NOMBRE\_QUE\_DE\_DES\_A\_LA\_RUTA.destination.latitude NOMBRE\_QUE\_DE\_DES\_A\_LA\_RUTA.destination.longitude Donde dice NOMBRE\_QUE\_DE\_DES\_A\_LA\_RUTA lo remplazas por el nombre que le quieras dar

[ver más](https://comunidad.apphive.io/t/como-marcar-la-ruta-en-un-mapa/2641)
{% endhint %}
{% endtab %}

{% tab title="Web view" %}
| Propiedad | Descripción | Tipo de valores que acepta la propiedad |
| :--- | :--- | :--- |
| href | Indica la dirección web que se mostrará en el componente | Direcciones web |
{% endtab %}

{% tab title="Calendar" %}
| Propiedad | Descripción | Tipo de valores que acepta la propiedad |
| :--- | :--- | :--- |
|  |  |  |
{% endtab %}

{% tab title="Icon" %}
| Propiedad | Descripción | Tipo de valores que acepta la propiedad |
| :--- | :--- | :--- |
| badgeText | Cambia el valor mostrado en el badge | Números y texto |
| src.name | Cambia el nombre del icono | texto |
| style.color | Cambia el color del icono | Un valor de un color, generalmente de la paleta de colores |
{% endtab %}

{% tab title="Video view" %}
| Propiedad | Descripción | Tipo de valores que acepta la propiedad |
| :--- | :--- | :--- |
| video.Config.url | Muestra el video de YouTube o Vimeo | Direcciones web de Youtue o Vimeo |
{% endtab %}

{% tab title="Graphic view" %}
| Propiedad | Descripción | Tipo de valores que acepta la propiedad |
| :--- | :--- | :--- |
| data | Es el conjunto de información numérica estática a graficar | texto |
| labels | Es el conjunto de información en texto estático  que se mostrará en las etiquetas | texto |
| PropLabel | Es el conjunto de información numérica dinámica a graficar | Objeto de la base de datos |
| ropValue | Es el conjunto de información en texto dinámico  que se mostrará en las etiquetas | Objeto de la base de datos |
{% endtab %}
{% endtabs %}

{% hint style="info" %}
No cuenta con callbacks
{% endhint %}

Información general

