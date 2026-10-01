---
description: Si Upload File sólo sube fotos y videos y falla con otros archivos, lee su salida en un Alert; suele pasar con archivos fuera de la memoria interna.
---

# Problema con Upload File

Si **Upload File** sube fotos y videos pero falla con otros archivos (PDF, documentos…), muestra en un **Alert** la salida de la función para leer el error exacto. Muchas veces el problema es que el archivo elegido **no está en la memoria interna del teléfono** o en una carpeta a la que la app no puede acceder: al elegirlo desde otra carpeta se sube sin problema.

## Cómo diagnosticarlo

1. Abre el selector de archivos con **Show file browser** y pasa el archivo elegido a **Upload File**.
2. En el callback de error de Upload File agrega un **Alert** que muestre directamente la salida de la función.
3. Prueba de nuevo con el mismo archivo y lee el mensaje.
4. Si el error indica que el archivo no existe, mueve el archivo a otra carpeta (por ejemplo, a la memoria interna) y vuelve a intentarlo.

## Preguntas frecuentes

**¿Puedo mostrar el nombre del archivo que se va a subir?**
No por ahora: **Show file browser** sólo devuelve la URL (la ubicación del archivo en el teléfono) y Upload File devuelve la dirección del archivo en la base de datos.

Consulta también [Upload file](../reference/funciones/base-de-datos-e/upload-file/README.md) y [Show file browser](../reference/funciones/phone-apis-e/show-file-browser/README.md).
