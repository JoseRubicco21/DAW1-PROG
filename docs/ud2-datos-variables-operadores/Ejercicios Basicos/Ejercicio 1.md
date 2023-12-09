## Enunciado
Escribe un programa Java que realice lo siguiente: declarar una variable N de tipo int, una variable A de tipo double y una variable C de tipo char y asigna a cada una un valor. A continuación muestra por pantalla:
El valor de cada variable.
La suma de N + A
La diferencia de A - N
El valor numérico correspondiente al carácter que contiene la variable C.
Si por ejemplo le hemos dado a N el valor 5, a A el valor 4.56 y a C el valor ‘a’, se debe mostrar por pantalla:
Variable N = 5
Variable A = 4.56
Variable C = a
5 + 4.56 = 9.559999999999999
4.56 - 5 = -0.4400000000000004
Valor numérico del carácter a = 97

## Solución
 
```java
public class Ejercicio_1 {
    public static void main(String[] args) { 
    int n = 1;
    double a = 2;
    char c = 'a';


    System.out.println("Valor de la variable n: " + n);
    System.out.println("Valor de la variable a: "+ a);
    System.out.println("Valor de la variable c: " + c);
    System.out.println("Suma de N + A " + (n+a));
    System.out.println("Diferencia entre N y A " + (n-a));
    System.out.println("Valor númerico del caracter: " + int(c));

    }
}
```