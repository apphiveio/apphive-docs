# Show file browser

![](../../../../gitbook/assets/image%20%28531%29.png)

La función Show file browser permite al usuario seleccionar archivos como imágenes, pdf, audio o texto plano  desde su dispositivo

[Información general](https://docs.apphive.io/reference/funciones/informacion-general-de-las-funciones) 



=== "Callbacks"

    ## Error retrieving file

    Se activa cuando ocurre un error durante el proceso de recuperación de los archivos para poder mostrarlos

    ## File retrieved

    Se activa cuando se recuperan los archivos de forma exitosa, retornando todos los archivos que se seleccionaron dentro de la galería de archivos del dispositivo

=== "Entry Vars"

    ## Select of media gallery

    ![](../../../../gitbook/assets/image%20%28523%29.png)

    Al activar esta entry var, permite seleccionar archivos de imagen de la galería del dispositivo

    !!! info

        Para los demás tipos de archivos no es necesario activarlo


    ## Select multiple files

    ![](../../../../gitbook/assets/image%20%28528%29.png)

    Al activar esta entry var, permite seleccionar mas de un archivo del mismo tipo de la galería del dispositivo

    ## Type file

    ![](../../../../gitbook/assets/image%20%28530%29.png)

    Perite seleccionar el tipo de archivo que se va a buscar dentro del dispositivo

    1. All files
    2. Audio
    3. Images
    4. pdf
    5. Plain Text
