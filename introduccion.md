###

<h1 align="center">Introducción a Java</h1>

- [Variables y tipos de datos](#variables-y-tipos-de-datos)
- [Operadores](#operadores)
- [Estructuras de control](#)
    - [If & Else](#)
    - [Switch]
###

<h2>Compilar Java</h2>
<p>Los archivos de Java se guardan con el mismo nombre.</p>

```bash
# Con Java necesitamos un compilador 
`javac` 
#esto lo traduce. 
# Escribimos en el cmd: 
`javac name.java` 
# Luego creará el archivo 
`name.class`.
# Ahora 
`java name`.
# Así se ejecuta un programa desde 0 en java.
```

###

<h2>Variables</h1>

###

<p align="left"> Una variable es un espacio en memoria donde podemos alojar información o datos ya sean de tipos numérico o de tipo texto. Para que nosotros declaremos una variable, necesitamos de dos elementos. En primer lugar, necesitamos de un `tipo` de dato y el segundo necesitamos de un `nombre`. Con el tipo de dato le vamos a decir al espacio en memoria qué tipo de información o dato va a recibir. Con el nombre vamos a decirle a nuestro programa a que variable o espacio en memoria estamos haciendo referencia. 
</p>

###

**Ejemplo:**
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
###

<h2>Tipos de datos</h2>

**Primitivos**
*Enteros*

  - byte (-128 hasta 127)
  - short (-32,768 hasta 32,767)
  - int (-2,147,483,648 hasta 2,147,483,647)
  - long (muy grande...)

**Decimales** (nos permiten alojar valores con punto decimal)
   
   - float
   - double

**Otros**

   - char (un solo caracter)
   - booleand (true/false)

**Tipos objeto** (son clases)

   - String, ejemplo 'Hola mundo'.

###

<h2 align="center">Operadores</h2>

| **Signo** | **Nombre del Signo** | **Tipo de operación**       | **Código ASCII** |
| :-------- | :------------------- | :-------------------------- | :--------------- |
| **+**     | Más                  | Suma                        | **ALT + 43**     |
| **-**     | Menos                | Resta                       | **ALT + 45**     |
| **(*)**   | Asterisco            | Multiplicación              | **ALT + 42**     |
| **/**     | Diagonal o Slash     | División                    | **ALT + 47**     |
| **^**     | Acento circunflejo   | Potencia                    | **ALT + 94**     |
| **(**     | Paréntesis apertura  | Prioridad entre operaciones | **ALT + 40**     |
| **)**     | Paréntesis cierre    | Prioridad entre operaciones | **ALT + 41**     |

<span>Operadores lógicos y relacionales</span>

| Operador |         Nombre         |    Ejemplo    |       Significado        |
| :------: | :--------------------: | :-----------: | :----------------------: |
|    <     |       Menor que        |     5 < 4     |     5 es menor que 4     |
|    >     |       Mayor que        |     A > B     |     A es mayor que B     |
|    ==    |       Igual que        |    5 == 5     |     5 es igual que 5     |
|    !=    | No igual a (diferente) | perro != gato | perro no es igual a gato |
|    <=    |  Menor que o igual a   |    A <= B     |  A es menor que o igual  |
|    >=    |  Mayor que o igual a   |    A >= B     |  A es mayor que o igual  |

###

<h2>Estructuras condicionales</h2>
<span>If & Else</span>
<p align="left">Es una instrucción que ayuda a nuestros programas a saber qué proceso o qué camino debe de seguir dependiendo en la situación que se encuentre. Una estructura condicional si no tiene condición no puede ser estructura condicional. No hay camino o proceso que seguir.</p>

```java
public class Promedio{
  public static void main(String args[]){

   int matematicas = 5;
   int biologia = 8;
   int quimica = 7;
   int promedio = 0;

   promedio = (matematicas + biologia + quimica) / 3;
   
   if(promedio >= 6){
    System.out.println("El alumno aprobó " + promedio); 
   } else {
    System.out.println("El alumno desaprobó " + promedio);
   }
 }   
}
```