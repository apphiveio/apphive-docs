# Copy Data From Path

![](../../../../gitbook/assets/image%20%28603%29.png)

La función Copy Data From Path permite copiar o mover la información de una colección de datos a otra dentro de la base de datos.

!!! danger

    Se copia la información, mas no la estructura de la base de datos, es decir que si no se tiene una estructura similar a la del origen es probable que no vea la información completa que copie o mueva.


!!! warning

    El hecho de que no vea la información no significa que no se haya hecho la operación de forma correcta, para poder visualizarla, se debe crear una estructura similar al path del origen en el path de destino.


[Información general](https://docs.apphive.io/reference/funciones/informacion-general-de-las-funciones) 



=== "Callbacks"

    ## Error

    Se activa cuando sucede un error durante el proceso especificado por la función

    ## No data origin

    Se activa cuando no se encuentra información en el origen para poder realizar el proceso especificado por la función

    ## Success

    Se activa cuando concluye el proceso de forma exitosa

=== "Entry Vars"

    ## Operation

    ![](../../../../gitbook/assets/image%20%28600%29.png)

    Permite seleccionar el tipo de acción que se va a realizar en la base de datos, las acciones son copiar o mover la información

    ## Origin

    ![](../../../../gitbook/assets/image%20%28585%29.png)

    Permite seleccionar la ruta de origen de la base de datos para realizar la operación previamente seleccionada,

    ## Target

    ![](../../../../gitbook/assets/image%20%28598%29.png)

    Permite seleccionar la ruta de destino en donde se realizará la acción previamente seleccionada



    ### Open database browser

    ![](../../../../gitbook/assets/image%20%28591%29.png)

    Esta opción permite abrir una ventana en donde se puede seleccionar la ruta especifica para poder elegir el origen y destino de la información

    Si se desea ingresar a un registro en particular, se debe agregar el id en el identifier para poder ingresar al siguiente subnivel de la colección.

    ![](../../../../gitbook/assets/image%20%28590%29.png)

    Si se desea copiar o mover una colección de datos completa solamente se debe de elegir la colección

    ![](../../../../gitbook/assets/image%20%28362%29.png)
