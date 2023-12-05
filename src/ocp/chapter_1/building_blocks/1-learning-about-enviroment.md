# Objetivos del exámen cubiertos en este capitulo
---
Manejar valores date, time, numeric y boolean.
- Uso de primitivos y de clases de envoltorios (wrapper) incluyendo el api MATH, parentesis, conversión de tipos, y casteos para evaluar expresiones booleanas y aritmeticas.

Utiilzar enfoque orientado a objetos.
- Declarar e instanciar objetos java incluyendo objetos de clases internas, y explicar el ciclo de vida de los objetos incluyendo creación, reasignacion de referencias y recolector de basura.
- Entender el scope de las variables, usar inferencia de tipos locales, aplicar encapsulación e inmutabilidad de objetos.

---
Nota personal: En la primera parte, se da la bienvenida al libro de estudio para la certificación. Para resumir te indica que este libro no es un curso de java y asume que sabemos java y si no, 
te manda a leer un libro para aprender java.
Nota personal 2: Perdonen el spanglish XD

Luego te dice en la cara que no te apures con la frase 'antes de correr, aprende a caminar'. En fin, en este capitulo
se veran:
- lo básico de los java packages
- clases
- variables
- tipos de datos

Pero no solo a usarlos, el libro te hara entender lo que hay por 'debajo' de cada caracteristica del lenguaje, asi que básicamente te dice que da igual que trabajes por varios años con java haciendo codigo, de todas formas fallaras este exámen por que no conoces las profundidades del mismo.

Por ejemplo, que hay de malo en esta declaración?

```java
public class MiClase {
    public static void main(String[] args) {
        int 3dMap;
        System.out.println(3dMap);
    }
}
```
ves? aparentemente nada, pero si hay un problema o mejor dicho se esta rompiendo una regla (y si sabes, eres un crack, pero igual debes estudiar mas).
DICHO ESTO, COMENCEMOS !
---

# Learning about the enviroment

Llegas al trabajo, descargas un jdk y lo instalas para luego configurar tu ide favorito, y luego haces tu holaMundo.java para deleitarnos con tu genialidad. Esto por varios años asi que en teoria sabes java ¿cierto?. Si pero para esta certificación 
tambien debes conocer las caracteristicas y elementos del entorno, cosas que quizas pasas de largo por que
simplemente 'son asi'. Esta sección habla sobre esto.

Componentes principales de java

El Java Developed Kit contiene el software minimo para poder programar en este lenguaje. 
- javac   : Convierte los .java en código bytecode .class
- java    : Ejecuta el programa
- jar     : Empaqueta el codigo.
- javadoc : Genera documentación.

El comando javac genera instrucciones en un formato especial llamado bytecode el cual puede correr el comando java. Entonces jaa
inicia la maquina virtual (el famoso JVM) antes de ejecutar el codigo.

<div style="background-color: #000; color: #ff0; padding: 10px; border-radius: 5px;">

Esto es importante: Cada 6 meses se libera una nueva version de java. Java 17 se libero en septiembre del 2021. Esto significa que es probable que cuando descargues el jdk veas una versiòn muy adelantada a la 17 pero te recomiendo que sigas estudiando con el jdk 17.
Las reglas y el comportamiento podrian cambiar con las versiones recientes y mas aun, interpretar como incorrecta algunas preguntas si es que usas una version mas reciente.

### Comprueba tu versiòn de java
```bash
javac -version
java -version
```
Ambos comandos deberian indicar la version 17.

</div>





