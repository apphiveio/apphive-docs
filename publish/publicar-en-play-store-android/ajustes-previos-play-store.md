---
description: >-
  ¿Estás listo para publicar tu App en Play Store? estos son los pasos previos
  que debes seguir
---

# 1. Ajustes previos a la compilación

{% hint style="success" %}
## **Cambiar Splas Screen**
{% endhint %}

1.-  Entra a tu proyecto en [https://editor.apphive.io/](https://editor.apphive.io/) 

![](../../.gitbook/assets/1.png)

2.- Selecciona una app

![](../../.gitbook/assets/2.png)

3.- Da clic en configuraciones y clic en configuraciones de la app que quieres modificar.

![](../../.gitbook/assets/3.jpeg)

4.- Da clic en configuración, en el menú de general selecciona splash screen y clic en el icono editar.

![](../../.gitbook/assets/4%20%281%29.png)

5.- En la sección subir archivo da clic en elegir archivo.

**La imagen del splash screen debe ser en formato PNG con un ancho de 640 Pixeles X 1136 Píxeles de Alto.**

![](../../.gitbook/assets/5%20%281%29.png)

{% hint style="success" %}
## **Obtener una suscripción Premium o Unlimited**
{% endhint %}

Sigue estos pasos para adquirir tu suscripción:

6.- Entra en el editor [https://editor.apphive.io ](https://editor.apphive.io/)y da clic sobre tu proyecto

![](../../.gitbook/assets/6%20%281%29.png)

7.- Da clic en suscripciones

![](../../.gitbook/assets/7%20%281%29.png)

 8.- Selecciona el plan de tu interés, para poder compilar. **Para sistema operativo Android y publicar en Play Store necesitas un plan Premium o Unlimited**

![](../../.gitbook/assets/8%20%281%29.png)

9.- Da clic sobre el recuadro de número de tarjeta

![](../../.gitbook/assets/9%20%281%29.png)

10.- Agrega los datos de tu tarjeta y clic en el botón Pay

![](../../.gitbook/assets/10%20%281%29.png)

{% hint style="success" %}
## Obtener cuenta de Firebase
{% endhint %}

 11.- Entra en [https://firebase.google.com/](https://firebase.google.com/) y da clic en comenzar.

![](../../.gitbook/assets/11.jpeg)

12.- Da clic en crear un proyecto.

![](../../.gitbook/assets/12.jpeg)

13.- Escribe el nombre de tu proyecto, clic en la casilla para aceptar las condiciones de Firebase y clic en continuar.

\***Puedes escribir el mismo nombre que le colocaste a tu proyecto en Apphive, este nombre solo servirá para que tu puedas identificar tu proyecto en Firebase.**

**MUY IMPORTANTE** Copia el nombre de tu proyecto en Firebase y pegalo en una nota o un documento de word de la siguiente manera:

NOMBRE PROYECTO FIREBASE: Uber eats plantillas

![](../../.gitbook/assets/13%20%281%29.png)

![](../../.gitbook/assets/14%20%281%29.png)

14.- Da clic en continuar

Puedes realizar los pasos de **Opcional activación de Google Analytics**\(este te permitirá tener estadísticas de comportamiento de tu base de datos y usuarios.\) o saltar al paso número 5 de Firebase

Opcional activación de Google Analytics 1: habilita Google Analytics

![](../../.gitbook/assets/15%20%281%29.png)

Opcional activación de Google Analytics 2: Selecciona o crea una cuenta

![](../../.gitbook/assets/16%20%281%29.png)

Opcional activación de Google Analytics 3: Escribe el nombre de tu proyecto y clic en guardar.

![](../../.gitbook/assets/17.png)

Opcional activación de Google Analytics 4: Selecciona tu país, clic en las 3 casillas de permisos y condiciones de servicio y clic en continuar.

![](../../.gitbook/assets/18.png)

15.- Esperar a que cree el proyecto y haga clic en continuar.

![](../../.gitbook/assets/19.png)

16.- Debes actualizar tu plan a Blaze para poder compilar, da clic en Actualizar y clic en Seleccionar plan.

![](../../.gitbook/assets/20.png)

17.- Da clic en Continuar.

![](../../.gitbook/assets/21.png)

18.- Verifica que tus datos sean correctos o da clic en el icono de editar y modifícalos

![](../../.gitbook/assets/22.png)

![](../../.gitbook/assets/23.png)

19.- Agrega el número de tarjeta de crédito o débito, la fecha de vencimiento, la clave de seguridad, el nombre del titular, verifica que la dirección antes agregada sea la misma de la tarjeta y da clic en Confirmar compra.

![](../../.gitbook/assets/24.png)

20.- Selecciona Functions y clic en comenzar

![](../../.gitbook/assets/25.jpeg)

21.- Da clic en continuar

![](../../.gitbook/assets/25.png)

22.- Da clic en finalizar

![](../../.gitbook/assets/26%20%281%29.png)

23.- Selecciona Realtime Database y clic en crear una base de datos.

![](../../.gitbook/assets/27.jpeg)

24.- Selecciona comenzar en modo bloqueado y da clic en habilitar.

![](../../.gitbook/assets/28.jpeg)

25.- **MUY IMPORTANTE** Copia la URL que tenga tu proyecto como se muestra en la siguiente imagen y pegala en una nota o un documento de word de la siguiente manera:

FIREBASE REALTIME DATABASE URL: [https://uber-eats-plantilla.firebaseio.com/](https://uber-eats-plantilla.firebaseio.com/)

![](../../.gitbook/assets/27.png)

26.- Da clic en Copias de seguridad y Empezar.

![](../../.gitbook/assets/28.png)

27.- Da clic en Continuar, Abre Opciones avanzadas, activa compresión, activa ciclo de vida de almacenamiento: 30 días y da clic en Guardar.

![](../../.gitbook/assets/29.jpeg)

![](../../.gitbook/assets/30.png)

28.- Selecciona Storage y clic en comenzar

![](../../.gitbook/assets/30.jpeg)

29.- Clic en siguiente, verifica que en ubicación este Nam5 \(us-central\) y clic en listo.

![](../../.gitbook/assets/31.jpeg)

![](../../.gitbook/assets/32.jpeg)

30.- **MUY IMPORTANTE** Copia el fragmento de URL de tu proyecto como se muestra en la siguiente imagen y pegala en una nota o un documento de word de la siguiente manera:

FIREBASE STORAGE URL: [uber-eats-plantilla.appspot.com](http://uber-eats-plantilla.appspot.com/)

![](../../.gitbook/assets/31.png)

31.- Da clic en configuraciones, configuración del proyecto y selecciona cuentas de servicio.

![](../../.gitbook/assets/33.jpeg)

![](../../.gitbook/assets/32.png)

32.- **MUY IMPORTANTE** Clic en Generar nueva clave privada y clic en Generar clave; esto descargara un archivo .json

Este archivo debes guardarlo en tu computadora, crea una carpeta con el nombre SERVICE ACCOUNT FILE y dentro de esta carpeta guardar este archivo .json

![](../../.gitbook/assets/33.png)

33.- Da clic en Authentication y selecciona Sign-in method.

![](../../.gitbook/assets/34.png)

Opcional: Si cualquiera de tus apps utiliza inicio de sesión con Gmail selecciona Google, da clic en Habilitar, selecciona tu dirección de correo electrónico DEBE AGREGAR LA MISMA CUENTA DE GMAIL CON LA QUE CREASTE LA FIREBASE y clic en Guardar.

![](../../.gitbook/assets/35.png)

34.- En la misma sección en la parte de abajo encontrarás Varias cuentas por dirección de correo electrónico da clic en Cambiar, selecciona Permite la creación de varias cuentas con la misma dirección de correo electrónico y da clic en Guardar.

![](../../.gitbook/assets/36.png)

{% hint style="success" %}
## Opcional Facebook for developers
{% endhint %}

