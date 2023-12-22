# Understanding the class structure

En un programa java, las clases son las estructuras bàsicas de construcciòn. Cuando creas una clase estas definiendo todas las partes y caracteristicas de una parte de la aplicaciòn. 
Si si una clase es básica y quieres conocer otros temas pero tranquilo, mas adelante se veran las interfaces, los records y los enums.

&emsp;&emsp; 
para usar la mayoria de las clases debes crear objetos. Un objeto es una instancia en tiempo de ejecuciòn de una clase en memoria. Un objeto es conocido como una
instancia o dicho de otra forma, la representaciòn de una clase. Todos los objetos de las diferentes clases de un programa son conocidos como el estado del programa. 
Tambien es importante saber que una referencia es una variable que apunta a un objeto. </br>

&emsp;&emsp;
En las siguientes secciones, veremos los campos, metodos y comentarios (fields, methods and comments). Tambien exploraremos la relaciòn entre clases y archivos.

## I. Fields and Methods
Las clases java tienen dos elementos primarios, los metodos usualmente llamados funciones o procedimientos en otros lenguajes y los campos o fields que son nada mas y nada menos que las variables. Todos juntos forman a los miembros de una clase.
Las variables mantienen el estado de un programa y los metodos operan sobre estos estados. 

Una clase java simple luce asi:

```java
1:  public class Animal {
2:  }
```
Importante es saber que java le da el nombre de 'keywords' a las palabras que tienen un significado para el lenguaje
como por ejemplo la palabra 'class' o la palabra 'public'. 

Hagamos la clase Animal mas interesante:

```java
1:  public class Animal {
2:      String name;
3:      public String getName() {
4:          return name;
5:      }
6:      public void setName(String newName) {
7:          name = newName;
8:      }
9:  }
```
Que tenemos aqui. En la linea 2 definimos una variable de nombre 'name' de tipo 'String'.
String es un tipo de dato que nos permite meter en una variable texto como por ejemplo "yo soy un texto". 
String es una clase proveida por el lenguaje.

## Metodos
Las lineas 3 y 5 muestran la definición de un método el cual es una operación que puede ser llamada.
En las líneas 6-8 hay otro método. Este tiene un tipo de retorno especial llamado void. 
La palabra clave void significa que no se devuelve ningún valor. 
Este método requiere que se le suministre información desde el método que lo llama.
esta información se llama parámetro. El método setName() tiene un parámetro llamado newName, 
y es de tipo String. Esto significa que el llamador debe pasar un parámetro String y no esperar 
que se devuelva nada.

El nombre del mètodo y los tipos de paràmetros se conocen como la 'firma' del mètodo. ¿Puedes identificar la firma de este mètodo?

```java
public int numberVisitors(int month) {
    return 10;
}
```
El nombre del mètodo es numberVisitors, y tenemos un parametro de nombre month que es de tipo Int. Entonces la firma del
mètodo es numberVisitors(int).

## Comentarios
Otra parte importante del código son los comentarios. Los comentarios no son ejecutados por lo que puedes colocarlos
en distintos lugares del código. Los comentarios hacen tu código mas entendible y facil de leer. Existen 3 tipos de comentarios
en java. El primer tipo de comentario es conocido como 'single line comment'

```java
//this is a single line comment
```
un single line comment inicia con doble slash. El compilador ignora todo lo que hay despues de los doble slash.
Luego tenemos los multiple-line-comment

```java
/*
        this is a multiple-line-comment
 */
```
Este tipo de comentario tambien es conocido como 'comentario multilinea'. Incluye todo desde el simbolo /* y el fin */. Finalmente tenemos los
java-docs-comments.

```java
/**
 * Javadoc multiple-line comment
 * @author Balto el terrible
 */
```
Este tipo es similar al comentario multilinea, salvo que comienza con /**. Esta sintaxis especial le
indica a la herramienta javadoc que ponga atención al contenido que aqui se encuentra.




