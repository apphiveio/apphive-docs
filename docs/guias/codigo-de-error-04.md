---
description: El código de error 04 al compilar se debe al Service Account usado; elimina los Service Account de tu Google Cloud, crea uno nuevo y vuelve a compilar.
---

# Código de error: 04

El código de error 04 aparece por un problema con el **Service Account** que se usó en la compilación. Apphive elimina automáticamente el Service Account anterior para que puedas cargar uno nuevo: borra los que tengas en tu Google Cloud, crea uno nuevo, cárgalo y vuelve a compilar.

## Cómo resolverlo

1. Elimina los Service Account que tengas creados en tu **Google Cloud**. En este video se muestra cómo hacerlo: [ver video](https://www.loom.com/share/6086831de7344bc497013cb632e2be0b).
2. Crea un **nuevo Service Account**. Consulta [Obtener el service account file](obtener-service-account-file.md).
3. Cárgalo en Apphive y manda a compilar de nuevo.

Si la compilación termina con éxito, el problema quedó resuelto.

## Si el error continúa

Si vuelve a fallar o tienes problemas al eliminar las claves, escribe a soporte desde el chat del editor (abajo a la derecha) con esta información:

1. Tu correo electrónico de contacto.
2. La URL de la app con error.
3. El código de error que recibiste por correo (incluye una captura del correo).
4. Lo que ya intentaste antes de escribir.
