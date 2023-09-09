## ¿Qué es Go?

Go es un lenguaje de programación que se ha desarrollado en Google. Go es expresivo, conciso y limpio. Go destaca en parte debido a sus mecanismos de simultaneidad únicos, lo que facilita la escritura de programas que pueden aprovechar varios núcleos a la vez. Se trata principalmente de un lenguaje fuerte y con establecimiento de tipos en modo estático, lo que significa que los tipos de variables se conocen en tiempo de compilación. Sin embargo, tiene algunas funcionalidades de tipos dinámicos.
Go tiene muchas similitudes con C y hereda aspectos de la sintaxis de C, como las instrucciones de flujo de control, los tipos de datos básicos, los punteros y otros elementos. Sin embargo, la sintaxis y la semántica del lenguaje van más allá de C. También comparte similitudes con Java, C#, Python y otros. En general, Go tiende a tomar prestadas y adaptar características de otros lenguajes de programación, aunque dejando de lado la mayor parte de la complejidad. Por ejemplo, puede usar algunas características de programación orientadas a objetos (OO) y patrones de diseño en Go, pero el paradigma de OO completo no está totalmente implementado. Conocerá los motivos más adelante en esta ruta de aprendizaje.

## Instalación

Confirmar que Go se ha instalado correctamente:

```cmd
go version
```
## Configuración de un área de trabajo de Go

Go difiere de otros lenguajes de programación en el modo en que organiza los archivos de proyecto. En primer lugar, Go funciona bajo el concepto de áreas de trabajo. Un área de trabajo es simplemente una ubicación en la que reside el código fuente de la aplicación. En Go, todos los proyectos comparten la misma área de trabajo. Pero Go ha empezado a cambiar este enfoque a partir de la versión 1.11. No tiene que preocuparse de eso todavía, porque abordaremos las áreas de trabajo en el siguiente módulo. Por ahora, el área de trabajo de Go se encuentra en $HOME/go, pero, si es necesario, se puede configurar otra ubicación para todos los proyectos.

## Compilación de un archivo ejecutable

Para generar un archivo ejecutable para el programa, use este comando:

```
go build main.go
```
## Declaración de variables

Para declarar una variables se usa la palabra clave:

```
var firstName string
```
La instrucción anterior declara una variable denominada firstName de tipo string. Hablaremos de los tipos de datos en la próxima sección. En este ejemplo se muestra la manera más sencilla de declarar una variable. Si quiere declarar otra variable, simplemente agregue una instrucción similar a la anterior. Puede declarar más de una variable en una sola línea si son del mismo tipo:

```
var firstName, lastName string

```