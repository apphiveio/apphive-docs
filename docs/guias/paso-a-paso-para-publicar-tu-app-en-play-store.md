---
description: Paso a paso para publicar tu app de Apphive en Play Store - ajustes previos, compilar APK y AAB, crear la app en Play Console y ajustes posteriores.
---

# Paso a paso para publicar tu app en Play Store

Para publicar tu app en Google Play necesitas una suscripción de pago de Apphive, tu propio proyecto de Firebase y una cuenta de desarrollador de Google Play. El orden es: ajustes previos, compilar en Apphive (APK y AAB), crear y completar la ficha en Play Console y, al final, los ajustes posteriores a la publicación.

## Ajustes previos a la compilación

1. **Cambia la pantalla de inicio (splash screen)** de tu app. Consulta [Splash screen de tu aplicación](splash-screen-de-tu-aplicacion.md).
2. **Obtén una suscripción Premium o Unlimited.** Con el plan gratuito no puedes compilar. Consulta los planes en [apphive.io/es/precio](https://apphive.io/es/precio).
3. **Conecta tu propio proyecto de Firebase.** Mientras desarrollas usas el Firebase de Apphive; para compilar necesitas el tuyo. Consulta [Obtener Firebase](obtener-firebase.md).
4. **Facebook for developers (opcional).** Sólo si alguna de tus apps usa inicio de sesión con Facebook. Consulta [Facebook for Developers](opcional-facebook-for-developers-si-cualquiera-de-tus-apps-utiliza-inicio-de-sesion-con-facebook.md) e [Inicio de sesión con Facebook (SHA en APK)](inicio-de-sesion-con-facebook-sha-en-apk.md).

!!! note

    Cuando pegues la **Firebase storage URL** en la configuración de compilación, pégala sin el prefijo `gs://`.

## Compilación

1. Solicita el **APK** y el **AAB** desde Apphive.
2. Descarga los archivos APK y AAB cuando la compilación termine. Consulta [Descargar los archivos APK y AAB](descargar-archivos-apk-y-aab.md).

## Publicación

1. Crea tu cuenta de desarrollador: [Crear cuenta de desarrollador en Play Store](../publish/publish-to-play-store-android/crear-cuenta-de-desarrollador-en-play-store.md).
2. Prepara los [recursos gráficos que pide Google Play](recursos-graficos-para-cargar-tu-app-a-google-play.md).
3. Crea la app y completa su ficha en Play Console (pasos detallados abajo).

### Crear la app en Google Play Console

1. Entra a [https://play.google.com/console/about/](https://play.google.com/console/about/) y da clic en **Ir a Play Console**.
   ![](img/5b7fef34490d.png)
2. Da clic en **Crear aplicación**.
   ![](img/27dcb516b999.png)
3. Escribe el nombre de tu app, elige el idioma, marca **Aplicación** y elige **Gratis** (si no se cobra la descarga) o **De pago** (si quieres cobrar por descargarla).
   ![](img/b79f6dbdd13f.png)
4. Acepta las **Políticas del Programa para Desarrolladores** y las **Leyes de exportación de EE. UU.** y da clic en **Crear aplicación**.
   ![](img/cf034e4b8f60.png)
5. Da clic en **Ver tareas**.
   ![](img/a0061aaddbeb.png)

### Acceso a la aplicación

1. Selecciona **Acceso a las aplicaciones**.
   ![](img/c4b89ede3bcb.png)
2. Si tu app tiene inicio de sesión o registro, elige **Todas o algunas de las funciones están restringidas**. Si no, elige **Todas las funciones están disponibles sin acceso especial**.
   ![](img/24ee9285f7c8.png)
3. Escribe un nombre para el instructivo, el correo y la contraseña de un usuario de prueba y, en **Otras instrucciones**, explica con detalle cómo recorrer la app. Da clic en **Aplicar**.
   ![](img/a0d577669b26.png)

    !!! warning "Muy importante"

        Crea ese usuario en tu app antes de enviarla: los revisores de Google no se crearán una cuenta.

    Ejemplo de instrucciones:

    1. Da clic en **Iniciar sesión** e ingresa el correo y la contraseña de prueba.
    2. En la ventana de pedidos selecciona uno de los productos del catálogo.
    3. Marca las casillas para agregar adicionales.
    4. Da clic en **Comprar**.
    5. Selecciona la dirección de entrega.

4. Da clic en **Guardar**.
   ![](img/b97e51a685fe.png)

### Anuncios

1. Regresa con la opción **Panel de control**.
    ![](img/e569bf39909d.png)
2. Selecciona **Anuncios**.
    ![](img/9e4c97926378.png)
3. Si tu app no tiene publicidad, elige **No, mi aplicación no contiene anuncios** y da clic en **Guardar**.
    ![](img/40d6e6182412.png)

### Clasificación de contenido

1. Da clic en **Panel de control**.
    ![](img/f02f63d0864b.png)
2. Selecciona **Clasificación de contenido**.
    ![](img/b44c311c5fcd.png)
3. Da clic en **Empezar cuestionario**.
    ![](img/bd915277cf13.png)
4. Escribe tu correo electrónico.
    ![](img/34c50e1c4fcb.png)
5. Elige la categoría que corresponda al contenido de tu app y da clic en **Siguiente**.
    ![](img/99e17b80570c.png)
6. Marca las casillas según el contenido de tu app y da clic en **Guardar**.
    ![](img/828e0e859bd1.png)
    ![](img/97b23715c52d.png)
    ![](img/722317003eb4.png)
7. Da clic en **Siguiente**.
    ![](img/2d05fbd944a8.png)
8. Da clic en **Enviar**.
    ![](img/eea637a33725.jpg)

### Política de privacidad

1. Regresa a **Contenido de la aplicación**.
    ![](img/661b6df90526.png)
2. Da clic en **Empezar** en **Política de privacidad**.
    ![](img/1433d18b02bc.png)
3. Agrega la URL de la política de privacidad de tu empresa o app. Los requisitos cambian según tu país, así que infórmate en sitios especializados de tu país.
    ![](img/1fe19621e8bf.png)
4. Da clic en **Guardar** y vuelve a **Contenido de la aplicación**.
    ![](img/a7e8fd7d069e.png)

### Público objetivo

1. Da clic en **Empezar** en **Contenido y audiencia objetivo**.
    ![](img/8737298f0da3.png)
2. Selecciona la edad del público al que va dirigida tu app y da clic en **Siguiente**.
    ![](img/7413e5a6984d.png)

Completa el resto de las tareas que te pide Play Console hasta que todas aparezcan en verde, sube tu AAB y envía la versión a producción. Más detalles en [Carga tu app a Google Play](../publish/publish-to-play-store-android/carga-tu-app-a-google-play.md).

!!! note "¿Necesito una página web?"

    Necesitas al menos una URL pública para tu política de privacidad. Si no tienes sitio web, puedes crear una página gratis con [Google Sites](https://sites.google.com/new).

## Ajustes posteriores a la publicación

Al publicarse en Google Play, la firma de tu app cambia. Si tu app usa **inicio de sesión con Gmail o con Facebook**, debes registrar la nueva firma; sigue [Ajustes posteriores](../publish/publish-to-play-store-android/ajustes-posteriores.md).

Si quieres que tu app publicada tenga los datos y usuarios que creaste durante el desarrollo, cópialos a tu proyecto de Firebase.

## Ocultar o actualizar tu app

- Para retirar temporalmente tu app de la tienda consulta [Ocultar/Mostrar mi app en Google Play](ocultar-mostrar-mi-app-en-google-play-android.md).
- Para publicar una actualización, vuelve a compilar desde Apphive y sube el nuevo AAB a Play Console. Si Google Play te dice que el bundle está firmado con la clave incorrecta, consulta [Tu Android App Bundle está firmado con la clave incorrecta](tu-android-app-bundle-esta-firmado-con-la-clave-incorrecta.md).
