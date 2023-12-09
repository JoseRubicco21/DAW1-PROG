## Enunciado
Si el valor de x al cuadrado es mayor que 100 aumenta el valor de la variable y en 1 y
lo imprime, en caso contrario que lo decremente en 1. 

## Solución

 
```java
public class Ejercicio_6 {
    public static void main(String[] args) { 
    // Code here
    int x = 25;

    System.out.println((x*x == 100) ? x-- : x++);
    }
}
```