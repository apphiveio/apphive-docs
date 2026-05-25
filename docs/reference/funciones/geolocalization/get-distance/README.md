# Get distance

![](../../../../gitbook/assets/image%20%28641%29.png)

La función Get distance permite obtener la distancia de un punto geográfico A a un punto geográfico B; pudiendo ser distancia por ruta o distancia lineal.

La distancia de ruta es calculada por los servidores de Google, mientras que la distancia lineal es del forma interna por la lógica de Apphive.

La distancia por ruta retorna la distancia de la ruta optima, esta ruta optima al ser calculada por los servidores de Google, puede retornarte la ruta con menor distancia o la ruta con menor tiempo de recorrido, para poder llegar de un punto a otro.

[Información general](https://docs.apphive.io/reference/funciones/informacion-general-de-las-funciones) 



=== "Callbacks"

    ## Error

    Se activa cuando ocurre un error en el proceso de obtención de la distancia entre los puntos geográficos. El error puede deberse a un error interno o por la falta de la API key de Google y su conexión.

    ## Success

    Se activa cuando se pudo obtener la distancia entre ambos puntos, retornando la distancia en kilómetros y metros y el tiempo estimado de recorrido en segundos.

=== "Entry Vars"

    ## Latitude destination

    ![](../../../../gitbook/assets/image%20%28639%29.png)

    Permite agregar la latitud del punto geográfico de destino

    ## Latitude origin

    ![](../../../../gitbook/assets/image%20%28647%29.png)

    Permite agregar la latitud del punto geográfico de origen

    ## Longitude destination

    ![](../../../../gitbook/assets/image%20%28638%29.png)

    Permite agregar la longitud del punto geográfico de destino

    ## Longitude origin

    ![](../../../../gitbook/assets/image%20%28643%29.png)

    Permite agregar la longitud del punto geográfico de origen

    ![](../../../../gitbook/assets/image%20%28649%29.png)

    Permite seleccionar el modo de ruta.

    * **Lineal:** Retorna la distancia lineal del punto geográfico de origen al punto geográfico de destino
    * **Route:** Retorna la distancia de ruta del punto geográfico de origen al punto geográfico de destino, esta distancia depende numero de calles que se tenga que recorrer y del sentido de las calles, por lo que es importante definir cual es el punto de origen y cual el de destino.
