## Enunciado
Con la siguiente clase Persona

```java
public class Persona {
    String nombre;
    int edad;
}
```

Crea dos personas p1 y p2. La persona p1 tiene como nombre “yo” y edad 45 años. . p2 tiene
como nombre “tu” y edad 37 años. El programa suma las edades de p1 y p2 y las imprime
por pantalla.

## Solución

 
```java
public class Persona {
    String nombre;
    int edad;
}

public class Unidad2 {
    public static void main(String[] args) { 
    
	 Persona p1 = new Persona();
	 Persona p2 = new Persona();
	 
	 p1.name = "yo";
	 p2.name = "tu";
	 
	 p1.age = 45;
	 p2.age = 37;
	 
	 p1.DNI = "000000000F";
	 p2.DNI = "00000000G";
	 
	 System.out.println("Edades sumadas: " + (p1.age + p2.age));
	 
	 System.out.println("\n"+p1.toString());
	 System.out.println("\n"+p2.toString());
	 
	 p1.calcEdad(p2.age);
	 
    }
}
```

