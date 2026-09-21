Hola asesores 2027 o angie, espero que alguien lea esto para que sepa algo del juego.

Primero quiero decir que el codigo que escribi esta horrible, espero nadie trate de aprender de el, tengo la opcion de reestructurarlo en dos dias, pero no lo haré pq me parece que asi esta bonito, solo arreglare las fugas de memoria y errores criticos que creo no tiene. 

Algo que si vale la pena mencionar es para que sirve cada archivo y la estructura de archivos, por si se quiere cambiar, arreglar o quitar algo.

El repositorio contiene 3 directorios en el directorio raiz; el primero es ".biblioteca", en el mismo se encuentran dos archivos uno .h y el otro .c que definen varias funciones que se ocupan en el programa principal, este directorio no es vital y creo que seria mejor si se quitara; el segundo directorio es "src", en este se encuentran dos archivos, uno contiene las reglas y el otro las palabras que pueden aparecer en el juego ambos archivos son texto plano por si se quiere editar alguna cosa facilmente; el ultimo directorio es "statics", aqui se encuentran las fuentes e imagenes que usa el juego.

En el directorio raiz del repositorio se encuentran 4 archivos. El archivo Palabras.bat y el archivo Palabras.sh, al ejecutarse compilan y ejecutan el juego, ademas convierten los archivos en src a archivos de solo lectura y en el caso de Palabras.bat oculta el archivo que contiene las palabras usadas en el juego, el sh no lo hace pq ocultar cosas en linux es un chiste. Los archivos bat se usan en windows y los archivos sh en sistemas UNIX.  
El archivo programa.c es el que contiene todo el juego, de este no digo nada por que tratare de documentarlo un poco en estos dias por si se quiere hacer algun cambio.  
El archivo .gitignore me parece que saben que hace.
  
Para compilar el juego sin usar los archivos sh o bat ejecuta:
``` bash
    gcc programa.c .biblioteca/funjs.o -o programa.exe -lallegro -lallegro_primitives -lallegro_image -lallegro_font -lallegro_ttf
```
Angie, si lees esto perdona mi pesima redaccion.
