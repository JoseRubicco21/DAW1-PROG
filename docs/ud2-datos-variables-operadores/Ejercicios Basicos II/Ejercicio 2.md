## Enunciado
Escribe un programa que reciba de la entrada estándar una temperatura en grados Celsius. A continuación, devolverá dicho valor convertido a grados Fahrenheit

La relación de conversión es la siguiente: F = 1.8*C + 32

Los valores mostrados se redondearán a un decimal

El programa debe generar la salida manteniendo el mismo formato del ejemplo mostrado

Entrada: 35

Salida: 

35,0 ºC son 95,0 ºF
## Solución
 
```java
import java.util.Scanner;

public class Ejercicio_2 {
    public static void main(String[] args) { 
        float temp;

        Scanner sc = new Scanner(System.in);

        System.out.println("Introduce la temperatura en grado celcius:");

        temp = sc.nextFloat();

        System.out.println(temp + "ºC son " + (1.8 * temp + 32) + "ºF");
    }
}
```


