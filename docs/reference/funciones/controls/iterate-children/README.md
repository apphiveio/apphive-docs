---
description: >-
  Esta función permite hacer un recorrido  a los controles internos o hijos y
  detecta las propiedades y generales de los mismos.
---

# Iterate children

![](../../../../gitbook/assets/image%20%28326%29.png)



=== "Callbacks"

    ## On error

    Se activa cuando ocurre algún tipo de error en el proceso de iteración, la función retorna que tipo de error sucedió en su proceso en EventOutput

    ## On iteration

    Se activa cuando el proceso de iteración se realizó de forma correcta, retornando todos los controles seleccionados en la entry var Tag

=== "Entry vars"

    Consta de dos entry vars

    1. Parent
    2. Tags

    ## Parent

    Generalmente se manda un control de tipo contenedor que contiene controles anidados de cualquier tipo

    ## Tags

    Puedes seleccionar los tipos de controles que que se deben de identificar dentro del contenedor padre para poder realizar cualquier tipo de proceso dentro de su callback

    [Información general](https://docs.apphive.io/reference/funciones/informacion-general-de-las-funciones)
