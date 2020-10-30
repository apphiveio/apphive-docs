# Data

## Text field basic data

![](../../../.gitbook/assets/image%20%28149%29.png)

Al habilitar esta función se abre una nueva tap de Data llamada **Data Picker Option**

![](../../../.gitbook/assets/image%20%28153%29.png)

{% hint style="danger" %}
Cuando se activa esta función el control **Field** no tendrá eventos para seleccionar
{% endhint %}

### **Data Picker Option**

#### **Control name**

![](../../../.gitbook/assets/image%20%28156%29.png)

Permite cambiar el nombre del control [ver más](https://docs.apphive.io/global-functions/data/control-name)

#### Disable date picker

![](../../../.gitbook/assets/image%20%28142%29.png)

Funciona para activar o desactivar la tap **Data Picker Option**

#### **Mode date**

![](../../../.gitbook/assets/image%20%28154%29.png)

Esta función se maneja en conjunto con la función **Date format** ya que al elegir un modo de fecha, la tipografía de **Date format** cambia con respecto al modo elegido.

Se pueden elegir 3 tipos de modos de fecha

1. Date \(Fecha\)
2. Date Time \(Fecha y Hora\)
3. Time \(Hora\)

#### Enable dynamic loading

![](../../../.gitbook/assets/image%20%28151%29.png)

Funciona para dar apariencia de cargado al elemento [ver más](https://docs.apphive.io/global-functions/data/enable-dynamic-loading)

#### Date format

![](../../../.gitbook/assets/image%20%28152%29.png)

Muestra el tipo de formato de fecha, dependiendo este mismo del elegido por el **Mode date** 

| Mode Date | Date Format |
| :---: | :---: |
| Date | ![](../../../.gitbook/assets/image%20%28148%29.png)  |
| Date Time | ![](../../../.gitbook/assets/image%20%28160%29.png)  |
| Time | ![](../../../.gitbook/assets/image%20%28158%29.png)  |

Eventualmente este tipo de formato puede ser editado por el que el usuario prefiera o necesite

Al presionar el field \(ya renderizado\) mostrará unas ventanas emergentes para mostrar y editar la fecha o la hora, dependiendo del **Mode Date**

| **Mode Date** | Ventaja emergente |
| :---: | :---: |
| Date / Date Time | ![](../../../.gitbook/assets/screenshot_20201029-151452.png)  |
| Time | ![](../../../.gitbook/assets/screenshot_20201029-151657.png)  |

### Control name

![](../../../.gitbook/assets/image%20%28147%29.png)

Sirve para cambiar el nombre al control [ver más](https://docs.apphive.io/global-functions/data/control-name)

### Control placeholder

![](../../../.gitbook/assets/image%20%28141%29.png)

 El atributo placeholder funciona para representar una indicación que ayude al usuario a completar estos campos

### Keyboard type

![](../../../.gitbook/assets/image%20%28143%29.png)

 Permite seleccionar el tipo de teclado que se mostrará en el Panel de control. 

### Keyboard return key type

Cambia la tipografía de la tecla intro

![](../../../.gitbook/assets/image%20%28145%29.png)

### Enable blur on submit

![](../../../.gitbook/assets/image%20%28161%29.png)

### Control is hidden

![](../../../.gitbook/assets/image%20%28150%29.png)

Oculta los controles cuando se activa [ver más](https://docs.apphive.io/global-functions/data/control-is-hidden)

### Disabled

![](../../../.gitbook/assets/image%20%28162%29.png)

Cuando se activa deshabilita la capacidad de editar el field

## Text field advanced data

### Type password

![](../../../.gitbook/assets/image%20%28163%29.png)

Representa un campo para contraseñas, su valor es ocultado \(generalmente, reemplazando sus caracteres con un símbolo carente de significado\) y no se les permite a los usuarios copiarlo al portapapeles. Esto actúa como una medida de seguridad que previene que el valor sea conocido por cualquier persona que no sea el usuario.

### Multiples lines

![](../../../.gitbook/assets/image%20%28164%29.png)

Este elemento nos permite agregar múltiples líneas en el field y dar la apariencia de parrado, de esta manera se evita que el texto agregado no siga su recorrido continuo en una sola linea.

### Input mask

![](../../../.gitbook/assets/image%20%28175%29.png)

Permite agregar una estructura al texto ingresado.

Se puede agregar una estructura solamente de números, letras, alfanumérico o aceptar cualquier texto excepto espacios, si no se tiene nada ingresado en la casilla de input mask se permite ingresar cualquier tipo de texto sin discriminación a dígitos. 

## Places autocomplete

### Enable places autocomplete

![](../../../.gitbook/assets/image%20%28166%29.png)

Al activar este switch se activan nuevos elementos de manipulación, estos nuevos elementos se utilizan generalmente para poder autocompletar direcciones geográficas, como direcciones de calles, ciudades, etc.

![](../../../.gitbook/assets/image%20%28165%29.png)

{% hint style="warning" %}
Solo se podrán visualizar en el render \(aplicación Apphive Previewer\) si se tiene integrada una key de la API Google
{% endhint %}

![](../../../.gitbook/assets/image%20%28167%29.png)

Al seleccionar algunos de estos campos \(Geocode, Address, Regions, Cities, Establishment\) podrá mostrar las diferentes direcciones o establecimientos que coincidan con el texto ingresado en el field

#### Search countries places autocomplete:

![](../../../.gitbook/assets/image%20%28174%29.png)

Este elemento nos permite seleccionar los diferentes paises que existen en el mundo, de esta manera las direcciones que aparezcan como sugerencia, serán las que se encuentren en el pais que se eligió.

### Enable Multiline

![](../../../.gitbook/assets/image%20%28170%29.png)

Permite activar líneas múltiples

### Near Location

![](../../../.gitbook/assets/image%20%28168%29.png)

Permite tener una ubicación cerca de un ponto geográfico, solo basta con colocar la latitud y longitud del la ubicación

## Button icon

### Button icon

Permite agregar un icono en el field [ver más](https://docs.apphive.io/global-functions/data/icon)

### Direction

Permite manipular la dirección del icono con respecto al texto [ver más](https://docs.apphive.io/global-functions/estilos/direction)

