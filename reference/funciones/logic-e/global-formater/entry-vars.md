# Entry Vars

## Origin data

![](../../../../.gitbook/assets/image%20%28463%29.png)

En esa sección se debe asignar el valor, arreglo u objeto que se desea se cambie su tipo de formato

## Origin Type

![](../../../../.gitbook/assets/image%20%28455%29.png)

En este sección se puede seleccionar los tipos de formatos en los que se encuentran actualmente la información de origen

## Origin Type

![](../../../../.gitbook/assets/image%20%28469%29.png)

Se puede asignar de igual manera el tipo de de estructura con la que se encuentra la información de origen

## Target Type

![](../../../../.gitbook/assets/image%20%28459%29.png)

Permite hacer selección de tipo de salida del la información de origen. El tipo de salida depende directamente del formato de la información de entrada.

<table>
  <thead>
    <tr>
      <th style="text-align:left">Formato de origen</th>
      <th style="text-align:left">Formato de salida</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">object</td>
      <td style="text-align:left">
        <ol>
          <li>arrayWithId</li>
          <li>arrayWithoutId</li>
          <li>get</li>
          <li>set</li>
        </ol>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">array</td>
      <td style="text-align:left">
        <ol>
          <li>concatArrays</li>
          <li>slice</li>
          <li>split</li>
        </ol>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">number</td>
      <td style="text-align:left">
        <ol>
          <li>Hexadecimal</li>
          <li>round</li>
          <li>money</li>
          <li>moneyNumber</li>
          <li>string</li>
        </ol>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">string</td>
      <td style="text-align:left">
        <ol>
          <li>noSpaces</li>
          <li>trimmed</li>
          <li>slice</li>
          <li>number</li>
          <li>Hexa Encoding</li>
          <li>MD5</li>
          <li>Base 64</li>
          <li>replace</li>
          <li>replaceAll</li>
          <li>Title Case</li>
          <li>Lower Case</li>
          <li>Upper Case</li>
          <li>sha256</li>
        </ol>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Base 64</td>
      <td style="text-align:left">
        <ol>
          <li>string</li>
        </ol>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">xml</td>
      <td style="text-align:left">
        <ol>
          <li>json</li>
        </ol>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">json</td>
      <td style="text-align:left">
        <ol>
          <li>xml</li>
        </ol>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">date</td>
      <td style="text-align:left">
        <ol>
          <li>date</li>
        </ol>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">HTML</td>
      <td style="text-align:left">
        <ol>
          <li>String</li>
        </ol>
      </td>
    </tr>
  </tbody>
</table>

### Locale

![](../../../../.gitbook/assets/image%20%28470%29.png)

Esta opción se hace presente solamente cuando el Origin Type está en formato date.

Esta opción permite mostrar la fecha en idioma español o en ingles, para lograr esto en la opción **Target type detail** se debe asignar la siguiente cadena **LLL**

| Idioma | Ejemplo de formato de salida |
| :---: | :---: |
| English | December 3, 2020 3:37 pm |
| Spanish | 3 de diciembre de 2020 15:37 |

## Target type detail

![](../../../../.gitbook/assets/image%20%28453%29.png)

Se puede asignar el tipo de de estructura con la que se saldrá la información de salida

