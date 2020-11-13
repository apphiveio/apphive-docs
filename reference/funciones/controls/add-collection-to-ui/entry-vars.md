# Entry vars

## Enable Horizontal

Al activar el switch la función de lista se hará de forma horizontal

{% hint style="danger" %}
Cuando se activa este switch se debe tener especial cuidado con las dimensiones en ancho del elemento hijo y que no esté en porcentaje sino que se encuentre en pixeles
{% endhint %}

## List data

En esta opción se debe de ingresar un objeto que contenga los registros que se van a reflejar en el objeto hijo \(el componente que se va repetir en la lista\) puede ser directamente de un eventOutput de una función anterior generalmente se utiliza la función Get Database Data pero tambien se puede obtener de una variable local que contenga un objeto iterable para mostrar la grafica

![](../../../../.gitbook/assets/image%20%28338%29.png)



### List settings

Abre una ventana en donde muestra de edición de los controles dentro del contenedor padre solamente debe de haber un contenedor o elemento que será el editable

![](../../../../.gitbook/assets/image%20%28329%29.png)

#### Enable category tabs

Permite abrir una serie de pestañas para dar una lista de objetos por categorización, se elige por que campo se va a realizar la categorización

![](../../../../.gitbook/assets/image%20%28337%29.png)

Debe seguir un tipo especifico de estructura en la base de datos para poder realizar este tipo de lista

![](../../../../.gitbook/assets/image%20%28336%29.png)

Se debe poner el tipo de categoría por cada producto producto, si se pone solamente la categoría y en una collection los productos, este tipo de lista no se podrá realizar



#### Enable filter List

Permite sobreponer un componente extra de filtrado en la lista, esto quiere decir que nos da una barra de búsqueda nativa para poder hacer una búsqueda dinámica en la lista renderizada.

![](../../../../.gitbook/assets/image%20%28333%29.png)

**Filter property**

En este apartado se debe colocar alguno de los campos por el que se va a buscar dentro de la lista, este campo se debe escribir exactamente como se encuentra en la base de datos para que se pueda hacer la búsqueda

**Filter placeholder** 

Puedes poner la indicación de búsqueda en la barra, generalmente se indica que se busque por el mismo campo en que se hace el **Filter property**

#### **Order by**

Es una elemento en el que se indica por que campo de la base de datos se puede ordenar la lista, esta la ordenará en orden alfabético o colocarse la palabra **createAt** y con esto los elementos se ordenarán desde el nuevo registro ordenado hasta el registro mas antiguo

![](../../../../.gitbook/assets/image%20%28330%29.png)

#### Num. colums

![](../../../../.gitbook/assets/image%20%28334%29.png)

Al activar esta función permite crear una lista en especie de grid o mosaicos, solamente debemos de colocar el numero de columnas a mostrar en la lista.

#### Previewer de lista

Muestra una pre visualización del contenedor padre en donde se hará la iteración del objeto hijo

![](../../../../.gitbook/assets/image%20%28331%29.png)

### **List Data**

\*\*\*\*

### List item function

![](../../../../.gitbook/assets/image%20%28321%29.png)

Permite hacer selección de los controles a modificar mostrando sus respectivos eventos

[Información general](https://docs.apphive.io/reference/funciones/informacion-general-de-las-funciones)





List reverse



Scroll Inverted

