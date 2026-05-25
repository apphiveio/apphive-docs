# Start geolocation tracking

![](../../../../gitbook/assets/image%20%28657%29.png)

La función Start geolocation tracking permite realizar el rastreo del dispositivo en primer y segundo plano, siguiendo como parámetro principal la distancia desde un punto inicial hasta que se mueva a una distancia establecida por las configuraciones asignadas por el usuario

[Información general](https://docs.apphive.io/reference/funciones/informacion-general-de-las-funciones)



=== "Callbacks"

    ## Error getting location

    Se activa cuando sucede un error al obtener la ubicación del dispositivo una vez alcanzado la distancia establecida en **Distance filter** desde el punto de origen hasta la ubicación actual.

    ## On location change

    Se activa cuando se alcanzó la distancia establecida en **Distance filter** desde el punto de origen hasta el punto actual.

    !!! warning

        Cuando se ejecuta en segundo plano, el tiempo de vida de las funciones dentro del callback se limita en la memoria de ejecución a medio segundo, este tiempo varia dependiendo del modelo del dispositivo, pasando este tiempo mata los procesos que se encuentren en ejecución

=== "Entry Vars"

    ## Desired accuracy

    ![](../../../../gitbook/assets/image%20%28663%29.png)

    Permite seleccionar la precisión con que se ubicará la posición del dispositivo rastreado.

    | Nombre | Proveedor de ubicación | Descripción |
    | :--- | :--- | :--- |
    | DESIRED\__ACCURACY\_HIGH_ | GPS+Wifi+Red Celular | Consumo de energía alto y precisión de ubicación alta |
    | DESIRED\__ACCURACY\_MEDIUM_ | Wifi+Red Celular | Consumo de energía medio y precisión de ubicación medio |
    | DESIRED\__ACCURACY\_LOW_ | Wifi \(baja energia\) +Red Celular | Menor consumo de energía y precisión de ubicación baja |
    | DESIRED\__ACCURACY\_VERY\_LOW_ | Red Celular | Mucho menos consumo de energía y precisión de ubicación muy baja  |

    ## Distance filter

    ![](../../../../gitbook/assets/image%20%28670%29.png)

    Establece un radio de distancia que activa la función cuando el usuario llega del punto original a la distancia establecida en la entry var

    ## Should show debug notifs

    ![](../../../../gitbook/assets/image%20%28681%29.png)

    Cuando se activa muestra una notificación cada vez que se dispara la función \(solo para pruebas\)

    ## Stop on terminate

    ![](../../../../gitbook/assets/image%20%28686%29.png)

    Cuando se encuentra activado va a detener el rastreo en cuento se cambie de aplicación o cambie de pantalla, si se encuentra desactivado, va a continuar el rastreo en segundo plano
