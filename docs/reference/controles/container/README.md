---
description: >-
  Un container es un delimitador abstracto, es decir, un objeto que contiene
  otros objetos que pueden ser incluidos o eliminados
---

# Container

![](../../../gitbook/assets/image%20%28140%29.png)



=== "Style"

    ## Appeareance

    ### Backgorund color

    Rellena el cuerpo del contenedor de un color solido [ver más](https://docs.apphive.io/global-functions/estilos/background-color)

    ### Background image

    Rellena el cuerpo del contenedor con una imagen seleccionada [ver más](https://docs.apphive.io/global-functions/estilos/background-image)

    ## Borders

    ### Border Width

    Asigna el color, ancho y tipo de borde del componente [ver más](https://docs.apphive.io/global-functions/estilos/border-width)

    ### Border Radius

    Redondea las esquinas del componente [ver más](https://docs.apphive.io/global-functions/estilos/border-radius)

    ## Dimentions

    Cambia el tamaño en pixeles del componentes, así mismo los puede cambiar en porcentaje, este porcentaje de dimensiones es directamente proporcional a las dimensiones del dispositivo [ver más](https://docs.apphive.io/global-functions/estilos/dimentions)

    ## Layout

    ### Direction

    Indica la dirección de los componentes hijos dentro de un contenedor [ver más](https://docs.apphive.io/global-functions/estilos/direction)

    ### Scroll

    Con este elemento podemos cambiar la dirección de scroll de los componentes hijos

    #### Horizontal

    | ![](../../../gitbook/assets/image%20%28109%29.png)  | ![](../../../gitbook/assets/image%20%28118%29.png)  |
    | :---: | :---: |


    Al activarlo el contenedor, permite mas objetos hijos sin que estos se encimen entre si o salgan del contenedor y da posibilidad de recorrer de izquierda a derecha el contenedor para visualizar todos los elementos hijos del contenedor

    ![](../../../gitbook/assets/image%20%2879%29.png)

    !!! danger

        Al activar esta función, las direcciones **alineado hacia arriba** y **alineado hacia abajo** se desactivan dejando disponibles solo **alineado a la izquierda** y **alineado a la derecha**


    #### Vertical

    | ![](../../../gitbook/assets/image%20%2888%29.png)  | ![](../../../gitbook/assets/image%20%28108%29.png)  |
    | :---: | :---: |


    Al activarlo el contenedor, permite mas objetos hijos sin que estos se encimen entre si o salgan del contenedor y da posibilidad de recorrer de arriba hacia abajo el contenedor para visualizar todos los elementos hijos del contenedor

    ![](../../../gitbook/assets/image%20%2898%29.png)

    !!! danger

        Al activar esta función, las direcciones **alineado a la izquierda** y **alineado a la derecha** se desactivan dejando disponibles solo **alineado hacia arriba** y **alineado hacia abajo**


    ### Control z-index

    Este elemento al activarlo \(cambiar el valor mayor a 0\) se sobrepone a los demás elementos utilizando la dimensión z como su punto base.

    ![](../../../gitbook/assets/image%20%2885%29.png)

    Al activar esta función, debemos de posicionar el elemento seleccionado, esto se logra tomando en cuenta las [dimensiones del contenedor](https://docs.apphive.io/global-functions/estilos/dimentions) así como el [outer margin](https://docs.apphive.io/global-functions/estilos/margins#outer-margin) y la posición del contenedor con respecto al contenedor al que queremos que se pose encima de él ya que estos nos permitirán la manipulación de la posición del contenedor en el eje z.

    !!! danger

        Las dimensiones deben ser en pixeles y no en porcentaje


    Si el contendor que queremos posicionar en el eje z esta por debajo de un contendor, debemos saber la altura de nuestro segundo contendor y el outer margin colocar el mismo valor pero en negativo en el valor superior , esto hará que el contenedor en posición z se sobreponga al primer contenedor y ambos bordes inferiores queden alineados \(imagen 1\), si se requiere  dejar un margen de espacio, basta con hacer mas pequeño el outer margin del contenedor en posición z \(imagen 2\)

    ![imagen 1](../../../gitbook/assets/image%20%2886%29.png)

    ![imagen 2](../../../gitbook/assets/image%20%28117%29.png)

    !!! warning

        Si el contenedor que vamos a posicionar en z se encuentra primero que el contenedor al que vamos a sobreponer nuestro contenedor, la lógica es la misma solo que en lugar de colocar el valor en el outer margin superior, lo colocamos en el inferior


    !!! info

        La misma lógica se aplica para los outer margin laterales


    ## Margins

    Los margins se utilizan para colocar una espacio entre elementos, ya sea de forma interna o de forma externa [ver más](https://docs.apphive.io/global-functions/estilos/margins)

    ## Shadows

    Con este elemento colocamos sombras a nuestro contenedor, tenemos 6 opciones de sombreado

    | Tipo de sombreado | Vista previa |
    | :---: | :---: |
    | ![](../../../gitbook/assets/image%20%28113%29.png)  |  ![](../../../gitbook/assets/image%20%2889%29.png)  |
    | ![](../../../gitbook/assets/image%20%2874%29.png)  | ![](../../../gitbook/assets/image%20%2884%29.png)  |
    | ![](../../../gitbook/assets/image%20%28122%29.png)  | ![](../../../gitbook/assets/image%20%2895%29.png)  |
    | ![](../../../gitbook/assets/image%20%28106%29.png)  | ![](../../../gitbook/assets/image%20%28111%29.png)  |
    | ![](../../../gitbook/assets/image%20%2887%29.png)  | ![](../../../gitbook/assets/image%20%2881%29.png)  |
    | ![](../../../gitbook/assets/image%20%2899%29.png)  | ![](../../../gitbook/assets/image%20%28115%29.png)  |

    De misma manera, podemos controlar que tan opaco se vería la sombra con la barra **Opacity**  que va de una escala de 0 a 1, siendo 0 transparente y 1 muy opaco

    ![](../../../gitbook/assets/image%20%2872%29.png)

    !!! warning

        El elemento **Shadows** solamente se puede activar cuando el contenedor tiene un color solido en el background, si el background es transparente, no se habilitará para su uso

=== "Data"

    ## Control Data

    ### Control name

    Nos sirve para cambiar el nombre al control [ver más](https://docs.apphive.io/global-functions/data/control-name)

    ### Enable dynamic loading

    Funciona para dar apariencia de cargado al elemento [ver más](https://docs.apphive.io/global-functions/data/enable-dynamic-loading)

    ### Control is hidden

    Funciona para poder ocultar los elementos [ver más](https://docs.apphive.io/global-functions/data/control-is-hidden)

    ## Layout

    ### Split percentage

    Esta propiedad nos facilita el poder dividir el contenedor de forma horizontal en el numero de secciones que sumadas deben se 100

    ![](../../../gitbook/assets/image%20%2897%29.png)

    Se pueden segmentar en partes iguales o en segmentes pequeños y grandes.

    se puede editar directamente el numero de sección, los numero deben ser separados por comas, pero con la restricción que la suma de los segmentos sea 100

    ![](../../../gitbook/assets/image%20%28107%29.png)

    Se puede segmentar también desde las opciones que nos ofrece de maneta directa

    ![](../../../gitbook/assets/image%20%28116%29.png)

    O ir aumentando o disminuyendo de segmentos con las opciones **+** , **-**

    ![](../../../gitbook/assets/image%20%2883%29.png)

    !!! info

        Si la suma de segmento no es 100, saldrá un mensa je de alerta ![](../../../gitbook/assets/image%20%28104%29.png) 


    ## Lock Container

    Permite bloquear el contenedor y no permite hacer edición de sus dimensiones

    ![](../../../gitbook/assets/image%20%28121%29.png)

=== "Events"

    ## OnPress

    ![](../../../gitbook/assets/image%20%28185%29.png)

    Se activa al presionar el control [ver más](https://docs.apphive.io/global-functions/events/onpress)

    ## OnReachEnd

    ![](../../../gitbook/assets/image%20%28184%29.png)

    Es un evento que trabaja en conjunto con la función Add Collection to UI, una vez cargada completamente la lista dinámica \(de la función Add Collection to UI\), este evento se activa para ejecutar las funciones que contenga

    [Generales del evento](https://docs.apphive.io/global-functions/events/generales-de-los-eventos)

    ## OnRefresh

    ![](../../../gitbook/assets/image%20%28179%29.png)

    Es un evento que trabaja en conjunto con la función Add Collection to UI, una vez cargada completamente la lista dinámica \(de la función Add Collection to UI\), puedes activar el evento deslizando hacia abajo la lista, generalmente este evento se utiliza para eliminar el caché de a lista y mostrar las nuevamente la lista con los registros nuevos \(si es que lo hay\).

    Este evento ayuda al menor consumo llamadas a la base de datos y ahorrar consumo de Megas de navegación

    [Generales del evento](https://docs.apphive.io/global-functions/events/generales-de-los-eventos)
