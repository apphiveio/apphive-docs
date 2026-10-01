---
description: Paso a paso para crear tu API key de Google Maps en Google Cloud Console, habilitar las APIs necesarias y agregarla a tu app de Apphive.
---

# Paso a paso: cómo obtener tu API key de Google

Para que los mapas, el geocoding, la distancia de ruta y el autocompletado de direcciones funcionen en tu app, necesitas una **API key de Google**. Se crea en Google Cloud Console: activas la facturación, habilitas siete APIs de Google Maps, generas la clave y la pegas en tu app de Apphive.

## 1. Crea tu proyecto en Google Cloud

Entra a [Google Cloud Console](https://console.cloud.google.com/projectselector2/home/dashboard) y crea un proyecto nuevo. Llena estas opciones:

- País donde usarás la app (el país principal; de todos modos podrás operar en todos los países).
- Acepta los términos.
- Opcional: recibir el boletín de novedades.
- Da clic en **Aceptar y continuar**.

![](img/7d498d83a326.png)

## 2. Agrega una cuenta de facturación

1. Abre el menú lateral (si no está abierto) y da clic en **Facturación**.

    ![](img/e0133e2dc04d.png)

2. Da clic en **Agregar cuenta de facturación**.

    ![](img/e5847958b821.png)

3. Si ya tienes una cuenta de facturación, sólo selecciónala. Si no, crea una nueva: elige el país que corresponde a la tarjeta que vas a agregar, acepta las condiciones del servicio y da clic en **Continuar**.

    ![](img/cafdace844c0.png)

4. Llena los datos de la persona o empresa que realizará el pago.

    ![](img/2169c62710f2.png)

5. Agrega los datos de tu tarjeta bancaria. Es posible que veas un cargo pequeño que se cancela en unos minutos: sirve para validar la tarjeta. No se te cobra nada a menos que excedas la capa gratuita de Google.

    ![](img/62372c28652a.png)

6. Cuando la tarjeta sea aceptada, volverás a la página inicial.

    ![](img/7263177367c2.png)

## 3. Habilita las APIs

Debes habilitar **cada una** de estas APIs:

- Directions API
- Distance Matrix API
- Maps JavaScript API
- Maps SDK for Android
- Maps SDK for iOS
- Places API
- Geocoding API

![](img/c16e0415263d.png)

Repite estos pasos por cada API de la lista:

1. Da clic en **Biblioteca**.

    ![](img/01176cb707f6.png)

2. Escribe el nombre de la API que estás agregando.

    ![](img/b1bfd3615970.png)

3. Da clic en **Habilitar**. En la imagen se muestra el ejemplo con Maps SDK for Android.

    ![](img/0d210d50ce2c.png)

Al terminar con todas, da clic en **APIs** para ir a tu panel y verifica que estén todas habilitadas. Si falta alguna, repite los pasos.

![](img/d851c470caeb.png)

![](img/542fc804ff05.png)

## 4. Genera la API key

1. Da clic en **Credenciales**.

    ![](img/781f29b758b2.png)

2. Entra a [Credenciales, en la sección APIs y servicios](https://console.cloud.google.com/apis/credentials).

    ![](img/c8ce2f1581cb.png)

3. Da clic en **Crear credenciales**.

    ![](img/e041fc1558b2.png)

4. Selecciona **Clave de API**.

    ![](img/460387a5d056.png)

5. Copia la clave.

    ![](img/8d7150e1330b.png)

## 5. Agrégala a tu app en Apphive

1. Entra al [editor de Apphive](https://editor.apphive.io/), abre tu aplicación y da clic en su nombre para entrar a las configuraciones.

    ![](img/ce4c3351fef1.png)

2. Da clic en **Settings**.

    ![](img/4dfe918e28d1.png)

3. Da clic en **API Keys**.

    ![](img/6a6a881e6186.png)

4. Pega la clave que copiaste y da clic en guardar. **Hazlo en cada app de tu proyecto**; puedes usar la misma clave para todas.

    ![](img/e30a2d3471f6.png)

### En el asistente de compilación

Si el asistente de compilación te pide la Google Maps key, pega tu API key en el recuadro marcado y da clic en **I'm ready**.

![](img/542fbf703df7.png)

## 6. Restringe la clave (recomendado)

Después de publicar tu app, es buena práctica restringir la clave. Entra de nuevo a [Credenciales](https://console.cloud.google.com/apis/credentials) y da clic en la clave que quieres restringir.

![](img/7cc198a3dbab.png)

## Problemas comunes

- **Google rechaza mi tarjeta de débito.** Para validarla se hace un cobro momentáneo que luego se devuelve, así que la tarjeta necesita tener fondos. Si tiene fondos y aun así la rechaza, llama a tu banco y pide que habiliten los pagos digitales a Google Cloud; luego vuelve a intentarlo.
