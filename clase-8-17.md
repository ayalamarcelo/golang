# Como introducir datos desde el teclado con scanner
Cuando comenzamos a programar en ocasiones requerimos interactuar con el usuario. Que nuestro programa le permita al usuario introducir datos desde el teclado. Vamos a diseñar un programa donde le pida tanto su nombre y números para poder sumarlos. Para esto vamos a utilizar una librería `Scanner`.
Conjunto de códigos escritos por alguien más. Para poder hacer uso de estas librerías, debemos importarlas.
Scanner es una sublibreria que nos permite poner datos. Para hacerlos más dinámico.

Importar :

```java
import java.util.Scanner;
```

```java
import java.util.Scanner;

public class Suma{
 public static void main(String args[]){

   Scanner in  = new Scanner(System.in); /*Vamos a introducir datos con ayuda de la clase System*/
   String nombre = "";
   int numUno = 0, numDos = 0, resultado = 0;

   System.out.println("¿Cuál es tu nombre?"); /*Despues de este mensaje se va a detener por un momento hasta que el usuario escriba algo y presione la tecla enter*/
   nombre = in.nextLine(); /*Si guardamos valores numericos in.nextInt*/
   /*Viene a nuestro objeto in recoge los datos y los va a guardar en la variable nombre y luego se limpia nuestro objeto*/
   System.out.println("Dame el primer valor para tu suma: ");
   numUno = in.nextInt();
   System.out.println("Dame el segundo valor para tu suma:");
   numDos = in.nextInt();

   resultado = numUno + numDos;

   System.out.println("Hola " + nombre + " el resultado de tu suma es: " + resultado);
 }   
}
```

## Condiciones compuestas con operadores lógicos y relacionales

| Operador | Nombre | Ejemplo | Significado |
|:--------:|:------:|:-------:|:-----------:|
| < | Menor que | 5 < 4 | 5 es menor que 4 |
| > | Mayor que | A > B | A es mayor que B |
| == | Igual que | 5 == 5 | 5 es igual que 5 |
| != | No igual a (diferente) | perro != gato | perro no es igual a gato |
|<= | Menor que o igual a | A <= B | A es menor que o igual |
|>= | Mayor que o igual a | A >= B | A es mayor que o igual |

