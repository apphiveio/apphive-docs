---
description: >-
  Permite cambiar la contraseña de la sesión que se encuentra activa en el
  momento
---

# Change my password

![](../../../../gitbook/assets/image%20%28348%29.png)

[Información general](https://docs.apphive.io/reference/funciones/informacion-general-de-las-funciones)



=== "Callbacks"

    ## Password changed successfully

    Se activa cuando la contraseña se cambió de forma satisfactoria

    ## Error changing password

    Se activa cuando sucedió algún tipo de error durante el cambio de la actualización, retornando el tipo de error que sucedió durante el proceso 

    !!! warning

        Para poder ver el tipo de error es necesario mostrarlo con la función send alert 

=== "Entry Vars"

    ## New password

    ![](../../../../gitbook/assets/image%20%28366%29.png)

    Permite agregar la nueva contraseña para la sesión que se encuentra activa

    !!! info

        El valor a ingresar debe ser mayor a 6 dígitos
