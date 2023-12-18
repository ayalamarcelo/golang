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

1:29