---
description: Cómo agregar tu app de Android a tu app de Facebook Developers con el nombre del paquete, MainActivity y el Release key hash.
---

# Añadir la app de Android a Facebook

Para que el inicio de sesión con Facebook funcione en tu app de Android, registra la plataforma Android en tu app de Facebook Developers con tres datos: el **nombre del paquete** de Android, la clase **MainActivity** y el **Release key hash**. El nombre del paquete y el key hash los copias desde Apphive.

## Pasos

1. Abre el panel de tu app en Facebook Developers (*Facebook app dashboard*).

    ![](img/a46e16a1e4a6.png)

2. Da clic en el ícono de **Android**.

    ![](img/b178f4f87c1a.png)

3. Da clic en **Siguiente**.

    ![](img/1413a1194ee1.png)

4. Da clic en **Siguiente** otra vez.

    ![](img/fb91e0d326aa.png)

5. Regresa a Apphive y da clic sobre el **Android package name** para copiarlo.

    ![](img/6883edf91b97.png)

6. En Facebook, pega el Android package name en **Nombre del paquete**. En el nombre de la clase escribe `MainActivity` (exactamente así, con las mismas mayúsculas y sin espacios) y da clic en **Save**.

    ![](img/ab4c74989bdf.png)

7. Da clic en **Usar el nombre de este paquete**.

    ![](img/3ccd81365e75.png)

8. Da clic en **Continuar**.

    ![](img/7566bc7d4be2.png)

9. Regresa a Apphive y da clic sobre el **Release key hash** para copiarlo.

    ![](img/9661b4a9590d.png)

10. En Facebook, pega el Release key hash en **Hashes de clave**, selecciona el hash (se marca en azul) y da clic en **Save**.

    ![](img/73989082610a.png)

11. Da clic en **Continuar**.

    ![](img/320058c5a575.png)

12. Activa el switch de **Inicio de sesión único**, da clic en **Save** y luego en **Siguiente**.

    ![](img/d2a2b3e9f350.png)

13. Regresa a Apphive y da clic en **I'm ready**.

    ![](img/79877e8dcf70.png)

!!! warning
    Escribe `MainActivity` tal cual. Un cambio de mayúsculas o un espacio extra hace que el inicio de sesión con Facebook falle.
