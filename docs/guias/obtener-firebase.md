---
description: "Crea tu proyecto de Firebase para compilar tu app de Apphive: plan Blaze, Functions, Realtime Database, Storage y cuenta de servicio."
---

# Obtener Firebase: crear el proyecto de Firebase de tu app

Para compilar tu app necesitas tu propio proyecto de Firebase en plan **Blaze**, con Functions, Realtime Database y Storage activados. Durante el proceso anota tres datos que te pedirá la compilación: el **nombre del proyecto**, la **URL de Realtime Database** y la **URL de Storage**.

## 1. Crea el proyecto

1. Entra a [firebase.google.com](https://firebase.google.com/) y da clic en **Comenzar**.

    ![](img/4298b1d22e17.jpeg)

2. Da clic en **Crear un proyecto**.

    ![](img/9462eedf4695.jpeg)

3. Escribe el nombre del proyecto (puede ser el mismo de tu proyecto en Apphive; solo sirve para que lo identifiques), acepta las condiciones de Firebase y da clic en **Continuar**.

    ![](img/77a1eb63b297.png)

    !!! tip "Anótalo"
        Copia el nombre del proyecto de Firebase en una nota: `NOMBRE PROYECTO FIREBASE: ...`

4. Google Analytics es opcional (te da estadísticas de uso de tu base de datos y tus usuarios). Si lo activas, selecciona o crea una cuenta, elige tu país y acepta las condiciones.

    ![](img/dab205541cd5.png)

5. Espera a que se cree el proyecto y da clic en **Continuar**.

    ![](img/80c7fe0ee93f.png)

## 2. Cambia al plan Blaze

Para poder compilar, el proyecto debe estar en plan Blaze. Da clic en **Actualizar > Seleccionar plan**, revisa tus datos y agrega una tarjeta de crédito o débito. Detalle en [Actualización de Firebase a plan Blaze](importante-actualizacion-de-google-firebase-de-plan-free-a-plan-blaze.md).

![](img/32da883d9e8f.jpg)

## 3. Activa Functions

Entra a **Functions**, da clic en **Comenzar**, luego en **Continuar** y en **Finalizar**.

![](img/20296bf674a1.jpeg)

## 4. Crea la Realtime Database

1. Entra a **Realtime Database** y da clic en **Crear una base de datos**.

    ![](img/b61803ce878f.jpeg)

2. Selecciona **Comenzar en modo bloqueado** y da clic en **Habilitar**.

    ![](img/c3f10ecbb012.jpeg)

3. Copia la URL de la base de datos y anótala: `FIREBASE REALTIME DATABASE URL: https://...firebaseio.com/` (ver [Obtener la URL de Firebase Realtime Database](obtener-firebase-realtime-database-url.md)).

    ![](img/2aff1021d390.png)

4. Opcional: en **Copias de seguridad**, da clic en **Empezar**; en **Opciones avanzadas** activa la compresión y el ciclo de vida de almacenamiento de 30 días, y guarda.

    ![](img/1c6dc74873cd.jpeg)

## 5. Activa Storage

1. Entra a **Storage** y da clic en **Comenzar**.

    ![](img/ce5fd976654a.jpeg)

2. Da clic en **Siguiente**, verifica que la ubicación sea **nam5 (us-central)** y da clic en **Listo**.

    ![](img/4f5e1d95bd3d.jpeg)

3. Copia el fragmento de la URL de Storage que se marca en la imagen y anótalo: `FIREBASE STORAGE URL: tu-proyecto.appspot.com`.

    ![](img/d057edc581ee.png)

## 6. Genera la cuenta de servicio

En **Configuración del proyecto > Cuentas de servicio**, da clic en **Generar nueva clave privada** y luego en **Generar clave**. Se descargará un archivo `.json`: guárdalo en una carpeta de tu computadora. Detalle en [Obtener el service account file](obtener-service-account-file.md).

![](img/5fee222facd8.jpg)
