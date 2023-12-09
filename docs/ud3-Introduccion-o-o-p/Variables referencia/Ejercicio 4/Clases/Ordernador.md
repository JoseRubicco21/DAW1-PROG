## Código

```java
public class Ordenador {
	private int num;
	private String ip;
	
	public int getNum() {
		return num;
	}

	public void setNum(int num) {
		this.num = num;
	}

	public String getIp() {
		return ip;
	}

	public void setIp(String ip) {
		this.ip = ip;
	}

	public boolean isReparado() {
		return reparado;
	}

	public void setReparado(boolean reparado) {
		this.reparado = reparado;
	}

	public Alumno getAlumno() {
		return alumno;
	}

	public void setAlumno(Alumno alumno) {
		this.alumno = alumno;
	}

	public Aula getAula() {
		return aula;
	}

	public void setAula(Aula aula) {
		this.aula = aula;
	}

	private boolean reparado;
	
	// Relation to classes
	private Alumno alumno;
	private Aula aula;
	
	@Override
	public String toString(){
		return ("Núm de ordenador: " + this.getNum() + "\n IP: " + this.getIp() + "\n");
	};
}
```