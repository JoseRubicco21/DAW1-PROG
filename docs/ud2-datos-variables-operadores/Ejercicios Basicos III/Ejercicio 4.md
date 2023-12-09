## Enunciado

Prueba esta instrucción: System.out.println("*".repeat(6)); ¿Qué hace?

Realiza un programa que dibuje lo siguiente

```
----------------------------------------------------------------------
|Descripción     |Precio          |Cantidad        |Subtotal         |
----------------------------------------------------------------------
----------------------------------------------------------------------
                       **Gracias por su compra** 

```
## Solución

 
```java
public class Ejercicio_4 {
    public static void main(String[] args) { 
    String tableFormat = "|%-16s|%-16s|%-16s|%-16s |%n";
		
		System.out.printf("%s%n", "-".repeat(70));
		System.out.printf(tableFormat, "Descripción", "Precio", "Cantidad", "Subtotal");
		System.out.printf("%s%n", "-".repeat(70));
		System.out.printf("%s%n", "-".repeat(70));
		System.out.printf("%48s %n", "**Gracias por su compra**");
    }
}
```

## Razonamiento

La instrucción `System.out.println("*".repeat(6));` repite el caracter `*` 6 veces. Es un método de un objeto de la clase *String*.

:::info Variable tableFormat
La variable table format se puede no usar, y poner todo en el mismo `System.out.printf()` pero considero que de dicha forma el código queda mucho mas "Limpio"
:::
