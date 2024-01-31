###

<h1 align="center">Programación con Java</h1>

###

<h2 align="left">Tabla de contenidos:</h2>

- [Arreglos bidimensionales (Matrices)](#arreglos-bidimensionales-matrices)



## Arreglos bidimensionales (Matrices)
Un arreglo en java puede tener más de una dimensión a este tipo de arreglos se les conoce como matrices. Una matriz en java al igual que un vector, es un espacio de memoria seccionado o dividido en varias partes, con la diferencia que en una matriz podemos guardar datos y dos dimensiones, es decir de lado a lado o bien de arriba hacia abajo.

Una matriz cuenta con varias filas y varias columnas, además que para poder hacer uso de una matriz en programación nosotros requerimos de dos índices.

```
índice i -> posición 0

índice j -> posición 0
```
El índice `i` se va a encargar de recorrer las columnas, mientras que el índice `j` se va a encargar de recorrer las filas. Hacemos uso de dos índices puesto que un índice no puede trabajar en dos dimensiones. Un índice solo puede hacer el recorrido de adelante hacia atras o bien hacer el recorrido de abajo hacia arriba.

<h3 align="left">Cómo funciona una matriz en conjunto con los índices</h3>

Si quiero localizar el nombre `Carmen` en mi matriz. Lo primero que debo hacer es: 
  Situar nuestros índices en la posición 0 de la fila o columna que hace referencia.

`Carmen` está en la columna 3, y en la fila 2.

```
índice i -> posición 3 columnas
índice j -> posición 2 filas
```
**Ejercicio:**
Crear un programa que muestre en pantalla una Matriz de 2 filas y 2 columnas con un número dentro de cada posición tal y como se muestra a continuación:

[5] [2]
[2] [5]

> Primero van las filas y luego las columnas.