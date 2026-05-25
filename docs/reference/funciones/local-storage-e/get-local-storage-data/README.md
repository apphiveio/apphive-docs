# Get local storage data

![](../../../../gitbook/assets/image%20%28428%29.png)

Permite realizar consultas de información a la base de datos local en el dispositivo 

!!! danger

    El tipo de información almacenado en y consultado en la base depende directamente del tipo de información que maneje el usuario dependiendo su interacción con la misma


[Información general](https://docs.apphive.io/reference/funciones/informacion-general-de-las-funciones)



=== "Callbacks"

    ## Error retrieving data

    Se activa cuando ocurre algun tipo de error al obtener los datos requeridos en el dispositivo

    ## Empty data

    Se activa cuando no se encuentran registros en una colección de información o no se encontró coincidencias en la búsqueda de un registro en especifico

    ## Success retrieving data

    Se activa cuando se recuperaron los datos de forma exitosa y retorna los datos encontrados en la consulta.

=== "Entry Vars"

    ## Is real time

    ![](../../../../gitbook/assets/image%20%28419%29.png)

    Se activa cuando se requiere que la función Get  local storage data se llame cuando alguno de los valores dentro del Path seleccionado en la base sufra de algún tipo de modificación, es decir que se agregue un registro, se modifique o se elimine

    ![](../../../../gitbook/assets/image%20%28421%29.png)

    Permite abrir una ventada en donde se encuentra la estructura de nuestra pase de datos para poder seleccionar las rutas de donde se desea extraer la información

    ![](../../../../gitbook/assets/image%20%28376%29.png)

    Al no agregar un valor en Identifier se puede hacer consulta de toda la información que se elige de la colección de datos.

    Cuando se agrega un valor en Identifier el sistema buscará en la colección de datos el registro en donde el record id coincida con el Identifiar asignado
