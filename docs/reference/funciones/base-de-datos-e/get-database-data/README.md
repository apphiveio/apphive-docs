# Get Database Data

La función Get database data nos perite consultar información cargada en la base de datos de la nube, permite consultar una colección completa de registro, registros en especifico o un campo con concreto de un registro, esta consulta de información puede obtenerse al cualquier numero de subniveles, dependiendo de la estructura de la colección dentro de la base de datos.

![](../../../../gitbook/assets/image%20%28379%29.png)

​[Información general](https://docs.apphive.io/reference/funciones/informacion-general-de-las-funciones)



=== "Callbacks"

    ## Permission denied

    Se activa cuando el punto desde donde se hace la consulta no cuenta con los permisos suficientes para consultar información de la base de datos

    ## End

    Se activa cuando el tiempo de vida al solicitar el proceso termina y la función no pudo completar la tarea de ninguna manera

    ## Empty data

    Se activa cuando la consulta no encuentra ningún tipo de datos o coincidencia en la ruta especificada

    ## Data obtained

    Se activa cuando se encuentra información en la ruta especificada retornando la información encontrada

=== "Entry Vars"

    ## End at

    ![](../../../../gitbook/assets/image%20%28368%29.png)



    ## Filter

    ![](../../../../gitbook/assets/image%20%28384%29.png)

    Permite agregar algun valor con el que realzará comparaciones en los registros de las colecciones de la base de datos



    ## Is real time

    ![](../../../../gitbook/assets/image%20%28372%29.png)

    Se activa cuando se requiere que la función Get database data se llame cuando alguno de los valores dentro del Path seleccionado en la base sufra de algún tipo de modificación es decir que se agregue un registro, se modifique o se elimine



    ## Limit to First

    ![](../../../../gitbook/assets/image%20%28367%29.png)

    Muestra un determinado nuero de registros de los primeros que fueron creados



    ## Limit to last

    ![](../../../../gitbook/assets/image%20%28381%29.png)

    Muestra un determinado nuero de registros de los últimos que fueron creados



    ## Order by

    ![](../../../../gitbook/assets/image%20%28374%29.png)

    Esta Entry Vars va de la mano con Filter, ya que esta es la que se encarga de asignar un campo en donde se hará la búsqueda del filtro dentro de la colección de datos



    ## Path on DB

    ![](../../../../gitbook/assets/image%20%28375%29.png)

    Permite abrir una ventada en donde se encuentra la estructura de nuestra pase de datos para poder seleccionar las rutas de donde se desea extraer la información

    ![](../../../../gitbook/assets/image%20%28376%29.png)

    Al no agregar un valor en Identifier se puede hacer consulta de toda la información que se elige de la colección de datos.

    Cuando se agrega un valor en Identifier el sistema buscará en la colección de datos el registro en donde el record id coincida con el Identifiar asignado

    ## Start at

    ![](../../../../gitbook/assets/image%20%28369%29.png)



    ## Time to refresh  \(seconds\)

    ![](../../../../gitbook/assets/image%20%28373%29.png)

    Cuando se asigna un valor numérico en este parámetro, es el numero de segundo en que la base de datos tomará en cuenta los cambios realizados en los registros, es decir que si se eliminan, modifican o agregan registros o valores, no se podrán notar hasta que el tiempo designado haya transcurrido 
