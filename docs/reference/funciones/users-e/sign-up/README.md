# Sign Up

La función Sign up permite a los usuarios acceder a la aplicación registrando sus datos. Los usuarios suelen rellenar formularios con un "nombre de usuario", "contraseña", "número de teléfono" y "correo electrónico".

![](../../../../gitbook/assets/image%20%28353%29.png)

[Información general](https://docs.apphive.io/reference/funciones/informacion-general-de-las-funciones)



=== "Callbacks"

    ## Error registering

    Se activa cuando sucede un error en el proceso de registro del usuario, estos errores puedes suceder por que el correo no tiene una estructura especifica, la contraseña es menor de 6 dígitos no se llenó algun campo \(exceptuando Phone\) o por que ocurrió un proceso interno

    ## Success

    Se activa cuando se crea el registro de forma exitosa

    ## User is already signed in

    Se activa cuando las credenciales que se ingresan coinciden con las de otro usuario que había creado una sesión de usuario con los mismos datos

=== "Entry Vars"

    ## Email

    Se debe ingresar un correo con estructura valida



    ## Name

    Se debe ingresar un nombre con estructura valida



    ## Password

    Se debe ingresar una contraseña con un mínimo de 6 dígitos



    ## Phone

    Se debe ingresar un numero telefónico de 10 dígitos o que tengan integrada la lada nacional

    !!! info

        Este parámetro es opcional del ingresar
