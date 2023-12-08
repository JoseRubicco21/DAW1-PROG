## Enunciado
El siguiente ejemplo imprime una tabla de verdad del operador &&. Observa que se ha utilizado el carácter tabulador para practicar el concepto de secuencia de escape aunque podríamos conseguir el columnado simplemente usando espacios en blanco. Realiza en el mismo programa la tabla de || (or logico).


## Solución

 
```java
public class Ejercicio_6 {
    public static void main(String[] args) { 
    System.out.println("falso\t||\tfalso\t=\t" + (false || false));
    System.out.println("falso\t||\tverdadero\t=\t" + (false || true));
    System.out.println("verdadero\t||\tfalso\t=\t" + (true || false));
    System.out.println("verdadero\t||\verdadero\t=\t" + (true || true));
    }
}
```

