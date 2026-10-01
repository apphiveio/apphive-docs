---
description: Para que lleguen las notificaciones push en iOS crea una Key de APNs (.p8) en tu cuenta de Apple Developer y súbela a Cloud Messaging en Firebase.
---

# Crear key para habilitar Push Notification en Firebase

Si tu app iOS envía notificaciones push, necesitas crear una **Key de Apple Push Notification (archivo .p8)** en tu cuenta de Apple Developer y subirla a **Firebase > Configuración del proyecto > Cloud Messaging** junto con su **Key ID** y tu **Team ID**. Sólo necesitas **un archivo .p8 para todas las apps del proyecto**.

## 1. Crear la Key en Apple Developer

1. Entra a [Certificates, Identifiers & Profiles](https://developer.apple.com/account/resources/identifiers/list/bundleId), selecciona **Keys** y da clic en el icono para agregar.
   ![](img/1dc5442a5556.jpeg)
2. Como nombre de la Key escribe el **Compilation ID** de tu app sin puntos. Ejemplo: `ioapphiveclientappsuserapp`.
   ![](img/1d7f33fbb25e.jpeg)
3. Selecciona **Apple Push Notification** (sólo si alguna de tus apps envía push) y **Sign in with Apple** (sólo si alguna de tus apps tiene inicio de sesión con Gmail o Facebook). Da clic en **Configure**.
   ![](img/6006990e3353.jpeg)
4. Selecciona el **Compilation ID** de tu app y da clic en **Save**.
   ![](img/9d01b2859fcb.jpeg)
5. Da clic en **Continue** y luego en **Register**.
   ![](img/d53b6f53f522.jpeg)
   ![](img/e11b95c75a59.jpeg)
6. Da clic en **Download** para descargar el archivo **.p8**. Guárdalo en una carpeta que puedas identificar (por ejemplo, `KEY`); lo vas a necesitar en Firebase.
   ![](img/6f4db12332da.jpeg)

!!! note

    Si ninguna de tus apps usa push ni inicio de sesión con Gmail o Facebook, no necesitas esta Key: continúa con la creación del contenedor de la app en App Store Connect.

## 2. Subir la Key a Firebase

1. Entra a la [consola de Firebase](https://console.firebase.google.com/) y selecciona tu proyecto.
   ![](img/de524ecb258d.jpeg)
   ![](img/c559b525f376.jpeg)
2. Da clic en el engrane y en **Configuración del proyecto**.
   ![](img/317e77b075f5.jpeg)
3. Abre la pestaña **Cloud Messaging**.
   ![](img/c6a202ecd110.jpeg)
4. Selecciona la app con el símbolo de iOS que usa push o inicio de sesión con Facebook.
   ![](img/41ae47831f5e.jpeg)
5. Da clic en **Subir**, luego en **Examinar**, elige el archivo **.p8** y da clic en **Abrir**.
   ![](img/7bdf7b51c80f.jpeg)
   ![](img/eec6254c880a.jpeg)
   ![](img/2f782d6b1271.jpeg)
6. Para obtener el Key ID, abre [Keys en Certificates, Identifiers & Profiles](https://developer.apple.com/account/resources/certificates/list) y selecciona la Key con el Compilation ID de tu app.
   ![](img/db44a6d594ec.png)
   ![](img/0c8124a1805b.png)
7. Copia el **Key ID** y pégalo en el recuadro **ID de clave** de Firebase.
   ![](img/a4849d9c86ee.jpeg)
   ![](img/b21c5d252dff.jpeg)
8. Copia tu **Team ID** y pégalo en el recuadro **ID de equipo**.
   ![](img/d82773f4504e.jpeg)
   ![](img/51ce87874ca6.jpeg)
9. Da clic en **Subir**.
   ![](img/8380b6193cf9.jpeg)

Con esto, las notificaciones push funcionarán en tu app iOS.
