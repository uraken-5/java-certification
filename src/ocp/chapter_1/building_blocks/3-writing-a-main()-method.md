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

