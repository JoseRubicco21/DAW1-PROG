## Enunciado

Calcula la IMC de una persona cuyo peso y altura los tenemos almacenados en sus respectivas variables. La formula que calcula el IMC debes investigar cual es. Recoger los dos datos por teclado. A continuación os aparece un ejemplo de salida de vuestro programa:

## Solución

 
```java
public class Ejercicio_5 {
    public static void main(String[] args) { 
    float weight, height;
		
		Scanner sc = new Scanner(System.in);
		
		System.out.println("Introduzca su peso:");
		weight = sc.nextFloat();

		System.out.println("Introduzca su altura:");
		height = sc.nextFloat();
		
		System.out.println("IMC: " + (weight / Math.pow(height, 2)));
		
		System.out.println("Tabla IMC\nDelgado: < 18.5\nNormal: entre 18.5 y 24.9\nSobrepeso: entre 25 y 29.9\nObeso: 30 o más");
		sc.close();
    }
}
```

