## Enunciado
 Escribe un programa usando printf() que calcule el total de una factura a partir de la base imponible (precio sin IVA). La base imponible estará almacenada en una variable.

## Solución
 
```java
import java.util.Scanner;

public class Ejercicio_1 {
    public static void main(String[] args) { 
           	Scanner sc = new Scanner(System.in);
			
			float baseImponible;
			
			System.out.printf("Introduce la base imponible:%n");
			baseImponible = sc.nextFloat();
			
			float iva =  baseImponible - baseImponible/1.21f;
			System.out.printf("%s %n", "-".repeat(35));
			System.out.printf("Base imponible: %15.2f %n", baseImponible);
			System.out.printf("Iva %26.2f %n", iva);
			System.out.printf("%s %n", "-".repeat(35));
			System.out.printf("Total %25.2f", baseImponible + iva);
			sc.close();
    }
}
```
