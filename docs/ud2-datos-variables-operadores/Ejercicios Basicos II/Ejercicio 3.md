## Enunciado
Escribe un programa que reciba el lado menor y mayor de un rectángulo y calcule su área y perímetro 

Los valores mostrados se redondearán a dos decimales

El programa debe generar la salida manteniendo el mismo formato del ejemplo mostrado:

Entrada: 

12,5 3
Salida:

Longitud del primer lado: 12,50

Longitud del segundo lado: 3,00

\====================

Perímetro: 31,00 Área: 37,50

\====================

## Solución

 
```java

import java.util.Scanner;

public class Ejercicio_3 {
    public static void main(String[] args) { 
    	Scanner sc = new Scanner(System.in);
          	Scanner sc = new Scanner(System.in);
			
			System.out.println("Introduce el lado 1 del cuadrado");
			float side = sc.nextFloat();
			System.out.println("Introduce el lado 2 del cuadrado");
	        float sideb = sc.nextFloat();

	        float area = side * sideb;
	        float perim = side*2 + sideb*2;
			
			System.out.println("Longitud del primer lado: " + side);
			System.out.println("Longitud del segundo lado: " + sideb);
	        System.out.println("========================================");
	        System.out.printf("Perimetro: %.2f Area: %.2f %n", area, perim);
	        System.out.println("========================================");
		sc.close();
	}
}
```
