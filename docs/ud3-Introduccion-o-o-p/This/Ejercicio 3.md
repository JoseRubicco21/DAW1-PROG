## Enunciado

Reescribe esta clase de forma que lugar de devolver una referencia al círculo mayor
devuelva una copia del circulo mayor, es decir, otro objeto Circulo distinto(un nuevo
objeto) pero con los mismos valores que el mayor de los dos iniciales.
```java
class Circulo{

    int coordenadaX;
    int coordenadaY;
    int radio;

    Circulo(int x, int y, int r){
        coordenadaX=x;
        coordenadaY=y;
        radio=r;
    }

    Circulo elMayor(Circulo c){
        return this.radio>c.radio?this:c;
    }
}
```

## Solución

```java
class Circulo{
    
    int coordenadaX;
    int coordenadaY;
    int radio;

    Circulo(int x, int y, int r){
        coordenadaX=x;
        coordenadaY=y;
        radio=r;
    }

    Circulo elMayor(Circulo c){
        return this.radio > c.radio ? this.clone() : c.clone();
    }
}
```
## Razonmaiento

Clone es un método que permite el clonado de objetos. Se hereda de la clase `Object`. Es importante hacer uso de este método en vez de hacer algo como lo siguiente:

```java
Circulo elMayor(Circulo c){
        return this.radio > c.radio ? new Circulo(this.coordenadaX, this.coordenadaY, this.radio) : new Circulo(c.coordenadaX, c.coordenadaY, c.radio);
    }
```
Para hacer uso de uno de los fuertes del paradigma orientado a objetos, **la modularidad**. Únicamente no es eso, si no que también con el método clone podemos expresamente restringir el clonado si sobreescribimos el método. Esto es muy útil si necesitamos algo como un *singleton*

:::info Singleton y patrones de diseño

Ahora mismo no es necesario saber que es un singleton, pero basicamente son objetos que solo tienen una instancia en toda la vida de la aplicación. Es un patrón de diseño de software.

:::