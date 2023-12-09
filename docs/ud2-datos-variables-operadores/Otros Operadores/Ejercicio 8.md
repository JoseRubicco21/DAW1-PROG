## Enunciado
Comprobar con números visualizados en base 2 la diferencia entre multiplicación lógica
y aritmética para dos variables enteras x e y.
## Solución
 
```java
public class Ejercicio_8 {
    public static void main(String[] args) { 
    	int x = 4, y = 5;
		
		System.out.println("Multiplicación lógica " +  Integer.toBinaryString(x) + " & "+  Integer.toBinaryString(y) + " : "  + Integer.toBinaryString(x&y));
        
		System.out.println("Multiplicación aritmética " + Integer.toBinaryString(x) + " & " + Integer.toBinaryString(y) + " : " + Integer.toBinaryString(x*y));
    }
}
```

## Razonmaiento