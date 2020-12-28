# Entry Vars

## Desired accuracy

![](../../../../.gitbook/assets/image%20%28663%29.png)

Permite seleccionar la precisión con que se ubicará la posición del dispositivo rastreado.

| Nombre | Proveedor de ubicación | Descripción |
| :--- | :--- | :--- |
| DESIRED\__ACCURACY\_HIGH_ | GPS+Wifi+Red Celular | Consumo de energía alto y precisión de ubicación alta |
| DESIRED\__ACCURACY\_MEDIUM_ | Wifi+Red Celular | Consumo de energía medio y precisión de ubicación medio |
| DESIRED\__ACCURACY\_LOW_ | Wifi \(baja energia\) +Red Celular | Menor consumo de energía y precisión de ubicación baja |
| DESIRED\__ACCURACY\_VERY\_LOW_ | Red Celular | Mucho menos consumo de energía y precisión de ubicación muy baja  |

## Distance filter

![](../../../../.gitbook/assets/image%20%28670%29.png)

Establece un radio de distancia que activa la función cuando el usuario llega del punto original a la distancia establecida en la entry var

## Should show debug notifs

![](../../../../.gitbook/assets/image%20%28681%29.png)

Cuando se activa muestra una notificación cada vez que se dispara la función \(solo para pruebas\)

## Stop on terminate

![](../../../../.gitbook/assets/image%20%28686%29.png)

Cuando se encuentra activado va a detener el rastreo en cuento se cambie de aplicación o cambie de pantalla, si se encuentra desactivado, va a continuar el rastreo en segundo plano

