# 1.1 Herramientas. Git LFS
## Crea una carpeta  que incluya 2 imágenes y 3 ficheros de texto. La utilizaremos para crear un repositorio Git que se conecte a GitHub. Puedes utilizar comandos o una herramienta visual. Las imágenes deben tener seguimiento LFS. Añade una imagen adicional y un fichero adicional y actualiza el repositorio GitHub con la nueva versión del proyecto.

1. Creamos el repositorio Git a partir de la carpeta local actual.
```
git init
```

2. Creamos 2 imágenes y 3 ficheros de texto en la carpeta del repositorio. Los ficheros de texto se han creado con el siguiente comando:
```
echo "txt1" > txt1.txt
```
Las imágenes correspondientes se han descargado de Google Imágenes.

3. Habilitamos Git LFS en el repositorio.
```
git lfs install
```

4. Indicamos a Git LFS que debe gestionar los ficheros con extensión jpg.
```
git lfs track *.jpg
```
Se creará un fichero .gitattributes con un listado de los jpg dentro del repositorio.

5. Añadimos los cambios actuales para posteriormente commitearlos.
```
git add .
git commit -m "first commit"
```

6. Creamos otra imagen y otro fichero de texto en el repositorio, y confirmamos los cambios de la siguiente manera:
```
git lfs track *.jpg
git add .
git commit -m "add another image and text file"
```

## Crea un repositorio Git LFS para el proyecto Unity de la tarea 1.2. Configura el fichero .gitattribute adecuado. Una segunda versión del fichero debe incluir una textura y un segundo script que muestre el mensaje en consola "Script tarea 1.2".
Se han necesitado los siguientes ficheros de configuración:
- [.gitignore](https://github.com/gcruz174/fdv2425_1.2_unityinterface/blob/main/.gitignore)
- [.gitattributes](https://github.com/gcruz174/fdv2425_1.2_unityinterface/blob/main/.gitattributes)


- [Textura](https://github.com/gcruz174/fdv2425_1.2_unityinterface/blob/main/Assets/TP_FastFood/Materials/ColorPallete.png)
- [Script](https://github.com/gcruz174/fdv2425_1.2_unityinterface/blob/main/Assets/Scripts/PrintMessage.cs)