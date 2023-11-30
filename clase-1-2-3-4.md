# Introducción e instalación de JDK
**JAVA**
Es un lenguaje de programación orientado a objetos multiplataforma.
Para programar en JAVA necesitamos:

   * Descargar el JDK.
   * Bloc de notas y CMD.

**Al no programar con editores profesionales o entornos de desarrollo (IDE), la retención de sintaxis es mayor y el desarrollo de la habilidad incrementa bastante al no tener ayuda**

*Minecraft, OpenOffice y Android se desarrollaron en JAVA*

```cmd
java -version
```
## Indentado, compilación y ejecucióm del código
El código se debe de leer de arriba hacia abajo y de derecha a izquierda.
La primera línea que debemos escribir es el nombre de nuestra clase. En java necesitamos de clases para poder ejecutar un programa y esa clase es la que va a contener el código que nosotros vamos a escribir. El método main es donde va a dar inicio tu programa. Lo que va a permitir que lo podamos ejecutar.

**Los archivos java se guardan con el mismo nombre de la clase**

Con Java necesitamos un compilador `javac`, esto lo traduce.
Escribimos en el cmd:
`javac name.java`
Luego creará el archivo `name.class`.
Ahora `java name`
Así se ejecuta un programa desde 0 en java.

## Errores sintáticos y lógicos
Estandarización: Standard de java, empieza el nombre de neustra clase con Mayúscula.

```java
public class Error{
  public static void main(String args[]){
   System.out.println("Hello world"); 
 }
}
```