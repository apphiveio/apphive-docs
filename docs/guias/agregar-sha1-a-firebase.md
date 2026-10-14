---
description: "Qué hacer cuando la compilación de Android se detiene en el paso «Agregar SHA1 a Firebase»: registrar la huella SHA-1 de tu app en tu proyecto de Firebase."
---

# Agregar la huella SHA-1 a Firebase

Al compilar para Android, Apphive registra automáticamente la huella **SHA-1** de tu app en tu proyecto de Firebase. Firebase la necesita, entre otras cosas, para que funcione el inicio de sesión con Google.

Si no pudimos registrarla nosotros (por ejemplo, por los permisos de tu proyecto de Firebase), la compilación se detiene en el paso **🔏 Agregar SHA1 a Firebase** y te muestra la huella que debes registrar.

## Cómo registrarla

1. En Apphive, abre el paso **Agregar SHA1 a Firebase** de tu compilación y copia la huella SHA-1 que aparece.
2. Entra a [console.firebase.google.com](https://console.firebase.google.com/) y abre el proyecto de Firebase de tu app.
3. Da clic en el engrane ⚙️ > **Configuración del proyecto** y, en la pestaña **General**, baja hasta **Tus apps**.
4. Elige la app de **Android** cuyo nombre de paquete coincide con el de tu app en Apphive.
5. Da clic en **Agregar huella digital**, pega la SHA-1 y guarda.
6. Regresa a Apphive y continúa la compilación.

!!! tip "Si ya estaba registrada y el inicio de sesión con Google falla"
    A veces Firebase guarda la huella pero no termina de crear su configuración interna. Bórrala y vuelve a agregarla en la misma app de Android. Eso obliga a Firebase a regenerarla.

!!! warning "Una huella por app"
    Cada app (pasajero, conductor, administrador…) tiene su propio paquete y su propia huella. Regístrala en la app de Android que corresponde, no en otra del mismo proyecto.
