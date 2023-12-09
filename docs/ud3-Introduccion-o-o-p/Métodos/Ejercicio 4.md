## Enunciado
Crea OtraClase:

```mermaid
classDiagram
    OtraClase {
        - char car
        - int num
        - OtraClase(char c, int n)
        - sumar1()
    }
```

## Solución

```java
public class OtraClase{
    private char car;
    private int num;

    OtraClase(char c, int n) {
        car = c;
        num = n;
    }

    public void sumar1(){
        num += 1;
    }
}
```
