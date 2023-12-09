## Enunciado
Con la clase Persona
```java
public class Persona {
    String nombre;
    int edad;
}
```
Crea un proyecto DemoPersona, que contiene dos clases:
- la clase persona
- Una clase DemoPersona que contiene un main() que usa la clase Persona.

DemoPersona hace lo siguiente:
- crea un objeto persona con nombre “Ana” y edad 3 y asigna este objeto a
la variable referencia p1.
8
- Crea un objeto persona con nombre “David” y edad 5 y asigna este objeto
a la variable referencia p2.
- Imprime los nombres de los objetos persona asociados a p1 y p2 para
comprobar que se hizo correctamente.

## Solución

### Clase persona

```java
public class Persona {

	String name;
	int age;

	@Override
	public String toString(){
		return "Nombre: " + name + "\nAños: " + age;
	};
}
```

### Clase DemoPersona
 
```java
public class DemoPersona {
    public static void main(String[] args) { 
    	Persona p1 = new Persona();	
		
		p1.name = "Ana";
		p1.age = 3;
		
		Persona p2 = new Persona();
		
		p2.name = "David";
		p2.age = 5;
		
		System.out.println(p1.toString()+"\n");
		System.out.println(p2.toString());
    }
}
```




