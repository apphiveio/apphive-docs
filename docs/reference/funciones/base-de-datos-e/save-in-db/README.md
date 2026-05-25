# Save in DB

La función Save in DB permite al usuario guardar información en forma de objeto en una estructura de árbol, esta información se guarda en formato json

![](../../../../gitbook/assets/image%20%28382%29.png)

​[Información general](https://docs.apphive.io/reference/funciones/informacion-general-de-las-funciones)



=== "Callbacks"

    ## Error saving data

    Se activa cuando ocurre algún tipo de error en el momento del proceso de guardado en la base de datos

    ## End

    Se activa cuando se termina el tiempo asignado al proceso, pero no pudo realizar la acción y tampoco tuvo algún tipo de error

    ## Data saved

    Se activa cuando el proceso de guardado de información concluye de forma exitosa

=== "Entry Vars"

    ## Should update db cache

    ![](../../../../gitbook/assets/image%20%28370%29.png)

    Cuando se activa esta función, se puede actualizar el caché de la base de datos

    ## Updates to make to the db

    ![](../../../../gitbook/assets/image%20%28385%29.png)

    Con esta opción podemos abrir una ventana en donde se puede seleccionar la ruta especifica de en donde se va a realizar el proceso de guardar información.

    Al presionar el botón Open database browser se abrirá una pequeña ventana para que puedas seleccionar la ruta de en donde se guardará la información necesaria

    ![](../../../../gitbook/assets/image%20%28399%29.png)

    Por defecto se agrega un id aleatorio en identifier para que los Record id de los registros nunca se dupliquen y en cada uno de los campos de la base de datos se puede integra información que se puede agregar de forma manual \(texto crudo\) o con variables que se encuentren dentro de la [tabla de controles](https://docs.apphive.io/reference/funciones/tabla-de-controles)

    ![](../../../../gitbook/assets/image%20%28402%29.png)
