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
- 'static' vincula el metodo en cuestion con la clase que la contiene. Esto significa que puedes llamar al método sin necesidad de crear un objeto

