# Cadenas de caracteres con el método equals
Es una secuencia de caracteres que pueden contener símbolos letras o números. 

**String** --> Permite declarar variables para alojar cadenas de caracteres (Texto).

## Declarar una variable
int numero = 0;
String nombre = "";

## Comparar valores
numero == 9;
nombre == "Juan";
nombre.equals("Juan");

>[!Note]
> "Equals" Le indica al programa que quieres comparar una cadena de caracteres en específico.

## Ejercicio
1. Realizar un programa que compare dos nombres para verificar que son iguales, mostrando un mensaje en pantalla al final que diga: los nombres son iguales / los nombres son diferentes. 

>[!Note] 
> Los nombres debe de introducirlos el usuario desde el teclado.

2. Realizar un programa que simule un inicio de sesión solicitando el nombre del usuario y la contraseña, para posteriormente comprarlos y mostrar un mensaje en pantalla que diga: Inicio de sesión correcto - nombre de usuario o password incorrectos.

## Manipulación de cadenas con los métodos lenght() y substring()
Cuando nosotros trabajamos con cadenas de caracteres, es muy importante poder manipularlas desde el hecho de saber cuántos caracteres contiene dicha cadena hasta poder cortar y obtener cierta cantidad de caracteres que vayamos a requerir. Para ello java pone a disposición dos métodos que es:

## Método lenght y método substring

Método **lenght** -> Indica cuantos caracteres posee una cadena de caracteres.

> C a r l o s
> 1 2 3 4 5 6

Posee un total de 6 caracteres

Método **substring** -> permite obtener una parte en específico de la cadena de caracteres. substring(desde, hasta);

> C a r l o  s
>0 1 2 34   5 6

* Obtener

> desde : 0
> hasta : 4

*Carl*

>[!Note] 
> Cuenta los espacios que hay entre letras

A diferencia del método lenght, al método substring hay que indicarle desde qué punto hay que punto hasta qué punto queremos hacer dicho corte.

## Arreglos unidimensionales (Vectores)
Un arreglo es una estructura de datos que almacena bajo el mismo nombre a una colección de datos. Un arreglo está seccionado o divido en varias partes.

Lista de alumnos --> Nombre de la colección de datos

| # de Lista | Nombre |
|:----------:|:------:|
| 1 | Juan |
| 2 | Guillermo |
| 3 | Ana |
| 4 | Luis |

<-- Colección de datos 

## Los arreglos se caracterizan por:

1. Almacenar los elementos en posiciones contiguas de memoria.
2. Tienen un mismo nombre de variable que representa a todos los elementos.
3. Los elementos son asignados a una posición dentro del vector.
4. Los arreglos trabajan en conjunto con índices que especifican la posición de cada elemento dentro del arreglo.

| # de Lista | Nombre |
|:----------:|:------:|
| 1 | Juan | --> Posición 1
| 2 | Guillermo | --> Posición 2
| 3 | Ana | --> Posición 3
| 4 | Luis | --> Posición 4

Esta flecha es un índice que indica la posición del elemento.

## Tipos de arreglos
* Tenemos dos tipos de arreglos

1. Arreglos unidimensionales mejor conocidos como "Vectores".

| v | v | v | v | v | v |
|---|---|---|---|---|---|

2. Arreglos bidimensionales mejor conocidos como "Matrices".

| v | v | v | v |
|---|---|---|---|
| v | v | v | v |
| v | v | v | v |
| v | v | v | v |

## Vectores (Arreglos unidimensionales)

Representación gráfica de un Vector:

| Juan | Guillermo | Ana | Luis | Pedro |
|:----:|:---------:|:---:|:----:|:-----:|

>[!Note]
> Se le llama unidimensional porque es una lista de una sola dimensión. Es decir, solo podemos guardar datos de atras hacia adelante o de adelante hacia atras.

Su longitud o tamaño depende del número de posiciones que nosotros le asignamos al momento de declarar el vector. Por ejemplo, este vector cuenta con 5 posiciones, aunque tenga 5 posiciones. Siempre la posición inicial de un vector debe de ser cero independientemente del nro de posiciones que contenga y estas posiciones incrementa de 1 en 1 hasta llegar a la posición final. Es por eso que la última posición de este vector es 4, aunque el nro total de posiciones en de 5.

| Posición 0 (inicial) | Posición 1 | Posición 2 | Posición 3 | Posición 4 (final) |
| Juan | Guillermo | Ana | Luis | Pedro |
|:----:|:---------:|:---:|:----:|:-----:|

>[!Note]
> Esta divido en 5 seccciones y a cada sección se le conoce como posición.

## Indice de un Vector
Los vectores trabajan en conjunto con un índice que se representa gráficamente con una fecha, las cuales necesitan ser declaradas como una variable del tipo entero y por consecuencia deben de tener un nombre y un valor de arranque o inicio.


Tipo de dato del índice[int]
Nombre del índice[indice_uno]
Valor inicial del índice[0]

`int indice_uno = 0;`

Este índice nos ayuda a recorrer todo el arreglo tanto de ida como de vuelta.

     | Posición  0 |
     |:-----------:|
     | Juan | <- Indice

Con la finalidad de consultar, modificar, eliminar o insertar algún elemento en cualquiera de las posiciones del lector.

## Sintaxis y pasos para programar un vector
Al igual que una variable, un vector hay que declararlo e indicarle lo siguiente: 

En primer lugar el tipo de datos que vamos a manejar. Cuando todos los tipos ingresen deberan de ser del mismo tipo de dato. Posteriormente hay que asignarle un nombre. Una vez asignado el nombre agregamos un par de corchetes [], luego inicializar el vector por lo que debemos agregarle un signo de igual. Escribimos la palabra `new` seguido nuevamente del tipo de dato que vamos a utilizar para nuestro vector, seguido de otro par de corchetes. Dentro el nro de posiciones que deseamos que contenga nuestro vector.

`int nombre[] = new int [5];`

* Introducir datos a nuestro vector
  
Para introducir elementos o datos a nuestro vector debemos de apoyarnos en el índice que acompaña a nuestro vector. Este índice tiene dos tipos de comportamiento. Un comportamiento estático y un comportamiento dinámico.
Un índice con comportamiento estático no es necesario declararlo ya que basta con indicar el nombre y la posición del vector a donde queremos que se dirija nuestro índice, esto quiere decir que no se moverá de su posición actual a no ser que nosotros le indiquemos de manera manual. Es decir, que escribamos una línea de código que le indique al indice que se debe de mover a una determinada posición.

`numeros[2] = 8;`

Nombre del vector[numeros]
Posición del vector[2]
Elemento a guardar[8]

Queremos guardar el elemento 8 en el vector numeros en la posición 2.

* Imprimir datos de un vector

Para imprimir solo utilizamos:

`System.out.println(numero[3]);`

Y dentro del paréntesis debemos de colocar el nombre del vector junto con la posición que queremos mostrar.

**Ejercicio**
Crear un vector de cinco posiciones, posteriormente guardar un número en cada una de las posiciones del vector, y finalmente imprimir en pantalla cada una de las posiciones para verificar que se hayan guardado los números de manera correcta.





