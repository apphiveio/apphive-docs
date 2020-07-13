---
description: Function to delete data from database
---

# Delete Database Data

The Delete database data is a function on the [Cloud Database](./) group, this function allows you to delete specific records on the database or the hole collection

![](../../../.gitbook/assets/captura-de-pantalla-2020-02-03-a-la-s-16.03.27.png)

### 📥 Entry vars

* **Database path to delete** 

{% hint style="danger" %}
If you don't set any specific data index all the data in the collection will be deleted
{% endhint %}

### ↗ Callbacks

* **Error deleting data.** This callback is called when for some reason it is not possible to delete the data from the database
* **Data deleted.** This is called once the database record \(s\) have been deleted successfully.

### 👉 Examples.

#### Deleting a full collection

In this example we deleted all the products in the database when the page loads

![](../../../.gitbook/assets/example-delete-database-data.gif)

#### Deleting a single record

To delete a single record you must have the id of the record you want to delete, in this example we have a product detail and you have the product id as a "Page context data"

![](../../../.gitbook/assets/delete-single-record.gif)

