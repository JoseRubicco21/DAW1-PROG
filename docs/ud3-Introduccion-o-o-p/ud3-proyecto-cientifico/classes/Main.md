## Explicación del Main

Este main no posee atributos per se. Sólo tiene un método estático `main()` por ende lo único que realmente hay que explicar aqui es que se esta haciendo:

Primeramente se instancia un Scanner conjunto a varios cientificos y proyectos.

Se imprime por pantalla que se creará un proyecto y se invoca el método `crearProyecto()`.

Se hará lo mismo para un cientifico.

Se invocará el método asignar en el objeto *p3* par asignar el cientifico *c4* en la posicion 3 de *p3*

Durante la ejecución del programa se imprimiran los diferentes proyectos para ver todos sus datos. Curiosamente no aparece `calcularPresupuesto()` por ningún lado pero realmente ya esta sucediendo en el `toString()` de cualquier instancia de la Clase Proyecto.

Finalmente se cierra el Scanner que se uso para pasar como argumento a los métodos `crearProyecto()`, `crearCientifico()`, `crearDireccion()`

## Código Fuente

```java
package proyecto_cientifico;

import java.util.Scanner;

public class Main {

	public static void main(String[] args) {
	
	Scanner sc = new Scanner(System.in);
	
	Cientifico c1 = new Cientifico();
	Cientifico c2 = new Cientifico("Jose", 30);
	Cientifico c3 = new Cientifico("Pedro");
	Cientifico c4 = new Cientifico();
	
	Proyecto p1 = new Proyecto();
	Proyecto p2 = new Proyecto("proyecto 1", 5000.00, 12, deps.MARKETING, c1, c2, c3);
	Proyecto p3 = new Proyecto("proyecto 1", 5000.00, 12, deps.INFORMATICA, c2, c3);
	
	
	// Create by user Input/Output
	System.out.println("*".repeat(24)+"\n* Creación de proyecto *\n"+"*".repeat(24)+"\n");
	p1.crearProyecto(sc);
	
	System.out.println("*".repeat(28)+"\n* Creación de cientifico *\n"+"*".repeat(28)+"\n");
	c4.crearCientifico(sc);
	
	System.out.println("*".repeat(14)+"\n* Proyecto 1 *\n"+"*".repeat(14)+"\n");
	System.out.println(p1.toString());
	System.out.println("*".repeat(14)+"\n* Proyecto 2 *\n"+"*".repeat(14)+"\n");
	System.out.println(p2.toString());
	
	p3.asignar(3, c4);
	System.out.println("*".repeat(14)+"\n* Proyecto 3 *\n"+"*".repeat(14)+"\n");
	System.out.println(p3.toString());
	
	sc.close();
	
	
	}
}

```