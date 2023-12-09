## Enunciado
Determinar si el valor de una variable x es par o impar. Nos ayudamos para averiguarlo
del operador %. Un número es par si es divisible entre 2, es decir, si al dividirlo entre
dos obtenemos de resto 0.

## Solución

 
```java
public class Ejercicio_1 {
    public static void main(String[] args) { 
        int x = 2;

        if (x % == 0) {
            System.out.println("El número es par");
        } else {
            System.out.println("El número es impar");
        }
    
    }
}
```


## Razonmaiento

Podemos saber si un número es par simplemente basandonos en el resultado del módulo (resto de la división) En caso de ser 0, es par sino impar.