## Pregunta 1
#Preprocesador
El preprocesador mirá los encabezados y reemplaza "include" y "defines" por lo que dice en el encabezado

#Compilacion I
Convierte el código C preprocesador en Assembler

#Compilacion II
Convierte el código Assembler a lenguaje de máquina. Todavía tiene cosas sin definir --> hay que linkear
T, U, C: descriptores
Se puede ver con "nm"

#Linkeo
Linkea con las librerías para definir las funciones que no están definidas

## Pregunta 2



## Pregunta 3
con movl le dice ...

## Pregunta 4

T: Funcion (texto?)
U: sin definir. En este caso, es una función que se va a definir cuando se linkee


000000000000003c T add_numbers
0000000000000000 T main
                 U printf

## Pregunta 5

El ejecutable tiene más símbolos ¿definidos dentro de stdio.h?
En principio, creíamos que no deberìa haber U, pero hay. Se explica con librerías dinámicas. Todas tienen @@ que indica donde buscarlas
