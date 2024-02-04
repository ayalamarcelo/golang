###

<h1 align="center">Programación con Java</h1>

###

<h2 align="left">Tabla de contenidos:</h2>

- [Arreglos bidimensionales (Matrices)](#arreglos-bidimensionales-matrices)
- [Arreglos bidimensionales (Matrices dinámicas)](#arreglos-bidimensionales-matrices-dinámicas)
- [Interfaces gráficas (Librería Swing)](#interfaces-gráficas-librería-swing)
- [Interfaces gráficas (swing - JFrame)](#interfaces-gráficas-swing---jframe)



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

## Arreglos bidimensionales (Matrices dinámicas)
Al igual que los vectores, las matrices también pueden tener un comportamiento dinámico, es decir, el llenado se haga automáticamente además que el recorrido de nuestros índices también lo van a hacer sin necesidad que nosotros escribamos muchas líneas de código indicando a los índices cada posición que deben recorrer.


Filas = 3
Columnas = 3
Contador = 1

```java
int numeros [][] = new int[filas][columnas];

for(int j = 0; j < filas; j++) {
  for (int i = 0; i < columnas; i++) {
    numeros[j][i] = contador;
    contador++;
    System.out.print("[" + numeros[j][i] + "]");
  }
  System.out.println("");
}
```

> La estructura repetitiva for nos ayuda a darle ese comportamiento dinámico a nuestros índices.
> Tenemos un for dentro de otro for.

|:--| 0 | 1 | 2 |
|:--|:--|:--|:--|
| 0 | 1 | 2 | 3 |
| 1 | 4 | 5 | 6 |
| 2 | 7 | 8 | 9 |

i = 0
j = 0

contador  = 1

## Interfaces gráficas (Librería Swing)
Una interfaz gráfica es un programa informático que facilita el entorno visual utilizando imágenes y objetos gráfico para representar las acciones y la información disponible en la interfaz, con esto el usuario puede manipular el programa sin la necesidad de escribir comandos e instrucciones complejas. Las interfaces gráficas surgen como una evolución de las interfaces de líneas de comando que se utilizaban en los primeros sistemas operativos. Un ejemplo de línea de comandos es el cmd de windows.
El jdk nos provee de distintas librerías y métodos, ejemplo: scanner. Ahora para hacer una interfaz gráfica tenemos que volver a recurrir en una librería la cual va a ser `swing`.

```java
import javax.swing.*;

public class Formulario extends JFrame{
  private JLabel label1;

  public Formulario(){
   setLayout(null)
   label1 = new JLabel("Hola mundo");
   label1.setBounds(10, 20,200,300);// coordenadas ancho y alto
   add(label1); //agregar
 }

 public static void main(String args[]){
  Formulario formulario1 = new Formulario();
  formulario1.setBound(0,0,400,300);
  formulario1.setVisible(true);
  formulario1.setLocationRelativeTo(null);// quiero que aparezca al centro de mi pantalla
 }
}
```
> `*` hacemos referencia a que vamos a utilizar todos los elementos que posee la librería swing. Para evitar estarlos importando cada vez que vayamos a utilizar uno.

> `extends` nos ayuda a importar  clases que han programado previamente otras personas y esas clases las incluye dentro del jdk.

Estamos combinando la librería swing junto con una nueva clase la cual vamos a importar y se llama `JFrame`. JFrame nos permite crear interfaces gráficas. La librería `swing` nos permite importar los elementos para armar nuestras interfaces, mientras que la clase JFrame lo que hace es permitirnos crear la interfaz gráfica, el contenedor donde van a ir todos nuestros elementos. Entonces al escribir la palabra `extends` estamos diciendo que queremos hacer uso de una clase que ya existe y que está en el jdk, el cual estamos importando gracias a la librería `swing`.
`JLabel` nos permite crear etiquetas, donde vamos a poder crear o mostrar datos en pantalla sin necesidad de un `System.out.print` el jlabel es mostrar esos datos en la interfaz gráfica.
`Modificadores de acceso` `private & public` son guardias de seguridad, se encargan de decir qué espacios son públicos y cuales privados. Con los modificadores de acceso le indicamos al programa qué elementos o clases u objetos van a ser de dominio público o de dominio privado. Nuestos JLabel siempre deben ser de dominio privado, solo los vamos a utilizar en la interfaz que estamos programando actualmente, mientras que el nombre de la clase, clase general es de dominio público, porque tienen que encontrarse.
`setLayout` va a indiciar a través de coordenadas donde queremos colocar los elementos de toda la interfaz, pero para evitar que los coloque donde quiera tenemos que poner la palabra `null`.
Los métodos los unimos con un punto cuando queremos que afecte a un objeto directamente o a un elemento, en este caso que afecte a nuestra `label1`.
`constructores` un constructor te permite construir cosas pero no en el lugar donde estás programando sino en un lugar donde lo vas a invocar. Un constructor debe llamarse igual que el nombre de tu clase `!importante`.

## Interfaces gráficas (swing - JFrame)
Vamos a manipular las coordenadas donde va a aperecer nuestra interfaz. 
