# Upload file

![](../../../../gitbook/assets/image%20%28413%29.png)

Permite cargar archivos y guardarlos en la base de datos para poder tener acceso remoto a ellas

Puede aceptar archivos de música, documentos, imágenes y retornar una dirección para poder tener acceso a la misma.

​[Información general](https://docs.apphive.io/reference/funciones/informacion-general-de-las-funciones)



=== "Callbacks"

    ## Error uploading file

    Se activa cuando ocurre algún tipo de error durante la carga del archivo en la base de datos

    ## File uploaded

    Se activa cuando el proceso de carga se ejecuta de forma exitosa, y retorna la dirección en la base de datos del archivo que se cargó

=== "Entry Vars"

    ## Max file size \(MB\)

    ![](../../../../gitbook/assets/image%20%28412%29.png)

    Permite seleccionar el tamaño máximo del archivo que se va a cargar, el numero que ingreses será interpretado en megabytes

    ## Permission request message

    ![](../../../../gitbook/assets/image%20%28410%29.png)

    Permite agrega un mensaje de permiso para el usuario, si es que no cuenta con los permisos necesarios para que la función se ejecute

    ## Permission request title

    ![](../../../../gitbook/assets/image%20%28414%29.png)

    Permite agrega el título del mensaje de permiso para el usuario, si es que no cuenta con los permisos necesarios para que la función se ejecute

    ## URI

    ![](../../../../gitbook/assets/image%20%28415%29.png)

    Permite abstraer el archivo del componente o control para poder cargarlo en la base de datos
