# POO
La **POO** es un paradigma que se utiliza fundamentalmente para brindar soluciones. Es una forma de programar cuya idea principal es emular el mundo real a través de los objetos. 
> "Un objeto en POO representa alguna entidad de la vida real, es decir, alguno de los objetos que pertenecen al negocio con que estamos trabajando o al problema con el que nos estamos enfrentando, y con los que podemos interactuar.."
> [Wikipedia](https://es.wikipedia.org/wiki/Objeto_(programaci%C3%B3n).
> Los objetos teiene dos principales: 
  - *Un estado* que obedece a unas características como: nombre, raza y color.
  - *Un comportamiento* como: ladrar, comer, dormir.

## Elementos básicos del POO:

1. *Clases:*  Se utilizan para representar las entidades o conceptos como los sustantivos en el lenguaje. Cada Clase es un conjunto de variables y metodos para operar con dichos datos _el comportamiento_- 
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
El concepto de herencia conduce a una estructura jerárquica o estructura de árbol, esto significa que las realciones de clases deben ajustarse a dicha estructura. Cada Calse tiene una clase padre y son conocidas como *superclases* y las clases hijas se les denomina *subclases*.
> las _superclase_ pueden tener un sinnúmero de subclases.
> 
> Una _subclase_ solo puede tener una superclase.





