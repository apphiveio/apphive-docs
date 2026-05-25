# Switch

![](../../../../gitbook/assets/image%20%28606%29.png)

La función Switch es un tipo de mecanismo de control de selección utilizado para permitir que el valor de una variable o expresión cambie el flujo de control de la ejecución de la lógica de la aplicación.

Se podría tomar como un conjunto de condiciones if \(==\)

[Información general](https://docs.apphive.io/reference/funciones/informacion-general-de-las-funciones) 



=== "Callbacks"

    ## Default

    Se activa cuando el valor de la variable no coincide con ninguno de los casos establecidos por el usuario

    ## Callbacks dinamicos

    Estos Callbacks dependen directamente del numero de casos que se agreguen en las entry vars, cada uno de ellos tendrá el mismo nombre de cada caso agregado.

    Y el modo de activación de cada callback depende de que el valor de la variable coincida \(sea igual\) con los casos agregados

    ![](../../../../gitbook/assets/image%20%28579%29.png)

=== "Entry Vars"

    ## Cases

    ![](../../../../gitbook/assets/image%20%28619%29.png)

    Permite agregar un numero finito de casos, el valor que se introduzca será el valor con el que se hará la comparación de la variable en la entry var **Value** y se mostrará, debajo de esta entry var

    ![](../../../../gitbook/assets/image%20%28582%29.png)

    ## Value

    ![](../../../../gitbook/assets/image%20%28623%29.png)

    Permite agregar una variable o control para poder hacer comparación de su valor con los casos agregados por el usuario
