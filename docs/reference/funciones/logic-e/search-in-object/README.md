# Search in Object

![](../../../../gitbook/assets/image%20%28476%29.png)

La función Search in Object permite buscar un determinado conjunto de registros dentro de un objeto, que tengan coincidencia de valores en una ruta especifica

[Información general](https://docs.apphive.io/reference/funciones/informacion-general-de-las-funciones)



=== "Callbacks"

    ## On Match

    Se activa una vez que se encontraron y retornará los registros que tuvieron coincidencias dentro del objeto, de igual manera si no encuentra coincidencias, no retornará nada, el tipo de retorno es un objeto

=== "Entry Vars"

    ## Object

    ![](../../../../gitbook/assets/image%20%28488%29.png)

    Permite asignar el objeto desde donde se hará la búsqueda y se filtrarán los registros que cumplan con el parámetro especifico

    ## Path

    ![](../../../../gitbook/assets/image%20%28481%29.png)

    Permite asignar la ruta de en donde se va a hacer la comparación del parámetro y encuentre las coincidencias

    ## valueToMatch

    ![](../../../../gitbook/assets/image%20%28485%29.png)

    Es el valor con el que se buscará las coincidencias dentro del objeto
