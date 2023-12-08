## Enunciado
Escribe un programa Java que realice lo siguiente: declarar dos variables X e Y de tipo int, dos variables N y M de tipo double y asigna a cada una un valor. A continuación muestra por pantalla:
El valor de cada variable.
La suma X + Y
La diferencia X – Y
El producto X * Y
El cociente X / Y
El resto X % Y
La suma N + M
La diferencia N – M
El producto N * M
El cociente N / M
El resto N % M
La suma X + N
El cociente Y / M
El resto Y % M
El doble de cada variable
La suma de todas las variables
El producto de todas las variables
Si por ejemplo le hemos dado a X el valor 1, a Y el valor 2, a M el valor 3.2 y a N el valor 4.7 se debe mostrar por pantalla:

Variable X = 1
Variable Y = 2
Variable M = 3.2
Variable N = 4.7
1 + 2 = 3
1 - 2 = -1
1 * 2 = 2
1 / 2 = 0
1 % 2 = 1
4.7 + 3.2 = 7.9
4.7 - 3.2 = 1.5
4.7 * 3.2 = 15.040000000000001
4.7 / 3.2 = 1.46875
4.7 % 3.2 = 1.5
1 + 4.7 = 5.7
2 / 3.2 = 0.625
2 % 3.2 = 2.0
Variable X = 1 el doble es 2
Variable Y = 2 el doble es 4
Variable M = 3.2 el doble es 6.4
Variable N = 4.7 el doble es 9.4
1 + 2 + 4.7 + 3.2 = 10.9
1 * 2 * 4.7 * 3.2 = 30.080000000000002

## Solución

 
```java
public class Ejercicio_2 {
    public static void main(String[] args) { 
    int x = 1;
    int y = 2;
    double n = 3.2;
    double m = 4.7;

    
    System.out.println("Variable X: " + x);
    System.out.println("Variable Y: " + y);
    System.out.println("Variable M: " + n);
    System.out.println("Variable N: " + m);
    System.out.println("La suma de X + Y: " + (x+y));
    System.out.println("La resta de X - Y: " + (x-y));
    System.out.println("La diferencia de N - M: " + (n-m));
    System.out.println("El producto de N * M: " + (n*m));
    System.out.println("El cociente de N / M: " + (n/n));
    System.out.println("El resto N % M: " + (n%m));
    System.out.println("La suma de X + N: " + (x+n));
    System.out.println("El cociente de Y / N: " + (y/n));
    System.out.println("El resto de Y % M: " + (y%m));
    System.out.println("El doble de X, Y, N, M: " + (x*2) + " " + (y*2) + " " + (n*2) + " " + (m*2));
    System.out.println("Suma de todas las variables: " + (x+y+n+m));
    System.out.println("Producto de todas las variables: " + (x*y*n*m));

    }
}
```