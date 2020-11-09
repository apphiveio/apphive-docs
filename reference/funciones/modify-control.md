---
description: >-
  Con esta función podemos modificar de forma dinámica las propiedades de los
  controles para dar apariencia de forma dinámica las aplicaciones editadas
---

# Modify Control

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
| item |  |  |
| name |  |  |
| value |  |  |
{% endtab %}

{% tab title="Radio" %}

{% endtab %}

{% tab title="Slider" %}

{% endtab %}
{% endtabs %}

### Media

{% tabs %}
{% tab title="Image" %}

{% endtab %}

{% tab title="Camera view" %}

{% endtab %}

{% tab title="Map" %}

{% endtab %}

{% tab title="Web view" %}

{% endtab %}

{% tab title="Calendar" %}

{% endtab %}

{% tab title="Icon" %}

{% endtab %}

{% tab title="Video view" %}

{% endtab %}

{% tab title="Graphic view" %}

{% endtab %}
{% endtabs %}

