---
description: Create list of elements using data in the database data
---

# Add Collections To UI

The add collection to UI is a function in the [elements](./) functions which allows to create lists of elements and modify using the registers on the [database data.](../../base-de-datos/) 

![](../../../.gitbook/assets/captura-de-pantalla-2020-02-10-a-la-s-10.26.28.png)

### 📥 Entry vars <a id="entry-vars"></a>

* **Enable horizontal:** you can select to see you list in a horizontal way
* **List data:** select the output for retrieve the list.
* **List instructions.** 
* **Modify element:** open a modifier on elements in your list.
* **List reverse:** change the order of the elements on the list.
* **Scroll inverted:** change the direction of the scroll in the list.

### 👉 Example.  <a id="examples"></a>

![](../../../.gitbook/assets/ezgif.com-video-to-gif-10%20%281%29.gif)

#### Use the database element.

1. Activate the [get database data](../cloud-database/get-database-data.md) and open database path.
2. Add a collection "Driver list" 
3. Add fields "address, name, phone number, photo and plates"
4. Push the button view data 
5. Press the button Add to add a record to "Driver list".

#### Add a collection to UI.

1. Add a collection to UI in the callback of the get [database data](../../base-de-datos/) when data obtained.
2. Select the previous output get database data in the list data.
3. Click on the button [modify elements](modify-control.md).
4. Select a container with elements to modify.
5. Click on list data and select the element to modify.
6. Select a control property to change like text.
7. Open the list context and write the name of the element to show in the database.

![Reload the page to check the modified elements in your list.](../../../.gitbook/assets/ezgif.com-video-to-gif-12%20%281%29.gif)

