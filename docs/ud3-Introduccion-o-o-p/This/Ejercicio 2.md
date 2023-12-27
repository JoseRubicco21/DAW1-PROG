## Enunciado
Reescribe el ejercicio anterior pero ahora utilizando operador condicional en lugar de
if y un constructor de forma que al crear el círculo ya se indique sus coordenadas y el
radio.

## Solución
### Clase Circulo

```java
class Circulo{
    
    int coordenadaX;
    int coordenadaY;
    int radio;

    Circulo(){

    }

    Circulo(int coordenadaX, int coordenadaY, int radio){
        this.coordenadaX = coordenadaX;
        this.coordenadaY = coordenadaY
        this.radio = radio
    }

    Circulo elMayor(Circulo c){
        this.radio < c.radio ? return c : return this;
    }

    @Override 

    public String toString(){
        return "coordenadaX = " + coordenadaX, + "\ncoordenadaY = " + coordenadaY + "\nradio = " + radio;
    }

}
```
### Main
 
```java
public class ClassName {
    public static void main(String[] args) { 
    
    Circulo c1 = new Circulo(10,10,2);
    Circulo c2 = new Circulo(20,20,4);

    Circulo cmayor = c1.elMayor(c2);

    System.out.println(cmayor);
    }
}
```
