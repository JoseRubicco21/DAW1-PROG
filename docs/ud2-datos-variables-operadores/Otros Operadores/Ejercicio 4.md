## Enunciado
Determinar si el valor de una variable x es par o impar. Nos ayudamos para averiguarlo
del operador %. Un número es par si es divisible entre 2, es decir, si al dividirlo entre
dos obtenemos de resto 0.

## Solución

 
```java
public class Ejercicio_4 {
    public static void main(String[] args) { 
    int x = 2;

    System.out.println((x % 2 == 0) ? "El número es par" : "El numero es impar");
    }
}
```


## Razonmaiento

Podemos saber si un número es par simplemente basandonos en el resultado del módulo (resto de la división) En caso de ser 0, es par sino impar.