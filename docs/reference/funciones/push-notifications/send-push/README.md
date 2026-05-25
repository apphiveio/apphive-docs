# Send push

![](../../../../gitbook/assets/image%20%28556%29.png)

La función send push permite al usuario enviar notificaciones push a las aplicaciones que se encuentren dentro del mismo proyecto que la app que enviará los mensajes

Al llegar la notificación se activará un sonido por defecto

!!! warning

    El sonido sonará siempre y cuando el dispositivo no se encuentre en vibrador, en silencio o en modo avión


[Información general](https://docs.apphive.io/reference/funciones/informacion-general-de-las-funciones) 



=== "Callbacks"

    ## Error sending notification

    Se activa cuando ocurre un error durante el proceso de enviar la notificación

    No se envía la notificación

    ## Notification sent

    Se activa cuando la notificación push se envia

=== "Entry Vars"

    ## Android visibility

    ![](../../../../gitbook/assets/image%20%28538%29.png)

    Permite seleccionar el tipo de mensaje para mostrar la notificación, siendo privado, publico o secreto

    !!! warning

        Solo para Android para iOS es por defecto del sistema


    ## body

    ![](../../../../gitbook/assets/image%20%28548%29.png)

    Permite agregar el cuerpo del mensaje mostrándose en el mensaje push

    ## Send to all

    ![](../../../../gitbook/assets/image%20%28549%29.png)

    Al activar el switch indica que la notificación se mandará a todos los usuarios de la app seleccionada

    ## Target app

    ![](../../../../gitbook/assets/image%20%28539%29.png)

    Permite seleccionar la aplicación dentro del proyecto y mandar las notificaciones push a el/los usuario\(s\) pertenecientes a la aplicaciones

    ### App process

    ![](../../../../gitbook/assets/image%20%28545%29.png)

    Esta sección se encontrará oculta hasta el momento de seleccionar una aplicación, cuando se des oculte mostrará los App Processes pertenecientes a esa aplicación

    !!! danger

        Es indispensable elegir un App processes para que la función send push realice su proceso de forma adecuada


    !!! info

        Si el App Process cuenta con Entry Vars estas aparecerán para poder mandar los valores para que el proceso realice su función de forma exitosa


    ## Target user email

    ![](../../../../gitbook/assets/image%20%28535%29.png)

    Permite ingresar el correo del usuario a quien se le enviará la notificación push

    ## Target User Uid

    ![](../../../../gitbook/assets/image%20%28540%29.png)

    Permite ingresar el id del usuario a quien se le enviará la notificación push

    ## title

    ![](../../../../gitbook/assets/image%20%28558%29.png)

    Permite agregar el titulo con el que se mostrará la notificación push
