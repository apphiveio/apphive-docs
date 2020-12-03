# Callbacks

## Done

Se activa cuando todas las iteraciones concluyeron

## Error

Se activa cuando ocurre algún tipo de error durante el proceso de iteración de la información

## Iteration

Abren una ventana **onCompute** en donde generalmente se ejecuta algún tipo de lógica para completar cierta acción. Se agrega un nuevo componente onComputeCallback 

![](../../../../.gitbook/assets/image%20%28434%29.png)

Esta función sirve como indicador de que una iteración se terminado de ejecutar e indicar el inicio de la siguiente iteración o llamar el callback Done dependiendo del Modo que se haya seleccionado

El tiempo de ejecución de cada iteración depende directamente de las funciones que se integren en la lógica, puesto que algunas pueden llevar más tiempo que otras, esto es por que algunas funciones son asíncronas y no tenemos el control de cuanto tiempo se van a tardar para ejecutar su proceso



## Non iterable

Se activa cuando la información en la Entry Var **Collection** no se puede iterar



[Ver más](https://comunidad.apphive.io/t/importante-mejora-en-la-funcion-foreach-si-la-usas-deberas-leer-esto/2058)

