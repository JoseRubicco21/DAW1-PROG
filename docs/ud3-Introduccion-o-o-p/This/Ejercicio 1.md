## Enunciado
Prueba la clase anterior Circulo desde el main() . Debes de crear dos círculos, comparar su
radio e imprimir las coordenadas del círculo devuelto por elMayor()

```java

class Circulo{
    int coordenadaX;
    int coordenadaY;
    int radio;

    Circulo elMayor(Circulo c){
        if(radio>c.radio){ //o también if(this.radio>c.radio)
        return this;
        } else {
        return c;
        }
    }

    @Override 

    public String toString(){
        return "coordenadaX = " + coordenadaX, + "\ncoordenadaY = " + coordenadaY + "\nradio = " + radio;
    }

}
```
## Solución

 
```java
public class Ejercicio_1 {
    public static void main(String[] args) { 
    
    Circulo c1 = new Circulo();
    Circulo c2 = new Circulo();

    c1.radio = 2;
    c1.coordenadaX = 10;
    c1.coordenadaY = 10;
    
    c2.coordenadaX = 10;
    c2.coordenadaY = 10;
    c2.radio = 4;

    System.out.println(c1.elMayor(c2).coordenadaX, c1.elMayor(c2).coordenadaY); // 
    
    }
}
```