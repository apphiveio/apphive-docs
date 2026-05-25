# Login

La función Login permite a los usuarios acceder a la aplicación identificándose y autentificándose. los usuarios deben llenar un formulario con un correo y una contraseña que coincidan con un usuario creado anteriormente

![](../../../../gitbook/assets/image%20%28352%29.png)

  
 ​[Información general](https://docs.apphive.io/reference/funciones/informacion-general-de-las-funciones)



=== "Callbacks"

    ## Error login

    Se activa cuando ocurre un error en el proceso de autentificación del usuario

    ## Invalid credentials

    Se activa cuando la autentificación de los usuarios es errónea, por que los datos \(Correo o Contraseña\) presentan alguna inconsistencia que no coincide con ninguna de las cuentas de usuario registradas en la aplicación en cuestión

    ## Successful login

    Se activa cuando el proceso de autentificación se realizó correctamente creando una sesión que permite el acceso a los datos asociados y su contenido privado con ese usuario dentro de la aplicación correspondiente

=== "Entry Vars"

    ## Email

    Se debe ingresar un correo con el que el usuario creó una cuenta de usuario anteriormente

    ## Password

    Se debe ingresar la contraseña que coincida con la cuenta de usuario del correo que se integró anteriormente
