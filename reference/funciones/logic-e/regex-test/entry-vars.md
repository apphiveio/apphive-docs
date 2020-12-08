# Entry Vars

## Basic regex

![](../../../../.gitbook/assets/image%20%28491%29.png)

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

{% hint style="warning" %}
Cundo se ingrese una custom regex, el basic regex debe estar en None para que el sistema valide la custom regex
{% endhint %}

## String to evalue

Es la cadena que se va a evaluar para que coincida con los patrones establecidos en basic regex o custom regex

