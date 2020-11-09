# Data

## Graphic config

### Type graphic

![](../../../.gitbook/assets/image%20%28306%29.png)

Permite seleccionar la apariencia de nuestra grafica hasta en 5 modelos distintos:

![](../../../.gitbook/assets/image%20%28305%29.png)

| Tipo de grafica | Vista previa |
| :---: | :---: |
| Line Chart | ![](../../../.gitbook/assets/image%20%28308%29.png)  |
| Bezier Chart | ![](../../../.gitbook/assets/image%20%28298%29.png)  |
| Bar Chart | ![](../../../.gitbook/assets/image%20%28301%29.png)  |
| Progress Chart | ![](../../../.gitbook/assets/image%20%28304%29.png)  |
| Pie Chart | ![](../../../.gitbook/assets/image%20%28295%29.png)  |

### Labels

![](../../../.gitbook/assets/image%20%28302%29.png)

En esta propiedad podemos agregar etiquetas identificadoras de los valores cuantitativos de forma estática 

Las etiquetas son colocados con interlineado después de ingresar una etiqueta

![](../../../.gitbook/assets/image%20%28303%29.png)

{% hint style="info" %}
La posición de las etiquetan dependen directamente del tipo de grafica que se elije

En la parte inferior en las siguientes graficas

1. Line Chart
2. Bezier Chart
3. Bar Chart

En la parte lateral derecha en las siguientes graficas

1. Progress Chart
2. Pie Chart
{% endhint %}

### Data

![](../../../.gitbook/assets/image%20%28297%29.png)

Permite agregar la información cuantitativa que se desea graficar de forma estática

Los valores son colocados con interlineado después de ingresar un valor

![](../../../.gitbook/assets/image%20%28300%29.png)

{% hint style="warning" %}
El numero de valores debe coincidir con el numero de etiquetas agregadas
{% endhint %}

### Colors

![](../../../.gitbook/assets/image%20%28296%29.png)

Esta propiedad permite agregar colores a los segmentos de la grafica Pie Chart, el numero de colores debe ser equivalente al numero de datos que se van a mostrar en la grafica 

Los valores son colocados con interlineado después de ingresar un valor

![](../../../.gitbook/assets/image%20%28299%29.png)

{% hint style="warning" %}
El nombre de los colores se debe de ingresar en ingles 
{% endhint %}

{% hint style="danger" %}
Esta propiedad **Colors** solamente está disponible para la grafica de Pie Chart
{% endhint %}

### Enable dynamic loading

![](../../../.gitbook/assets/image%20%28151%29.png)

Funciona para dar apariencia de cargado al elemento [ver más](https://docs.apphive.io/global-functions/data/enable-dynamic-loading)

### Control is hidden

![](../../../.gitbook/assets/image%20%28150%29.png)

Oculta los controles cuando se activa [ver más](https://docs.apphive.io/global-functions/data/control-is-hidden)

### Prop value

![](../../../.gitbook/assets/image%20%28294%29.png)

Con esta propiedad podemos elegir de forma estática el nombre del campo dentro de la base de datos de donde se sacarán de forma dinámica los valores que se van a graficar 

### Prop label

![](../../../.gitbook/assets/image%20%28309%29.png)

Con esta propiedad podemos elegir de forma estática el nombre del campo dentro de la base de datos de donde se sacarán de forma dinámica las etiquetas que se van a graficar 

{% hint style="info" %}
Estas dos propiedades solamente funcionarán cuando se ingrese información de forma dinámica o de una base de datos
{% endhint %}

