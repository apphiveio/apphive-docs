---
description: Para redondear a la centena más cercana divide entre 100, redondea con Global Formater (round) y multiplica el resultado por 100.
---

# ¿Cómo puedo redondear a la centena más cercana?

Global Formater redondea a entero, así que el truco es cambiar la escala: divide el número entre 100, redondéalo y vuelve a multiplicarlo por 100. Por ejemplo, 260 se redondea a 300 y 1850 a 1900.

## Pasos

1. Divide el número entre 100 con [Arithmetic Operation](../reference/funciones/logic-e/arithmetic-operation/README.md). Por ejemplo, 1850 → 18.5.
2. Pasa el resultado por [Global Formater](../reference/funciones/logic-e/global-formater/README.md) con origen de tipo **number** y salida **round**. 18.5 → 19.
3. Multiplica el resultado del Global Formater por 100. 19 → 1900.

!!! note
    El mismo método sirve para otras escalas: divide y multiplica entre 10 para redondear a la decena, o entre 1000 para redondear al millar.
