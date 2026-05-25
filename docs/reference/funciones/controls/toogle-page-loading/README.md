# Toogle page loading

![](../../../../gitbook/assets/image%20%28596%29.png)

La función Toogle page loading permite al usuario mostrar un loader que se superpone a la pantalla, impidiendo acción de la misma, se utiliza como indicador de carga, para darle tiempo de respuesta a las funciones que se renderizan

[Información general](https://docs.apphive.io/reference/funciones/informacion-general-de-las-funciones) 



=== "Entry Vars"

    ## onlyDisable

    ![](../../../../gitbook/assets/image%20%28614%29.png)

    Permite desactivar el loader cuando se activa el switch, generalmente se utiliza en los callbacks de las funciones que se renderizan al final, esto para asegurar que todas las funciones tengan el tiempo suficiente de cumplir su función; puede haber mas de uno, dependiendo de los callbacks de las funciones, ya sean de error o de éxito.

    ## onlyEnable

    ![](../../../../gitbook/assets/image%20%28580%29.png)

    Permite activar el loader cuando se activa el switch, generalmente se utiliza al inicio de los eventos y solo se utiliza una vez
