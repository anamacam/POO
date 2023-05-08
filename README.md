# POO
La **POO** es un paradigma que se utiliza fundamentalmente para brindar soluciones. Es una forma de programar cuya idea principal es emular el mundo real a través de los objetos. 
> "Un objeto en POO representa alguna entidad de la vida real, es decir, alguno de los objetos que pertenecen al negocio con que estamos trabajando o al problema con el que nos estamos enfrentando, y con los que podemos interactuar.."
> [Wikipedia](https://es.wikipedia.org/wiki/Objeto_(programaci%C3%B3n).
> Los objetos teiene dos principales: 
  - *Un estado* que obedece a unas características como: nombre, raza y color.
  - *Un comportamiento* como: ladrar, comer, dormir.

## Elementos básicos del POO:

1. *Clases:*  Se utilizan para representar las entidades o conceptos como los sustantivos en el lenguaje. Cada Clase es un conjunto de variables y metodos para operar con dichos datos _el comportamiento_.
> Una clase agrupa Estado (atibutos) y comportamientos(métodos) de los objetos.

2. *Métodos:* Es una subrutina o serie de sentencias para llevar a cabo una acción que retorna una salida o valor.

```java
public class Animal
{
    private String raza;
    private String nombre;
    private int edad;

    public Animal(String nuevoNombre)
    {
        nombre = nuevoNombre; //Se le da un nombre al animal
    }

    //Método para obtener la edad del animal
    public int getEdad()
    {
        return edad;
    }

    //Método para establecer la edad del animal
    public void setEdad(int nuevaEdad)
    {
        edad = nuevaEdad;
    }

    //Método para obtener el nombre del animal
    public String getNombre()
    {
        return nombre;
    }
}
```
3. *Herencia:* es un mecanismo que permite reutilizar o extender comportamientos definidos en otras clases compartiendo métodos y datos.

 - Superclases y Subclases
 
El concepto de herencia conduce a una estructura jerárquica o estructura de árbol, esto significa que las realciones de clases deben ajustarse a dicha estructura. Cada Calse tiene una clase padre y son conocidas como *superclases* y las clases hijas se les denomina *subclases*.
> las _superclase_ pueden tener un sinnúmero de subclases.
> 
> Una _subclase_ solo puede tener una superclase.

```mermaid
         classDiagram
    Animal <|-- Duck
    Animal <|-- Fish
    Animal <|-- Zebra
    Animal : +int age
    Animal : +String gender
    Animal: +isMammal()
    Animal: +mate()
    class Duck{
      +String beakColor
      +swim()
      +quack()
    }
    class Fish{
      -int sizeInFeet
      -canEat()
    }
    class Zebra{
      +bool is_wild
      +run()
    }

```

4. *Objetos* : como se explicó al inicio de este artículo, los objetos tienen un *estado* determinado por una o más varialbles y un *comportamiento* que obedece a los métodos. El comportamiento es publico y el estado es privado.

```java
public class Aclaracion
{
    private int atributo1;
    private int atributo2;
    private String atributo3;

    //Declaramos un constructor
    public Aclaracion(int attr1, int attr2, String attr3)
    {
        atributo1 = attr1;
        atributo2 = attr2;
        atributo3 = attr3;
    }

    public static void main(String[] args)
    {
        Aclaracion ac = new Aclaracion(5, 10, "x");//Creamos un objeto enviando parámetros al constructor

        System.out.println(ac.atributo1 + ", " + ac.atributo2 + ", " +ac.atributo3);//Mostramos el valor de los atributos
        //Imprime '5, 10, x'
    }
}
```
5. *Eventos:* son acciones que se generan en aplicaciones gráficas ocasionados por los usuarios al oprimir un botón, cambiar el color del texto o dar clic en un texto.

![evento](https://image1.slideserve.com/3553213/generaci-n-de-eventos1-l.jpg)

*Tipos de eventos:*

- ActionEvent : generado por activación de componentes
- AdjustmentEvent : generado por  ajuste de  componentes  ajustables como  barras de desplazamiento
- ContainerEvent :  generado  cuando los  componentes  se  agregan  o se quitan  de un contenedor
- FocusEvent : generado cuando un componente entra o sale del foco
- ItemEvent : generado  cuando un artículo  se  selecciona  de una lista,  opción, o caja de  chequeo
- KeyEvent : generado por actividad del teclado
- MouseEvent : generado por actividad del ratón
- PaintEvent : generado cuando un componente se pinta
- TextEvent : generado cuando un componente del texto se modifica
- WindowEvent : generado por actividad de la ventana (como cerrar, abrir, minimizar)


    



