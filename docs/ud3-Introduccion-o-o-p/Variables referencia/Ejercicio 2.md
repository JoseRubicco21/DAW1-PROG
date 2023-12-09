## Enunciado
Sobre el ejercicio anterior, crea un proyecto IntercambioReferencias que
intercambia los objetos a los que apuntan p1 y p2, de forma que p1 apunte a la
persona de nombre David y p2 a la persona de nombre Ana. Utiliza una variable
referencia intermedia temp para hacer el intercambio. No se trata de cambiar los
valores de los objetos, si no de intercambiar las parejas objetos y variables referencias.


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
		
		// Auxiliar variable is created
		Persona personaTemporal;
		// personaTemporal has p1 reference
		personaTemporal = p1;
		// p1 has p2 reference
		p1 = p2;
		// p2 gets overriden with personaTemporal reference wich is p1
		p2 =  personaTemporal;
		
		System.out.println(p1.toString()+"\n");
		System.out.println(p2.toString());
    }
}
```

