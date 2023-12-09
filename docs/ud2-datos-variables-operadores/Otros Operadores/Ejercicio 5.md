## Enunciado
Tenemos almacenados dos números enteros almacenados en variables x e y. Queremos
averiguar si x es múltiplo de y. De nuevo, ayúdate del operador módulo.

## Solución
 
```java
public class Ejercicio_5 {
    public static void main(String[] args) { 
    int x = 4;
    int y = 2;

    System.out.println((x % y == 0) ? "x es multiplo de y" : "x no es multiplo de y")
    }
}
```