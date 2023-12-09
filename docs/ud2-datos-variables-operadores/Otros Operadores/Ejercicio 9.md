## Enunciado
De forma similar al ejemplo comprueba el funcionamiento de %=, >>= y |= produciendo la siguiente salida

Siendo el valor incial de I = 10.

| Valor de I | Operador |
| :--: | :--: |
|  1   | %= |
| 0 | >>= |
|1 | \|= |
## Solución
 
```java
public class Ejercicio_9 {
    public static void main(String[] args) { 
    int i = 10;
		
		System.out.println("Valor inicial de i: " + i);
		System.out.println("Valor de i tras i%=3: " + (i%=3));
		System.out.println("Valor de i tras i>>=1: " + (i>>=1));
		System.out.println("Valor de i tras i|=1: " + (i|=1));
    }
}
```

## Razonmaiento