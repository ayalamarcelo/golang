# Introducción e instalación de JDK
**JAVA**
Es un lenguaje de programación orientado a objetos multiplataforma.
Para programar en JAVA necesitamos:

   * Descargar el JDK.
   * Bloc de notas y CMD.

**Al no programar con editores profesionales o entornos de desarrollo (IDE), la retención de sintaxis es mayor y el desarrollo de la habilidad incrementa bastante al no tener ayuda.**

*Minecraft, OpenOffice y Android se desarrollaron en JAVA.*

```cmd
java -version
```
## Indentado, compilación y ejecución del código
El código se debe de leer de arriba hacia abajo y de derecha a izquierda.
La primera línea que debemos escribir es el nombre de nuestra clase. En java necesitamos de clases para poder ejecutar un programa y esa clase es la que va a contener el código que nosotros vamos a escribir. El método main es donde va a dar inicio tu programa. Lo que va a permitir que lo podamos ejecutar.

**Los archivos java se guardan con el mismo nombre de la clase.**

Con Java necesitamos un compilador `javac`, esto lo traduce.
Escribimos en el cmd:
`javac name.java`
Luego creará el archivo `name.class`.
Ahora `java name`.
Así se ejecuta un programa desde 0 en java.

## Errores sintáticos y lógicos
Estandarización: Standard de java, empieza el nombre de nuestra clase con mayúscula.

```java
public class Error{
  public static void main(String args[]){
   System.out.println("Hello world"); 
 }
}
```
Un error lógico se pueden causar por dos errores: error lógico del código o error lógico del programador.
Errores sintácticos: falta de punto y coma, que hayas puesto mal un paréntesis, mal el nombre de una variable. Un programa no se va a poder ejecutar si no corriges los errores.
*Aprender a leer errores*

## Variables y tipos de datos en JAVA
**Primitivos**
*Enteros*

  * byte (-128 hasta 127)
  * short (-32,768 hasta 32,767)
  * int (-2,147,483,648 hasta 2,147,483,647)
  * long (muy grande...)

**Decimales** (nos permiten alojar valores con punto decimal)
   
   * float
   * double

**Otros**

   * char (un solo caracter)
   * booleand (true/false)

**Tipos objeto** (son clases)

   * String, ejemplo 'Hola mundo'.

## Variables
Una variable es un espacio en memoria donde nosotros vamos a poder alojar información o datos ya sean de tipos numérico o de tipo texto.
Para que nosotros declaremos una variable, necesitamos de dos elementos. En primer lugar, necesitamos de un `tipo` de dato y el segundo necesitamos de un `nombre`. Con el tipo de dato le vamos a decir al espacio en memoria qué tipo de información o dato va a recibir. Con el nombre vamos a decirle a nuestro programa a que variable o espacio en memoria estamos haciendo referencia. 

Ejemplo:
`Tipo: int nombre: numUno`
Programamos una suma:

```java

public class Suma{
  public static void main(String args[]){
 
   int numUno = 5;
   int numDos = 2;
   int resultado = 0;
   
   resultado = numUno + numDos;
   System.out.println("El valor de tu suma es: " + resultado);
 }
}
```
