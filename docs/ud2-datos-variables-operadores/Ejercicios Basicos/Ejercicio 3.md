## Enunciado
Escribe un programa Java que declare una variable entera N y asígnale un valor. A continuación escribe las instrucciones que realicen los siguientes:
Incrementar N en 77.
Decrementarla en 3.
Duplicar su valor.
Si por ejemplo N = 1 la salida del programa será:
Valor inicial de N = 1
N + 77 = 78
N - 3 = 75
N * 2 = 150

## Solución

 
```java
public class Ejercicio_3 {
    public static void main(String[] args) { 
    int n = 1;

    n += 77; // n = n + 77
    System.out.println("Valor de N: " n);
    n -= 3; // n = n - 3
    System.out.println("Valor de N: " n);
    n *= 2; // n = n * 2
    System.out.println("Valor de N: " n);

    }
}
```

