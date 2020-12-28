# Callbacks

## Error getting location

Se activa cuando sucede un error al obtener la ubicación del dispositivo una vez alcanzado la distancia establecida en **Distance filter** desde el punto de origen hasta la ubicación actual.

## On location change

Se activa cuando se alcanzó la distancia establecida en **Distance filter** desde el punto de origen hasta el punto actual.

{% hint style="warning" %}
Cuando se ejecuta en segundo plano, el tiempo de vida de las funciones dentro del callback se limita en la memoria de ejecución a medio segundo, este tiempo varia dependiendo del modelo del dispositivo, pasando este tiempo mata los procesos que se encuentren en ejecución
{% endhint %}

