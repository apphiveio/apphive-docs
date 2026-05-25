# forEach

![](../../../../gitbook/assets/image%20%28442%29.png)

La función forEach permite recorrer todos los elementos o registros de un arreglo o de un objeto

[Información general](https://docs.apphive.io/reference/funciones/informacion-general-de-las-funciones)



=== "Callbacks"

    ## Done

    Se activa cuando todas las iteraciones concluyeron

    ## Error

    Se activa cuando ocurre algún tipo de error durante el proceso de iteración de la información

    ## Iteration

    Abren una ventana **onCompute** en donde generalmente se ejecuta algún tipo de lógica para completar cierta acción. Se agrega un nuevo componente onComputeCallback 

    ![](../../../../gitbook/assets/image%20%28434%29.png)

    Esta función sirve como indicador de que una iteración se terminado de ejecutar e indicar el inicio de la siguiente iteración o llamar el callback Done dependiendo del Modo que se haya seleccionado

    El tiempo de ejecución de cada iteración depende directamente de las funciones que se integren en la lógica, puesto que algunas pueden llevar más tiempo que otras, esto es por que algunas funciones son asíncronas y no tenemos el control de cuanto tiempo se van a tardar para ejecutar su proceso



    ## Non iterable

    Se activa cuando la información en la Entry Var **Collection** no se puede iterar



    [Ver más](https://comunidad.apphive.io/t/importante-mejora-en-la-funcion-foreach-si-la-usas-deberas-leer-esto/2058)

=== "Entry Vars"

    ## Collection

    ![](../../../../gitbook/assets/image%20%28441%29.png)

    En esta sección se debe ingresar el conjunto de información que se requiere recorrer cada uno de sus valores o registros, puede ser un objeto o un arreglo los elementos de los que puede hacer lectura

    ## Mode

    ![](../../../../gitbook/assets/image%20%28439%29.png)

    Permite seleccionar el tipo de recorrido con el que se va a realizar la lectura de los registros y la ejecución de las funciones en cada una de las iteraciones 

    | Modo | Descripción | Representación grafica de lectura |
    | :--- | :--- | :--- |
    | async | Va a ejecutar todas las iteraciones al mismo tiempo | ![](../../../../gitbook/assets/image%20%28448%29.png)  |
    | default | Va a ejecutar las iteraciones sin tener un orden de ejecución | ![](../../../../gitbook/assets/image%20%28437%29.png)  |
    | sync | Va a ejecutar las iteraciones una después de la otra | ![](../../../../gitbook/assets/image%20%28461%29.png)  |
