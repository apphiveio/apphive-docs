---
description: Para un pedido programado pide al usuario el día y la hora con pickers, guárdalos en el pedido y valida que la hora no sea demasiado próxima.
---

# Cómo hacer un pedido programado

Un pedido programado (entrega o recolección a una hora elegida por el cliente) no necesita programación especial: pide al usuario el día y la hora, guárdalos junto con el pedido en la base de datos y valida que la hora elegida tenga sentido para tu negocio.

## Pasos

1. En la pantalla del carrito agrega los controles para elegir el momento del pedido, por ejemplo dos **Picker**: uno con los días y otro con las horas (20:00, 20:30, 20:45…). Si lo prefieres, puedes mostrarlos dentro de un **Bottom menu sheet**.
2. Si ofreces **recoger en tienda**, agrega un **Switch** para que el cliente elija entre entrega a domicilio y recoger; muestra los pickers de hora cuando corresponda.
3. Al confirmar el pedido, guarda el día y la hora elegidos como campos del pedido en la base de datos.
4. Agrega una validación antes de guardar; por ejemplo, que la hora del pedido no sea antes de 30 minutos de la hora actual.
5. En la app del negocio o del repartidor, lee esos campos para saber si el pedido es para entrega inmediata o para la hora indicada.

!!! note

    El picker de días depende del tipo de negocio: en un restaurante normalmente basta con elegir la hora del mismo día; en servicios con cita puede tener sentido elegir varios días.

!!! tip

    Si la lógica del pedido se usa en varias pantallas, ponla en un **App process** para llamarla desde donde la necesites.

Consulta también [Picker](../reference/controles/picker/README.md) y [Toogle bottom menu sheet](../reference/funciones/controls/toogle-bottom-menu-sheet/README.md).
