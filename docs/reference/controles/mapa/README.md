---
description: >-
  Un mapa es una representación gráfica simplificada de un territorio con
  propiedades métricas sobre una superficie bidimensional
---

# Map

![](../../../gitbook/assets/image%20%28231%29.png)



=== "Style"

    ## Dimentions

    Permite cambiar el valor del ancho y alto del componente [ver más](https://docs.apphive.io/global-functions/estilos/dimentions)

=== "Data"

    ## Map Options

    ### Latitude

    ![](../../../gitbook/assets/image%20%28284%29.png)

    ### Longitude

    ![](../../../gitbook/assets/image%20%28261%29.png)

    La latitude y longitude se utilizan para poner por defecto la ubicación inicial del mapa, estas coordenadas tienen un valor por defecto pero se pueden modificar a la preferencia del desarrollador

    ### Zoom

    ![](../../../gitbook/assets/image%20%28277%29.png)

    Esta propiedad nos permite hacer un acercamiento en el mapa para poder visualizar las áreas de nuestro interés pudiendo ser demasiado cerca para obtener la vista de cierto numero de calles o tan lejos para poder ver grandes extensiones de territorio sus valores se manejan entre 0 y 100 pudiendo agregar decimales o milésimas.

    ### isDisabled

    ![](../../../gitbook/assets/image%20%28276%29.png)

    Al habilitar el switch el mapa no se puede alterar de ninguna forma de manera manual, es decir que no se puede arrastrar para poder ver otra área distinta a la que se ve actualmente así mismo no se puede hacer algún tipo de zoom

    ### Map center icon image

    ![](../../../gitbook/assets/image%20%28266%29.png)

    Al activar el switch se genera un marcador predefinido n el centro del mapa, la ubicación de este marcador indica las coordenadas actuales del punto que indica el mapa

    El [Background image](https://docs.apphive.io/global-functions/estilos/background-image) sirve para sustituir el icono predefinido por uno de la elección del usuario

    ### Enable dynamic loading

    ![](../../../gitbook/assets/image%20%28151%29.png)

    Funciona para dar apariencia de cargado al elemento [ver más](https://docs.apphive.io/global-functions/data/enable-dynamic-loading)

    ### Control is hidden

    ![](../../../gitbook/assets/image%20%28150%29.png)

    Oculta los controles cuando se activa [ver más](https://docs.apphive.io/global-functions/data/control-is-hidden)

    ### Show Current Location Pointer

    ![](../../../gitbook/assets/image%20%28269%29.png)

    Muestra la ubicación en tiempo real de nuestra ubicación independientemente de donde esté situadas las coordenadas  el marcador en el mapa

=== "Events"

    ## onMarkerPressed

    ![](../../../gitbook/assets/image%20%28260%29.png)

    Este evento se activa cuando se presiona algún marker, al hacer click en alguno de los markers sus coordenadas se tomará como principales, ubicando la posición principal del mapa en éstas.

    !!! danger

        No es al presionar el market que se activa en las opciones de data, sino las que se visualizan cuando se hace uso de la función Query Fire Geolocation


    ## onRegionChange

    ![](../../../gitbook/assets/image%20%28241%29.png)

    Este evento se activa cuando las coordenadas tienen un cabio por mínimo que sea, se comporta como un listener y se activa en todo momento que exista algun tipo de variación de coordenadas

    ## onRegionChangeComplete

    ![](../../../gitbook/assets/image%20%28268%29.png)

    A diferencia del evento onRegionChange este evento se activa una vez terminemos de mover la ubicación en el mapa, y ya no tengan alguna variación las coordenadas del mapa
