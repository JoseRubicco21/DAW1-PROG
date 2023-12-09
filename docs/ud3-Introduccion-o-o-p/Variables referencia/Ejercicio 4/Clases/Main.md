## Código

```java
public class Main {

	public static void main(String[] args) {
		
		// Creation of Aula object
		Aula aula = new Aula();
		
		aula.setNum(26);
		aula.setPlanta(2);
		
		// Creation of students
		Alumno a1 = new Alumno();
		a1.setName("Jose");
		a1.setDni(new DNI());
		a1.getDni().setNum(0000002);
		a1.getDni().setLetra('B');
		a1.setAge(22);
		
		Alumno a2 = new Alumno();
		a2.setName("Ana");
		a2.setDni(new DNI());
		a2.getDni().setNum(33333);
		a2.getDni().setLetra('C');
		a2.setAge(23);
		
		Alumno a3 = new Alumno();
		a3.setName("Pedro");
		a3.setDni(new DNI());
		a3.getDni().setNum(555555);
		a3.getDni().setLetra('N');
		a3.setAge(21);

		// Creation of PCs
		Ordenador o1, o2, o3;
		
		o1 = new Ordenador();
		o2 = new Ordenador();
		o3 = new Ordenador();
		
		o1.setNum(1);
		o2.setNum(2);
		o3.setNum(3);
		
		o1.setIp("192.168.10.100"); 
		o2.setIp("192.168.10.101");
		o3.setIp("192.168.10.102");
		
		// Assignation of every PC to every Student as 1:1
		o1.setAlumno(a1);
		o2.setAlumno(a2);
		o3.setAlumno(a3);
		
		a1.setOrdenador(o1);
		a2.setOrdenador(o2);
		a3.setOrdenador(o3);
		
		// Assigning students and PCs to the classroom
		a1.setAula(aula);
		a2.setAula(aula);
		a3.setAula(aula);
		
		o1.setAula(aula);
		o2.setAula(aula);
		o3.setAula(aula);
	
		aula.setAlu1(a1);
		aula.setAlu2(a2);
		aula.setAlu3(a3);
		
		System.out.println(aula);
	}
}
```