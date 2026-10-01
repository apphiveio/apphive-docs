---
description: Si Google Play pide orientar tu app a Android 15 (nivel 35 de la API), genera una nueva compilación en Apphive y sube el nuevo AAB.
---

# Google pide Android 15 (nivel 35 de la API): cómo solucionarlo

El aviso «Actualizar tu aplicación para orientarla a Android 15 (nivel 35 de la API) o versiones posteriores» significa que **la versión publicada en Google Play** se compiló para un nivel de API anterior al que Google exige. En Apphive no tienes que cambiar nada en el código: **genera una nueva compilación de Android y sube el nuevo archivo AAB a Google Play**. Las compilaciones nuevas ya cumplen el nivel de API que pide Google.

## Pasos

1. **Genera una nueva compilación de Android (Google Play)** desde el editor de Apphive.
2. **Descarga el archivo AAB** cuando termine la compilación. Si quieres probar antes, instala el APK en un teléfono con Android 15 o superior. Consulta [Descargar los archivos APK y AAB](descargar-archivos-apk-y-aab.md).
3. **Sube el AAB a Google Play Console** como una nueva versión. Google detecta el nuevo nivel de API y el aviso desaparece cuando esa versión se publica.

!!! note
    El aviso se refiere a la versión que está **publicada** en Google Play, no a la última que compilaste. Si ya compilaste recientemente, quizá no necesites compilar otra vez: basta con subir esa compilación.

## Si algo no funciona

Si después de compilar alguna función de tu app falla, escribe al chat de soporte de Apphive indicando qué parte específica falla.
