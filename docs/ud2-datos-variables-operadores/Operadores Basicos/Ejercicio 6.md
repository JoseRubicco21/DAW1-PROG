## Enunciado
Crea un pequeño programa que muestre por pantalla si el dato de una variable está en el
rango de edad 18-40 años (ambos inclusives). Ultiliza el operador condicional (?)
Luego haz una modificación para que acepte el rango anterior o 60-70 años (no inclusives).

## Solución
 
```java
public class Ejercicio_6 {
    public static void main(String[] args) { 
    int n = 20;

    System.out.println(n >= 18 && n <= 40 ? "La variable esta en el rango" : "La variable no esta en el rango");
  
    n = 60;
    System.out.println((n >= 18 && n <= 40) || (n > 60 && n < 70) ? "La variable esta en el rango" : "La variable no esta en el rango");

    }
}
```