---
description: This function send an email to the user email address to recover his password.
---

# Forget Password

The forget password is a function in the [users](./) functions which allows to the users change their password by sending a email to the user email, this function is important to the users to secure their account.

![](../../../.gitbook/assets/captura-de-pantalla-2020-02-10-a-la-s-10.34.27.png)

### 📥 Entry vars <a id="entry-vars"></a>

* **Email:** select a the text field to provide a way for the user to set his email address.

### ↗ Callbacks <a id="entry-vars"></a>

* **Email not sent:** you can set functions after the app can't send the email.
* **Email sent:** you can set functions after the app send the email.

### 👉 Example. 

![](../../../.gitbook/assets/ezgif.com-video-to-gif-16.gif)

#### Forget password

1. Add a forget password in the button.
2. Select an element to fill with a email.
3. Add a [send alert](../notifications/send-alert.md) if the email was send correctly. 

![The user will recibe a email to change his password](../../../.gitbook/assets/ezgif.com-video-to-gif-17%20%282%29.gif)

