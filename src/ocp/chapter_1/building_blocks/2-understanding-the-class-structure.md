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



