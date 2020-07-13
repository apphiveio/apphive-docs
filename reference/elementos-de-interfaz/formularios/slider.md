---
description: A component used to select a single value from a range of values.
---

# Slider

![](../../../.gitbook/assets/captura-de-pantalla-2020-02-07-a-la-s-9.34.30.png)



### 🎨 Styles

* **Appearance**

  * **Thumb color**: select the color in the slider control using the [color picker](../../estilos/color-picker.md). 
  * **Thumb border color**: select the color in the slider control border using the [color picker](../../estilos/color-picker.md).  
  * **Selection color**: select the color in the slider value using the [color picker](../../estilos/color-picker.md).   
  * **Blank color**: select the color in the slider left value using the [color picker](../../estilos/color-picker.md).

* **Dimensions**
  * **Width:** set how wide the slider element is using.
  * **Height:** set how tall the slider element is using.

### ⚙ Properties

* **Generic properties**
  * **Control name:** you can add a name to the slider element this could be the way to identify this element about another elements.
  * **Enable** [**skeleton loaders**](../../estilos/skeleton-loader.md)**:** this tool provides an indication to the user that something is coming but not yet available on the slider element.
  * **Control is hidden:** hide the slider element from the screen.

{% hint style="info" %}
The [**skeleton loader**](../../estilos/skeleton-loader.md) component provides a user with a visual indicator that content is coming/loading. This is better received than traditional full-screen loaders.
{% endhint %}

* **Specific Properties**
  * **Slider minimum value**: initial minimum value of the slider. Default value is 0.
  * **Slider maximum value**: Initial maximum value of the slider. Default value is 5.
  * **Slider step**: Step value of the slider. The value should be between 0 and maximum value. Default step value is 1.

### 👆 Events

* **On charge:** the on charge ****event detects when the value of a slider element changes. 

