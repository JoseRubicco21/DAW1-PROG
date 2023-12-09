## Código

```java
public class Aula {
	private int num; // Could be short
	private int planta; // Could be short, Enum or String. 
	
	
	// Relation to classes
	//Alumno alumno; // This should be an array of objects
	private Ordenador ordenador; // This should be an array  of objects
	
	// Since we're not using an array list we would need to do:
	private Alumno alu1;
	private Alumno alu2;
	private Alumno alu3;
	
	// Same would go for PCs
	
	public int getNum() {
		return num;
	}

	public void setNum(int num) {
		this.num = num;
	}

	public int getPlanta() {
		return planta;
	}

	public void setPlanta(int planta) {
		this.planta = planta;
	}

	public Ordenador getOrdenador() {
		return ordenador;
	}

	public void setOrdenador(Ordenador ordenador) {
		this.ordenador = ordenador;
	}

	public Alumno getAlu1() {
		return alu1;
	}

	public void setAlu1(Alumno alu1) {
		this.alu1 = alu1;
	}

	public Alumno getAlu2() {
		return alu2;
	}

	public void setAlu2(Alumno alu2) {
		this.alu2 = alu2;
	}

	public Alumno getAlu3() {
		return alu3;
	}

	public void setAlu3(Alumno alu3) {
		this.alu3 = alu3;
	}

	@Override
	public String toString(){
		return ("Núm de aula: " + this.getNum() + "\n planta: " + this.getPlanta() + "\nAlumnos: " + this.getAlu1() + this.getAlu2() + this.getAlu3());
	};
	
}
```