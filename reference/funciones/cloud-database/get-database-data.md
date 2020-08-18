---
description: Obtain registers from the cloud database data.
---

# Get Database Data

Agregar colección a la interfaz de usuario es una función en las funciones de [elementos](https://docs.apphive.io/reference/funciones/elements) que permite crear listas de elementos y modificar utilizando los registros en los datos de la [base de datos. ](https://docs.apphive.io/reference/funciones/elements/add-collections-to-ui)

![](../../../.gitbook/assets/captura-de-pantalla-2020-02-10-a-la-s-10.26.28.png)

### 📥 Entry vars  \(Variables de entrada\) <a id="entry-vars"></a>

* **Enable horizontal:** puede seleccionar para ver su lista de forma horizontal
* **List data:** seleccione la salida para recuperar la lista.
* **List instructions.** 
* **Modify element:** abre un modificador en los elementos de tu lista.
* **List reverse:** cambiar el orden de los elementos de la lista.
* **Scroll inverted:** cambiar la dirección del desplazamiento en la lista.

### 👉 Ejemplo.  <a id="examples"></a>

![](../../../.gitbook/assets/ezgif.com-video-to-gif-10%20%281%29.gif)

**Utilice el elemento de la base de datos**.

1. Active la obtención de datos de la base de datos \([get database data](get-database-data.md)\)

    y abra la ruta de la base de datos.

2. Agregar una colección "Lista de controladores" Agregue los campos "dirección, nombre, número de teléfono, foto y placas"
3. Presione el botón ver dato
4. Presione el botón Agregar para agregar un registro a la "Lista de controladores". \("Driver list"\).

#### Add a collection to UI. \(Agregar una colección a la interfaz de usuario\)

1. Agregue una colección a la interfaz de usuario en la devolución de llamada de obtener datos de la [base de datos](https://docs.apphive.io/reference/base-de-datos) cuando se obtengan los datos.
2. Seleccione la salida anterior para obtener datos de la base de datos en la lista de datos.
3. Haga clic en el botón modificar elementos. \([modify elements](../elements/modify-control.md)\).
4. Seleccione un contenedor con elementos para modificar.
5. Haga clic en los datos de la lista y seleccione el elemento a modificar.
6. Seleccione una propiedad de control para cambiarla como texto.
7. Abra el contexto de la lista y escriba el nombre del elemento para mostrar en la base de datos.

![Reload the page to check the modified elements in your list.](../../../.gitbook/assets/ezgif.com-video-to-gif-12%20%281%29.gif)

