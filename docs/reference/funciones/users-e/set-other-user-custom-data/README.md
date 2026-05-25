# Set other user custom data

![](../../../../gitbook/assets/image%20%28584%29.png)

La función Set other user custom data permite agregar una variable personalizada a la información del usuario, sin importar en que aplicación se encuentre el usuario, pero debe estar dentro del mismo proyecto en que se llama esta función.

[Información general](https://docs.apphive.io/reference/funciones/informacion-general-de-las-funciones) 



=== "Callbacks"

    ## Error updating data

    Se activa cuando ocurre un error durante el proceso de asignarle la nueva variable al usuario

    ## Success updating data

    Se activa cuando se se agregar de forma exitosa la variable personalizada 

=== "Entry Vars"

    ## appId

    ![](../../../../gitbook/assets/image%20%28594%29.png)

    Permite seleccionar una aplicación para poder agregar una variable extra a alguno de los usuarios de la misma aplicación.

    ## Key

    ![](../../../../gitbook/assets/image%20%28605%29.png)

    Permite crear la variable personalizada para poder agregarle al usuario

    ## userId

    ![](../../../../gitbook/assets/image%20%28631%29.png)

    Se ingresa el id del usuario a quien se le desea agregar la variable nueva

    !!! info

        el usuario debe corresponder a los usuarios pertenencientes a la app seleccionada en **appId**


    ## Value

    ![](../../../../gitbook/assets/image%20%28607%29.png)

    Permite agregar un valor a la variable personalizada creada en la entry var **Key**
