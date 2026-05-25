# Update AuthInfo

![](../../../../gitbook/assets/image%20%28636%29.png)

La función Update AuthInform permite actualizar información por defecto del usuario que tiene su sesión activa

[Información general](https://docs.apphive.io/reference/funciones/informacion-general-de-las-funciones) 



=== "Callbacks"

    ## error

    Se activa cuando se genera un error durante el proceso de actualización de información del usuario

    ## Finally

    Se activa cuando termina el tiempo determinado para realizar la acción y la función no realizó ningún cambio

    ## notLoggedIn

    Se activa cuando el sistema no encuentra una sesión iniciada para poder cambiar la información del usuario

    ## then

    Se activa cuando se realizó de forma exitosa el proceso de modificación de información.

=== "Entry Vars"

    ## Key

    ![](../../../../gitbook/assets/image%20%28624%29.png)

    Muestra las variables por defecto de los usuarios, estos keys no muestran las variables personalizadas que se pudiesen agregar al usuario.

    ![](../../../../gitbook/assets/image%20%28583%29.png)

    ## Value

    ![](../../../../gitbook/assets/image%20%28625%29.png)

    Permite agregarle la nueva información a la variable seleccionada previamente
