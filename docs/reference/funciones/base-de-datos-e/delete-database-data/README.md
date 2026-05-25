# Delete database data

![](../../../../gitbook/assets/image%20%28341%29.png)

Esta función perite eliminar registros específicos de una colección de datos, una colección completa de datos de la base de datos 



=== "Callbacks"

    ## Error deleting data

    Se activa cuando sucede un error en el proceso de borrar en la base de datos, ya sea por una mala conexión o un proceso fallido mientras se realza la tarea

    ## Data deleted

    Se activa cuando el proceso de eliminar la información se culminó exitosamente

=== "Entry Vars"

    ## Should update db cache

    ![](../../../../gitbook/assets/image%20%28358%29.png)

    Cuando se activa esta función, se puede actualizar el caché de la base de datos

    ## Updates to make to the db

    ![](../../../../gitbook/assets/image%20%28343%29.png)

    Con esta opción podemos abrir una ventana en donde se puede seleccionar la ruta especifica de en donde se va a realizar el proceso de borrar información.

    Si se desea eliminar un registro en particular, se debe agregar el id del registro dentro de la colección de información 

    ![](../../../../gitbook/assets/image%20%28356%29.png)

    Si se desea borrar una colección de datos completa solamente se debe de elegir la colección

    ![](../../../../gitbook/assets/image%20%28362%29.png)
