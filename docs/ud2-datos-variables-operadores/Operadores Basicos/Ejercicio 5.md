## Enunciado
int z = x++%5;
produce un valor de Z diferente que la instrucción
int z = ++x%5;

## Solución
 
```java
public class Ejercicio_5 {
    public static void main(String[] args) { 
    int x = 10;
    int x2 = 10;
    int y = x++%5;
    System.out.println("x++%5: " + y);
    int z = ++x2%5;
    System.out.println("++x%5: " + z);
    }
}
```

## Razonmaiento

El código se ejecuta de la siguiente manera:

```mermaid
flowchart LR
    p[println]
    p2[println]
    id1[y = 10%5 == 0]
    id2[x = x + 1] 
    
    id1 --> p --> id2

    id3[x2 = x2 + 1]
    id4[z = 11%5 == 1]
    id3 --> id4 --> p2
```

Por lo tanto podemos asumir que sufijo se ejecuta siempre después de un *"Punto de ejecución"* como puede ser un System.out.println.

