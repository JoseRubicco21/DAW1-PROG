## Enunciado
Con lo visto con printf() mejora la visualización del [Ejercicio 4 ejercicio 4 de Ejercicios Básicos II](../Ejercicios%20Basicos%20II/Ejercicio%204.md)

## Solución
 
```java
import java.util.Scanner;
public class Ejercicio_3 {
    public static void main(String[] args) { 
    	
		Scanner sc = new Scanner(System.in);
		
		double initialEuros, interestRate, years, total, revenue;
		
		System.out.println("Introduzca el capital Inicial: ");
		initialEuros = sc.nextFloat();
		
		System.out.println("Introduzca la tasa de interes: ");
		interestRate = sc.nextFloat();
		
		System.out.println("Introduzca el número de años: ");
		years = sc.nextFloat();
		
		total = initialEuros * Math.pow(1 + (interestRate/100), years);
		revenue = total - initialEuros;
		
		String tableFormat = "* %-20s %23.2f %s * %n";
		
		System.out.printf("Capital Inicial (\u20AC): %.2f %n", initialEuros);
		System.out.printf("Interés anual (%%): %.2f %n", interestRate);
		System.out.printf("Años (a): %.2f %n", years);
		System.out.print("*".repeat(50) + "\n");
		System.out.printf(tableFormat, "Capital inicial: ", initialEuros, "\u20AC");
		System.out.printf(tableFormat, "Interés anual:", interestRate , "%");
		System.out.printf(tableFormat, "Periodo: ", years, "a", "*");
		System.out.printf(tableFormat, "Capital final: ", total, "\u20AC");
		System.out.printf(tableFormat, "Rendimiento: ", revenue, "\u20AC");

		System.out.print("*".repeat(50) + "\n");
		sc.close();	
    }
}
```

:::info Nota sobre el ejercicio
El ejercicio ya contaba con la mejoria en un principio, por ende son el mismo.
:::