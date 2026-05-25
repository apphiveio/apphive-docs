---
description: Modify control (controls)
---

# Modify control

Modify control es una de las funciones más utilizadas al momento de desarrollar tu aplicación en Apphive. Esta te permite modificar los controles dentro de ella, aportando vida y dinamismo a tu aplicación en el momento en que tus usuarios interactúan con ella. Te permite modificar distintas propiedades dependiendo del control que utilices, como texto, fondos, fuentes, colores, y tamaños.. Tiene 3 Entry vars : “Data to send” , “Element” , “Property to modify” y no cuenta con callbacks.

<figure><img src="../../../gitbook/assets/image (696).png" alt=""><figcaption></figcaption></figure>

=== "Entry Vars"

    **Data to send :** Colocaremos el valor que queramos modificar, como un string en caso de ser un texto, un hexadecimal en caso de querer cambiar el color de un texto o fondo de un botón, hasta números para modificar un tamaño. Debes asegurarte que el valor que envíes sea permitido por el parámetro a modificar. **(Required)**

    **Element :** Ingresamos el ID del control que deseas modificar o principalmente seleccionarlo desde el menú de variables en la sección controls, donde encontrarás tus controles que tienes en tu página permitiéndote seleccionar el que deseas modificar. **(Required)**

    **Property to modify :** Encontraremos tanto en un dropdown con las propiedades disponibles para modificar una vez que seleccionemos el control desde el menú de variable o en un field donde podrás colocar la propiedad deseada a modificar en caso de no encontrarla dentro de las opciones del dropdown anterior o ingreses el id del control directamente.. **(Required)**

=== "Callbacks & OutVars"

    **(No contiene  callbacks)**

    OutVars

    ```
    Null
    ```

