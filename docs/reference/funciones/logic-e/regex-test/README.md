# Regex Test

![](../../../../gitbook/assets/image%20%28484%29.png)

La función Regex Test permite comparas los valores con patrones para encontrar una determinada combinación de caracteres dentro de una cadena de texto

[Información general](https://docs.apphive.io/reference/funciones/informacion-general-de-las-funciones)



=== "Callbacks"

    ## Does not match

    Se activa cuando la cadena evaluada no coincide con el patrón establecido de comparación

    ## Match

    Se activa cuando la cadena evaluada coincide con el patrón establecido de comparación

    ## onError

    Se activa cuando ocurre un error durante el proceso de evaluación de la cadena con el patrón

=== "Entry Vars"

    ## Basic regex

    ![](../../../../gitbook/assets/image%20%28491%29.png)

    Perite elegir un patrón predefinido por el sistema para comparar el texto \(generalmente ingresado por el usuario\)

    | Basic regex | Definición |
    | :--- | :--- |
    | Email | Compara y valida una cadena con el patrón de estructura de un correo electrónico |
    | only numbers | Compara y valida una cadena solamente con números |
    | only letters | Compara y valida una cadena solamente con letras |
    | At least three characters | Compara y valida una cadena para que contenga al menos 3 dígitos |
    | Phone \(10 digits\) | Compara y valida una cadena con una estructura de un numero telefónico de 10 dígitos solamente |
    | Phone \(With country code\) | Compara y valida una cadena con una estructura de un numero telefónico con LADA |

    ## Custom regex

    Permite agregar una expresión regular para poder cumplir un patrón especifico personalizado y aceptar otro tipo de cadenas a las básicas

    !!! warning

        Cundo se ingrese una custom regex, el basic regex debe estar en None para que el sistema valide la custom regex


    ## String to evalue

    Es la cadena que se va a evaluar para que coincida con los patrones establecidos en basic regex o custom regex
