## Enunciado
Escribe un programa que solicite la nota de cada una de las 3 evaluaciones (pueden contener decimales).

El programa mostrará la nota final (media de la nota de las evaluaciones) de dos maneras: redondeada a dos decimales y redondeada al entero más próximo. También debe indicar si se ha aprobado o no.

## Solución

 
```java
import java.util.Scanner;

public class Ejercicio_7 {
    public static void main(String[] args) { 
    	    Scanner sc = new Scanner(System.in);
			
			float primeraEvaluacion;
			float segundaEvaluacion;
			float terceraEvaluacion;
			float media;
			
			System.out.println("Introduzca la nota de la primera evaluación");
			primeraEvaluacion = sc.nextFloat();
			System.out.println("Introduzca la nota de la segunda evaluación");
			segundaEvaluacion = sc.nextFloat();
			System.out.println("Introduzca la nota de la tercera evaluación");
			terceraEvaluacion = sc.nextFloat();
			
			media = (primeraEvaluacion + segundaEvaluacion + terceraEvaluacion)/3;
			
			System.out.printf("La media total es %.2f %n", media);
			System.out.println((media > 5) ?  "Aprobado" : "Reprobado");
			
			sc.close();
    }
}
```

