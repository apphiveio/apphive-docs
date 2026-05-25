# Geocoding

![](../../../../gitbook/assets/image%20%28648%29.png)

La función Geocoding permite obtener la información general de un punto geográfico especifico en el mapa.

[Información general](https://docs.apphive.io/reference/funciones/informacion-general-de-las-funciones) 



=== "Callbacks"

    ## Error

    Se activa cuando no se pudieron obtener los datos del punto geográfico, ya sea por un error interno del proceso o por la falta de la API key de Google y su conexión.

    ## Success

    Se activa al obtener la información del punto geográfico, retorna la información obtenida.

    La información comprende las coordenadas del punto geográfico, el nombre de la calle, ciudad, país y todas sus variaciones de la dirección de punto.

=== "Entry Vars"

    ## latitude

    ![](../../../../gitbook/assets/image%20%28642%29.png)

    Se agregar el dato de la latitud del punto geográfico a obtener su información

    ## longitude

    ![](../../../../gitbook/assets/image%20%28650%29.png)

    Se agregar el dato de la longitude del punto geográfico a obtener su información
