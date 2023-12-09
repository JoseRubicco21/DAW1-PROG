## Enunciado
Escribe un programa que reciba de la entrada estándar un número de días, horas, minutos y segundos (en ese orden) y calcule el número total de segundos

El programa debe generar la salida manteniendo el mismo formato del ejemplo mostrado:

Entrada:
365
5
48
45
Salida:
365 días, 5 horas, 48 minutos y 45 segundos son 31556925 segundos

## Solución
 
```java
public class Ejercicio_1 {
    public static void main(String[] args) { 
    long dias, horas, minutos, segundos, total;
		
		Scanner sc = new Scanner(System.in);
		
		System.out.println("Itroduzca un número de dias, horas, minutos y segundos (en ese orden) para calcular.\nDias: ");
		
		dias = sc.nextLong();
		
		System.out.println("Horas: ");
		 
		horas = sc.nextLong();
		
		System.out.println("Minutos: ");
		
		minutos = sc.nextLong();
		
		System.out.println("Segundos: ");
		
		segundos = sc.nextLong();
		
		total = (dias*86400) + (horas*3600) + (minutos*60) + segundos;
		
		System.out.println(dias + " dias " + horas + " horas " + minutos + " minutos y " + segundos + " segundos son en total: " + total + " segundos");
		
		sc.close();
    }
}
```
