# Range Iteration

![](../../../../gitbook/assets/image%20%28452%29.png)

La función rangeIteration permite generar un numero especifico de iteraciones, para tener el control en el numero ejecuciones de las funciones

[Información general](https://docs.apphive.io/reference/funciones/informacion-general-de-las-funciones)



=== "Callbacks"

    ## Error

    Se activa cuando ocurre un error durante el proceso de ejecución de la función

    ## onFinish

    Se activa cuando todas las iteraciones finalizan

    ## Iteration

    Se activa en cada una de las iteraciones, las funciones que se encuentren dentro de este Callback se ejecutarán en cada una de las iteraciones.

=== "Entry Vars"

    ## end

    ![](../../../../gitbook/assets/image%20%28451%29.png)

    Permite establecer el limite de iteraciones

    ## interval

    ![](../../../../gitbook/assets/image%20%28454%29.png)

    Se refiere a la cantidad de números con que se harán los saltos numéricos para alcanzar el final de iteraciones, dependiendo de este numero será el numero de iteraciones entre en punto de inicio y el punto final de iteraciones

    ## start

    ![](../../../../gitbook/assets/image%20%28435%29.png)

    Permite establecer un punto de inicio ara comenzar las iteraciones, generando un rango numerico entre la Entry Vars Start y End
