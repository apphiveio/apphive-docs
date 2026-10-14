---
description: "Error de compilación ANDROID_PACKAGE_NOT_IN_GOOGLE_SERVICES: el nombre de paquete de tu app no aparece como app de Android en tu proyecto de Firebase."
---

# El paquete de Android no está registrado en Firebase

**Error:** `ANDROID_PACKAGE_NOT_IN_GOOGLE_SERVICES` («Your Android package name is not registered in your Firebase project»).

Firebase genera una configuración por cada app de Android, identificada por su **nombre de paquete** (por ejemplo `com.miempresa.usuario`). Si al compilar no encuentra una app de Android con el paquete exacto de tu app, la compilación falla con este error.

Normalmente Apphive da de alta la app de Android en tu proyecto de Firebase automáticamente al compilar. Si aun así aparece este error, puedes registrarla tú:

1. En Apphive, copia el **nombre de paquete** de la app que falló (en la configuración de Android de la app).
2. Entra a [console.firebase.google.com](https://console.firebase.google.com/) y abre el proyecto de Firebase de tu app.
3. Da clic en el engrane ⚙️ > **Configuración del proyecto** > **Tus apps** > **Agregar app** > **Android**.
4. Pega el nombre de paquete **exactamente igual** (mayúsculas, puntos y sufijos incluidos) y registra la app. No hace falta que descargues el archivo `google-services.json`: Apphive lo obtiene solo al compilar.
5. Vuelve a lanzar la compilación.

!!! tip "Es por app"
    Si tu proyecto tiene varias apps (usuario, conductor, administrador), cada una necesita su propia app de Android en Firebase. Puede fallar una y compilar otra el mismo día.

Si el error continúa después de registrar el paquete, escríbenos desde el chat de soporte con el nombre de la app y la hora de la compilación.
