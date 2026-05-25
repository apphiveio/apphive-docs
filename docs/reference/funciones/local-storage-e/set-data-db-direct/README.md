# Set data DB direct

![](../../../../gitbook/assets/image%20%28629%29.png)

  
La función Set data DB direct permite agregar información en un registro de forma directa.‌

En comparación de la función Save in DB, esta función solamente permite agregar información en un único campo‌

​[Información general](https://docs.apphive.io/reference/funciones/informacion-general-de-las-funciones)



=== "Callbacks"

    ## Error

    Se activa cuando sucede algún error durante el proceso de guardar la información ya sea por que no es la tura correcta o por un error interno

    ## Success

    Se activa cuando el proceso de guardado se ejecuta de forma exitosa

=== "Entry Vars"

    ## Data

    ![](../../../../gitbook/assets/image%20%28632%29.png)

    Se ingresa la información que va a ser guardada dentro de un registro de una colección de datos

    ## Path

    ![](../../../../gitbook/assets/image%20%28630%29.png)

    Permite agregar la ruta en donde se va a guardar la información de la entry var Data

    ### Conseguir ruta

    Abrir la función **Delete local storage data** y presionar en el botón

    ![](../../../../gitbook/assets/image%20%28591%29.png)

    Esta opción permite abrir una ventana en donde se puede seleccionar la ruta y campo especifico para guardar la información.

    ![](../../../../gitbook/assets/image%20%28592%29.png)

    Una vez indicando la ruta, se debe copiar la ruta que se muestra en la parte superior de la ventana y pegarla en la entry var de **Path**

    ![](../../../../gitbook/assets/image%20%28618%29.png)

    Una vez obtenida la ruta puedes eliminar la función **Delete local storage data**
