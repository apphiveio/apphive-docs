# Query fire geolocation

![](../../../../gitbook/assets/image%20%28570%29.png)

La función Query fire geolocation permite obtener un numero determinado de registros de un grupo del Geo Fire, estos registros son consultados se muestran  si se encuentran dentro de un radio de un punto geográfico asignado en las entry vars

[Información general](https://docs.apphive.io/reference/funciones/informacion-general-de-las-funciones) 



=== "Callbacks"

    ## Error at make query

    Se activa cuando surge un error durante el proceso de la consulta de la información del grupo de Geo Fire

    ## New key location entered

    Se activa cada vez que se encuentra un marcador nuevo dentro del área especificada

    ## Key location exited

    Se activa cada vez que un marcador sale del área especificada

    ## Key location moved

    Se activa cada ver que el punto central cambia de posición respecto al original

=== "Entry Vars"

    ## Group name

    ![](../../../../gitbook/assets/image%20%28569%29.png)

    Permite seleccionar el grupo o categoria desde donde se hará la consulta de la información

    ## Center latitude

    ![](../../../../gitbook/assets/image%20%28562%29.png)

    Permite agregar la latitud desde donde será el centro de consulta

    ## Center longitude

    ![](../../../../gitbook/assets/image%20%28567%29.png)

    Permite agregar la longitud desde donde será el centro de consulta

    ## Radius \(km\)

    ![](../../../../gitbook/assets/image%20%28566%29.png)

    Permite agregar una distancia en kilómetros, que servirá como distancia de radio generando un área circular, todos los marcadores que se encuentren dentro de esta área se mostrarán el mapa, lo que se encuentren fuera del área no serán mostrados.
