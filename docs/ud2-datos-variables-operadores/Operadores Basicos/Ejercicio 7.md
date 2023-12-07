## Enunciado
Dadas las variables tipo int con valores A=5, B=3, C=12. Indicar si la evaluación de estas
expresiones daría como resultado verdadero o falso:

- A >3
- B !=C
- A*B==3
- C/B== -4
- (A+B == 8) && (A-B ==2)
- (A+B == 8) || (A-B == 6) 

## Solución

 
```java
public class Ejercicio_7 {
    public static void main(String[] args) { 
    int a = 5;
    int b = 3;
    int c = 12;

    System.out.println(a > 3); // true
    System.out.println(b != c); // true
    System.out.println(a*b == 3); // false
    System.out.println(c/b == -4); // false
    System.out.println((a+b == 8) && (a-b == 2)); // true
    System.out.println((a+b == 8) || (a-b == 6)); // true
    }
}
```