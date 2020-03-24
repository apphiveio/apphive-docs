---
description: Usually used to verify if the user is logged and access in the app.
---

# Is Logged In?

The is logged in? is a function in the users functions which allows to the app and admin if that user is actually logged to have access to data associated with that user and his private content.

![](../../../.gitbook/assets/captura-de-pantalla-2020-02-10-a-la-s-10.40.34.png)



### ↗ Callbacks <a id="entry-vars"></a>

* **User is logged in:** you can set functions or say which screen should be accessible if user is logged.
* **User is not logged in:** you can set functions or say which screen should be accessible if user isn't logged.

### 📤 Out vars <a id="entry-vars"></a>

* **ID current user:** select the specific user ID to get if his is logged or not.

### 👉 Example.  <a id="examples"></a>

![](../../../.gitbook/assets/ezgif.com-video-to-gif-3.gif)

1. Open splash screen and add an on load.
2. Add an is logged in? function.
3. Activate a [replace screen](../navigation/replace-screen.md) to the home if the user is logged in.
4. Activate a [replace screen](../navigation/replace-screen.md) to the register page if the user is not logged in or he [logout](logout.md) from the app.

![](../../../.gitbook/assets/ezgif.com-video-to-gif-15%20%281%29.gif)

{% hint style="info" %}
If the fist page of the app is a splash screen the app will check if the user previously login or not. 
{% endhint %}

