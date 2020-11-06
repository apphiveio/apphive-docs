# Events

## onMarkerPressed

![](../../../.gitbook/assets/image%20%28260%29.png)

Este evento se activa cuando se presiona algún marker, al hacer click en alguno de los markers sus coordenadas se tomará como principales, ubicando la posición principal del mapa en éstas.

{% hint style="danger" %}
No es al presionar el market que se activa en las opciones de data, sino las que se visualizan cuando se hace uso de la función Query Fire Geolocation
{% endhint %}

## onRegionChange

![](../../../.gitbook/assets/image%20%28241%29.png)

Este evento se activa cuando las coordenadas tienen un cabio por mínimo que sea, se comporta como un listener y se activa en todo momento que exista algun tipo de variación de coordenadas

## onRegionChangeComplete

![](../../../.gitbook/assets/image%20%28268%29.png)

A diferencia del evento onRegionChange este evento se activa una vez terminemos de mover la ubicación en el mapa, y ya no tengan alguna variación las coordenadas del mapa

