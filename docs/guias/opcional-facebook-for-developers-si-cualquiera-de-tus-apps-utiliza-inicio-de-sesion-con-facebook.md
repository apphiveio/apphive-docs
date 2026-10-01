---
description: Crea tu app en Facebook for Developers, obtén el Facebook App ID y la clave secreta, y actívalos en Firebase y en tu compilación de Apphive.
---

# Facebook for Developers: obtener el Facebook App ID (si tus apps usan inicio de sesión con Facebook)

Este paso sólo es necesario si alguna de tus apps usa inicio de sesión con Facebook. Tienes que crear una app en Facebook for Developers, copiar su **identificador de la app** (Facebook App ID) y su **clave secreta**, habilitar Facebook como método de acceso en Firebase y pegar esos dos datos al compilar tu app en Apphive.

## 1. Crear la app en Facebook for Developers

1. Entra a [https://developers.facebook.com/](https://developers.facebook.com/) y haz clic en **Iniciar sesión**.

    ![](img/b3516bd41b4f.jpeg)

2. Inicia sesión con tu usuario y contraseña de Facebook.

    ![](img/949bf19895a0.png)

3. Haz clic en **Mis apps**.

    ![](img/6fd5c88288a5.jpeg)

4. Haz clic en **Crear app** y selecciona la opción **Para todo lo demás**. Si no aparece, selecciona **Crear experiencias conectadas**.

    ![](img/875c63fb336b.png)

5. En **Nombre para mostrar de la app** escribe el mismo nombre de tu proyecto de Firebase, y como correo usa el mismo con el que creaste tu proyecto de Firebase (ahí te avisarán si hay algún problema con tu app de Facebook). Haz clic en **Crear identificador de la app**.

    ![](img/77cb34f888d5.png)

6. Marca la casilla **No soy un robot** y haz clic en **Enviar**.

    ![](img/1b3f66e0b9df.png)

## 2. Copiar el Facebook App ID y la clave secreta

1. Copia el **Identificador de la app** y guárdalo en una nota, por ejemplo:

    ```
    FACEBOOK APP ID: <tu identificador>
    ```

2. Haz clic en **Configuración** y selecciona **Básica**.

    ![](img/29d970295a84.png)

3. Junto a la **Clave secreta de la app**, haz clic en **Mostrar** y escribe la contraseña de tu cuenta de Facebook.

    ![](img/8e81b0ce5fa1.png)

4. Copia la clave secreta y guárdala en la misma nota:

    ```
    FACEBOOK SECRET KEY: <tu clave secreta>
    ```

    ![](img/34a9433362fd.png)

!!! warning
    La clave secreta es privada: no la compartas ni la publiques.

## 3. Habilitar Facebook en Firebase

1. Abre [Firebase](https://firebase.google.com/) y haz clic en **Ir a la consola**.

    ![](img/120a1a38629a.jpeg)

2. Haz clic en tu proyecto de Firebase.

    ![](img/dd0cf86d0869.png)

3. Selecciona **Authentication** y haz clic en **Sign-in method**.

    ![](img/435e4593742c.png)

4. Selecciona **Facebook** y haz clic en **Habilitar**. Pega el Facebook App ID en **App ID** y la clave secreta en **App Secret**. Haz clic en **Guardar**.

    ![](img/86821dfd7de0.png)

    ![](img/2038972f5f84.png)

    ![](img/9ccd5d577941.png)

## 4. Agregar los datos en la compilación de Apphive

Cuando compiles tu app, Apphive te pedirá estos dos datos:

1. Pega el identificador de la app en **Facebook app ID** y la clave secreta en **Facebook app secret key**.
2. Haz clic en **Set Facebook app ID**.

![](img/30fda790b739.png)

## Si tienes más de una app con inicio de sesión con Facebook

Si varias apps de tu proyecto usan inicio de sesión con Facebook y cada una tiene un nombre de paquete distinto, en **Configuración** > **Básica**, al final de la página, agrega la clave de cada app en el mismo campo donde pegaste la primera.

![](img/39b0aa1e7a1d.png)

![](img/489c36bc523d.png)

Más detalles en [Inicio de sesión con Facebook: SHA en APK](inicio-de-sesion-con-facebook-sha-en-apk.md).

Para el proceso completo de publicación, consulta [Publicar en Play Store](../publish/publish-to-play-store-android/README.md).
