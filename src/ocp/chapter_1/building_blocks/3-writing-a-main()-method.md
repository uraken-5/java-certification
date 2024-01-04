## Writing a main() Method
Un programa java inicia su ejecución con el método 'main'. En esta sección aprenderemos como crear uno (un programa, obvio) pasar parametros y ejecutar 
el programa. El método 'main' es usualmente conocido como el punto de entrada al programa ya que es lo primero que buscara la
JVM cuando ejecutes el programa.

## I. Creating a main() Method
El método 'main' le dice a la JVM que ejecute nuestro código. La clase mas simple luce asi con su metodo main.

```java
1:  public class Zoo {
2:      public static void main(String[] args) {
3:          System.out.println("Hello World");
4:      }
5:  }
```
Este metodo imprimira por consola la palabra 'Hello World'. para compilar y ejecutar este codigo debes colocarlo en 
un archivo de nombre Zoo.java y posicionarte en su ubicación para luego hacer:

```text
javac Zoo.java
java Zoo
```
Si el programa te dice 'Hello World' compilo bien, si aparecio algun error deberias primero que nada leer el error y posiblemente no tengas instalado el JDK 17 o quizas te falte configurar la variable de entorno PATH. 
Aqui no haremos troubleshooting asi que tendras que buscar con chatgp3. 

Para poder compilar un archivo java con el comando 'javac' el archivo debe tener la extensión '.java'. El nombre del archivo debe hacer
match con el nombre de la clase publica (Zoo).
El resultado es un archivo de bytecode con el mismo nombre del archivo pero con extension .class.

Vamos a revisar las palabras claves que tiene la firma del metodo 'main'l.

- 'public' es una palabra clave que declara el nivel de exposición del método para las clases la puedan llamar. 'public' indica que 
tenemos un acceso total desde cualquier parte del programa. 
- 'static' vincula el metodo en cuestion con la clase que la contiene. Esto significa que puedes llamar al método sin necesidad de crear un objeto.
- 'void' es un tipo de retorno. Indica que el metodo no devuelve ningun valor. Es buena practica utilizar 'void' en métodos que cambian el estado del objeto.
- 'main' finalmente llegamos a la lista de parametros del método main, representado por un array de java.lang.String. Se puede usar cualquier nombre de variable valido siguiendo alguno de estos tres formatos:
```java
String[] args
String options[]
String... friends
```
El compilador acepta cualquiera de estos. Arg, options y friends solamente son los nombres que se le asignaron a la lista de String.
Los corchetes indican que son arreglos de String y los tres puntitos son conocidos como 'varargs' (lista de argumentos variables) 

## Passing parameters to a java program
Vamos a ver como pasar parametros a un metodo. Modificaremos la clase Zoo para que imprima los dos argumentos que le son enviados.

```java
public class Zoo {
    public static void main(String[] args) {
        System.out.println(args[0]);
        System.out.println(args[1]);
    }
}
```
El código [0] accede al primer elemento del arreglo, como sabras en java partimos contando desde el 0. Para ejecutar este metodo hacemos lo siguiente:

```text
javac Zoo.java
java Zoo Bronx Zoo
```

La salida es la siguiente:

```text
Bronx
Zoo
```
muy fácil de entender el por que esta salida.

Si necesitas colocar una frase (espacios entre palabras) tienes que mandar los argumentos entre comillas dobles.
```text
javac Zoo.java
java Zoo "San Diego" Zoo
```
Ahora la salida aparece con espacios
```text
San Diego
Zoo
```
Entonces, ¿ que pasaria si le pasamos solo un argumento ?. 
```text
javac Zoo.java
java Zoo Zoo
```
Al leer args[0] java puede obtener 'Zoo' pero entrara en panico cuando intente leer args[1]. ¿Que hago si no hay argumento en la posición 1?. Java
lanzara una exception que te dira que no tiene idea de que hacer con el argumento de la posición 1.
```text
Zoo
Exception in thread "main" java.lang.ArrayIndexOutOfBoundsException:
Index 1 out of bounds for length 1
at Zoo.main(Zoo.java:4)
```
## Single file source code

Si estas cansado de tipear javac y java cada vez que tienes que compilar para probar un código, aqui tenemos un
shortcut para ti. Puedes intentar algo como esto:
```text
java Zoo.java Bronx zoo
```
Como vez, es mas corto de realizar y cumple la misma funcion que hacerlos por separado, no creo que necesite mas explicación.
Esta caracteristica es llamada 'launching single file source code' y es util para testing o para pequeños programas.









