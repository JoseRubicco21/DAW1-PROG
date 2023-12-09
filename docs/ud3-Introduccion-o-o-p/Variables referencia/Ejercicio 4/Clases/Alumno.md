## Código

```java
public class Alumno {
	private String name; // You could also add Last name as an attribute.
	private DNI dni;
	private int age;
	
	// Relation to other classes
	private Ordenador ordenador;
	private Aula aula;
	
	public String getName() {
		return name;
	}

	public void setName(String name) {
		this.name = name;
	}

	public DNI getDni() {
		return dni;
	}

	public void setDni(DNI dni) {
		this.dni = dni;
	}

	public int getAge() {
		return age;
	}

	public void setAge(int age) {
		this.age = age;
	}

	public Ordenador getOrdenador() {
		return ordenador;
	}

	public void setOrdenador(Ordenador ordenador) {
		this.ordenador = ordenador;
	}

	public Aula getAula() {
		return aula;
	}

	public void setAula(Aula aula) {
		this.aula = aula;
	}

	@Override
	public String toString(){
		return ("Nombre: " + name + "\nEdad: " + age + "\nDNI: " + dni + "\n" + ordenador);
	};
}

```