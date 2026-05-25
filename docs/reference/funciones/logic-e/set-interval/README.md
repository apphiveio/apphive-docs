# Set interval

![](../../../../gitbook/assets/image%20%28499%29.png)

La función Set interval permite crear iteraciones controladas por tiempos, de esta manera cuando culmine el tiempo especificado se ejecutarán las funciones asignadas por la lógica

[Información general](https://docs.apphive.io/reference/funciones/informacion-general-de-las-funciones)



=== "Callbacks"

    ## On done

    Se activa cada vez que transcurre el tiempo determinado en la entry var de la función, ejecutando las funciones que se encuentran dentro de este callback

    ## On register

    Se activa la primera vez que se comienza a ejecutar la función creando un id de intervalo, dicho id puede ser guardado en alguna variable global, local o en algún registro de las bases de datos

    !!! info

        Cada función de Set interval genera un id distinto

=== "Entry Vars"

    ## Time\(seconds\)

    ![](../../../../gitbook/assets/image%20%28500%29.png)

    Permite agregar valor numérico de un tiempo determinado en segundos
