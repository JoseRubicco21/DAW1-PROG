## Enunciado
Tenemos almacenados dos números enteros almacenados en variables x e y. Queremos
averiguar si x es múltiplo de y. De nuevo, ayúdate del operador módulo.

## Solución

 
```java
public class Ejercicio_2 {
    public static void main(String[] args) { 
    int x = 4;
    int y = 2;

    if(x % y == 0){
        System.out.println("x es multiplo de y");
        } else {
        System.out.println("x no es multiplo de y");
    }

    }
}
```