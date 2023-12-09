## Enunciado
Escribe un programa que reciba por la entrada estándar una cantidad inicial en euros, una tasa de interés y un número de años (en ese orden). El programa mostrará por pantalla cuál será el capital resultante transcurridos el número de años indicado. La salida debe mostrar el formato del ejemplo de ejecución adjunto

NOTA: dado un capital inicial C, el capital resultante a un interés del x por cien durante n años es:

$
c * ( 1 + \frac{x}{100} )^n
$
## Solución

```java
import java.util.Scanner;

public class Ejercicio_4 {
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
