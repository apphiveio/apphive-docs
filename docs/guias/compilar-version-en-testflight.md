---
description: Para compilar tu app iOS en TestFlight crea una API Key en App Store Connect (Key ID, Issuer ID y archivo .p8) y crea el contenedor de tu app.
---

# Compilar versión en TestFlight

Para compilar tu app iOS y subirla a TestFlight, Apphive te pide los datos de una **API Key de App Store Connect**: el **Key ID**, el **Issuer ID** y el archivo **.p8**. Además, debe existir el **contenedor de tu app** en App Store Connect; mientras no exista, la compilación queda incompleta.

![](img/6816b25f51ae.png)

## 1. Crear la API Key en App Store Connect

1. Entra a [https://appstoreconnect.apple.com/](https://appstoreconnect.apple.com/).
2. Da clic en **Usuarios y accesos**.
   ![](img/4cd81588cba2.png)
3. Selecciona la pestaña **Keys** (o **Claves**, según tu idioma).
   ![](img/93e72d89faa3.png)
4. Verifica que estés en **App Store Connect API** y da clic en **Request Access**.
   ![](img/ae053dfaffe1.png)
5. Marca la casilla para aceptar compartir tus API Keys (así la compilación puede hacerse de forma automática) y da clic en **Enviar**.
   ![](img/ca96dfcd43db.png)
6. Da clic en **Generate API Key**.
   ![](img/a96c2c9fc6a9.png)
7. Ponle cualquier nombre y en **Access** selecciona **Admin**.
   ![](img/affd3836e8dc.png)
8. Da clic en **Generate**.
   ![](img/f67a0fda3e74.png)
9. Da clic en **Download API Key** y luego en **Download**. Se descarga un archivo **.p8**: guárdalo donde puedas encontrarlo fácilmente.
   ![](img/e331d5bd728b.png)
   ![](img/c5ee28405739.png)

## 2. Cargar la API Key en Apphive

1. Ya tienes los tres datos que pide la compilación: **Key ID**, **Issuer ID** y el **archivo .p8**.
   ![](img/6d3fa0ae57a6.png)
2. Copia el **Key ID** y el **Issuer ID** en el editor.
3. En **Custom api key name** escribe un nombre que te permita identificar la clave. Puede ser cualquiera; sirve para que, al compilar otros proyectos, no tengas que volver a cargar todos los campos.
4. Da clic en **Pick key file**, selecciona el archivo .p8 y da clic en **Abrir**.
   ![](img/12e149cf1683.png)
   ![](img/b83f6783f54d.png)
5. Da clic en **Continuar**.
   ![](img/1a2386b8035d.png)

Si todavía no existe el contenedor de tu app en App Store Connect, Apphive te avisará que debes crearlo.

![](img/1f233d7fddd6.png)

## 3. Crear el contenedor de la app en App Store Connect

1. Entra a [https://appstoreconnect.apple.com/](https://appstoreconnect.apple.com/) y da clic en **Mis Apps**.
   ![](img/a65b8b39f1ee.png)
2. Da clic en el botón **Agregar** y en **Nueva app**.
   ![](img/d87b27d9142e.jpeg)
3. Selecciona **iOS**, escribe el nombre de la app y elige su idioma principal.
   ![](img/55adc74afe5a.jpeg)
4. En **ID de pack** (Bundle ID) selecciona el **Compilation ID** de tu app, por ejemplo `io.apphive.clientapps.userapp`.
   ![](img/84817539d46d.jpeg)
5. Escribe el mismo Compilation ID en **SKU**, selecciona **Acceso ilimitado** y da clic en **Crear**.
   ![](img/6376ad904df2.jpeg)

## 4. Reanudar la compilación

Cuando el contenedor exista, si la compilación no cambia de estado da clic en **CANCEL INPUT** y elige la opción de recargar. En ese momento la compilación comienza.

Si tu app usa notificaciones push, configura también la clave de APNs en Firebase: [Crear key para habilitar Push Notification en Firebase](crear-key-para-habilitar-push-notification-en-firebase.md).
