---
description: Cómo leer códigos de barras PDF417 en tu app de Apphive y extraer sólo los datos que necesitas, como la dirección de un paquete.
---

# Lector de código de barras para código PDF417

Apphive puede leer códigos QR y códigos de barras con la cámara del teléfono. Para formatos densos como **PDF417** (el que suelen llevar las etiquetas de paquetería), la opción más confiable es un **lector de códigos de barras externo por Bluetooth**: entrega el contenido como texto y en tu app lo separas para quedarte sólo con los campos que te interesan.

## Por qué no conviene la cámara para PDF417

El formato PDF417 no es tan redundante como un QR. Según la luz y la calidad de la cámara, el teléfono puede tardar en reconocerlo: en una oficina funciona, pero en un almacén o en la calle con mala iluminación cuesta más trabajo.

Un lector (pistola) de códigos de barras conectado por Bluetooth al teléfono es mucho más preciso y escribe el contenido del código como una entrada de texto.

## Extraer sólo algunos datos del código

El contenido de un PDF417 suele venir como una sola cadena con campos separados por un carácter, por ejemplo `|`. Para quedarte sólo con algunos campos (dirección, ciudad, código postal):

1. Recibe el texto leído (del campo donde escribe el lector Bluetooth, o del callback de la función de lectura).
2. Pásalo por un **Global Formater** con la opción **split**, indicando el carácter por el que quieres dividir (en el ejemplo, `|`). La salida es un arreglo, por ejemplo `["V01~A01", "D01~L6Y5Z4", ...]`.
3. Toma sólo las posiciones que te interesan: la posición `0` es el primer elemento, la `1` el segundo, y así sucesivamente.
4. Une esos valores con la función **Concat** para armar la dirección completa.

Con el resultado puedes llenar una lista, guardarlo en la base de datos o usarlo para consultar la dirección en Google.

## Referencias

- [Barcode Read](../reference/funciones/phone-apis-e/barcode-read/README.md)
- [Global Formater](../reference/funciones/logic-e/global-formater/README.md)
- [Concat](../reference/funciones/logic-e/concat/README.md)
