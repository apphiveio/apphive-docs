---
description: >-
  La propiedad border-radius permite a los desarrolladores definir qué tan
  redondeadas serán las esquinas de su componente en cuestión.
---

# Border Radius

## Opciones de Border Radius

![](../../.gitbook/assets/image%20%2847%29.png)

Desde esta opción podemos elegir que tan redondeadas queremos que se vean las esquinas de nuestro componente. Se muestran 4 bordes marcado en 0 que son los valores por defecto de cada componente.

Los bordes redondeados toman el valor del border radius y desde las esquinas del componente van hacia abajo y a la derecha \(esquina superior izquierda\), hacia la izquierda y abajo \(esquina superior derecha\), hacia arriba y a la izquierda \(esquina inferior derecha\) y hacia arriba y a la derecha \(esquina inferior izquierda\). una vez recorridos los pixeles \(valor del border radius\) crean una curva para hacer los bordes redondeados.

| Descripción | **Borde** | **Escala** |
| :--- | :--- | :--- |
| Bordes con esquinas | ![](../../.gitbook/assets/image%20%2865%29.png)  | 0 |
| Bordes semi redondeados | ![](../../.gitbook/assets/image%20%2859%29.png)  | 25 |
| Borde completamente redondeado | ![](../../.gitbook/assets/image%20%2850%29.png)  | 68 |

Para que los bordes queden completamente redondeados, debemos asignar el valor equivalente a la mitad de la longitud de los lados  \(la imagen de la tabla anterior es de dimensiones 230 largo x 135 alto\). Dicho esto, dependiendo de las medidas del componente es como se le dará una apariencia ovalada, semi-ovalada o circular.

Todos los bordes que tengan el indicativo azul señalan que siempre tendrán el mismo valor de borde, por lo que si se quiere asignar valores distintos solo se tiene que dar click sobre el indicativo que se le quiera asignar un valor distinto a los demás. Así sus valores serán independientes de los otros valores.

![](../../.gitbook/assets/image%20%2868%29.png)

