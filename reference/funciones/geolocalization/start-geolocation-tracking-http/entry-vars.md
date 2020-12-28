# Entry Vars

## Desired accuracy

![](../../../../.gitbook/assets/image%20%28658%29.png)

Permite seleccionar la precisión con que se ubicará la posición del dispositivo rastreado.

| Nombre | Proveedor de ubicación | Descripción |
| :--- | :--- | :--- |
| DESIRED\__ACCURACY\_HIGH_ | GPS+Wifi+Red Celular | Consumo de energía alto y precisión de ubicación alta |
| DESIRED\__ACCURACY\_MEDIUM_ | Wifi+Red Celular | Consumo de energía medio y precisión de ubicación medio |
| DESIRED\__ACCURACY\_LOW_ | Wifi \(baja energia\) +Red Celular | Menor consumo de energía y precisión de ubicación baja |
| DESIRED\__ACCURACY\_VERY\_LOW_ | Red Celular | Mucho menos consumo de energía y precisión de ubicación muy baja  |

## Distance filter

![](../../../../.gitbook/assets/image%20%28688%29.png)

Establece un radio de distancia que activa la función cuando el usuario llega del punto original a la distancia establecida en la entry var

## Params

![](../../../../.gitbook/assets/image%20%28669%29.png)

Permite asignar parámetros que se requieran dentro del webhook 

![](../../../../.gitbook/assets/image%20%28673%29.png)

Se crea un parámetro y dentro de él, puedes agregar la información que requieres en las funciones dentro del webhook

![](../../../../.gitbook/assets/image%20%28667%29.png)

## Should show debug notifs

![](../../../../.gitbook/assets/image%20%28664%29.png)

Cuando se activa muestra un aviso cada vez que se dispara la función \(solo para pruebas\)

## Stop on terminate

![](../../../../.gitbook/assets/image%20%28671%29.png)

Cuando se encuentra activado va a detener el rastreo en cuento se cambie de aplicación o cambie de pantalla, si se encuentra desactivado, va a continuar el rastreo en segundo plano

## Url

![](../../../../.gitbook/assets/image%20%28692%29.png)

Se agrega el Url que se genera en el App process cuando se define que se ejecutara en la nube.

### Configuración del App process a webhook

Agregar una variable llamada **location** en Process input dentro del app process \(es indispensable agregar esta función dentro del App process pero no es necesario agregarlo en la entry var **Params** dentro de la función Start geolocation tracking http, puesto que esta se agrega por defecto en Params\)

![](../../../../.gitbook/assets/image%20%28690%29.png)

Se debe agregar las variables en Process input dentro del app process que se agregaron en Params de la función Start geolocation tracking http \(deben ser exactamente igual las variables\)

![variables en App process](../../../../.gitbook/assets/image%20%28661%29.png)

![variables en Params](../../../../.gitbook/assets/image%20%28694%29.png)

{% hint style="danger" %}
Importante agregar Callbacks
{% endhint %}

Se deben agregar Callbacks en Process callbacks dentro del app process, son indispensables agregarlas para saber cuando finalizan los procesos de las funciones del app process, de no hacerlo puede generar enormes gastos en su cuenta de Google

![callbacks en App process](../../../../.gitbook/assets/image%20%28677%29.png)

![callbacks en la l&#xF3;gica del App process](../../../../.gitbook/assets/image%20%28682%29.png)

Asignar la lógica correspondiente en onTriggered dentro del app process

Activar el switch onCloud

![](../../../../.gitbook/assets/image%20%28672%29.png)

Presionar el botón **Generate webhook url**

![](../../../../.gitbook/assets/image%20%28674%29.png)

Presionar el botón **Generate url** para generar la nueva url de nuestro webhook

![](../../../../.gitbook/assets/image%20%28687%29.png)

Copiar la url generada del webhook

![](../../../../.gitbook/assets/image%20%28668%29.png)

Pegarla en la Entry var **Url** de la función **Start geolocation tracking http**

![](../../../../.gitbook/assets/image%20%28654%29.png)

{% hint style="danger" %}
Para producción se debe sustituir la url por la nueva url que se envía al correo al momento de compilar la aplicación
{% endhint %}

