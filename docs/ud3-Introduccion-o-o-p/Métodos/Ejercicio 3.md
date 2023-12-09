## Enunciado
Modifica el siguiente ejemplo de forma que los atributos sean private y se acceda a
8
ellos a través de set/get.
```java
class Bicicleta {
 int velocidade = 0;
 int marcha = 1;
 void cambiarMarcha(int novoValor) {
 marcha = novoValor;
 }
 void acelerar(int incremento) {
 velocidade = velocidade + incremento;
 }
 void frear(int decremento) {
 velocidade = velocidade - decremento;
 }
 void imprimirEstado() {
 System.out.println("Velocidade: "+velocidade+" Marcha: "+marcha);
 }

}
class Unidad2{
 public static void main(String[] args) {
 // Crea dous obxectos bicicleta
 Bicicleta bicicleta1 = new Bicicleta();
 Bicicleta bicicleta2 = new Bicicleta();
 // Invoca os métodos destes obxectos
 bicicleta1.acelerar(10);
 bicicleta1.cambiarMarcha(2);
 bicicleta1.imprimirEstado();
 bicicleta2.acelerar(10);
 bicicleta2.cambiarMarcha(2);
 bicicleta2.frear(2);
 bicicleta2.cambiarMarcha(3);
 bicicleta2.imprimirEstado();
 }
}
```

## Solución

```java
public class Bicicleta {

	private int velocidad;
	private int marcha;
	
	
	
	public int getVelocidad() {
		return velocidad;
	}

	public void setVelocidad(int velocidad) {
		this.velocidad = velocidad;
	}

	public int getMarcha() {
		return marcha;
	}

	public void setMarcha(int marcha) {
		this.marcha = marcha;
	}

	void cambiarMarcha(int nuevaMarcha) {
		this.setMarcha(nuevaMarcha);
	}
	
	void acelerar (int incremento) {
		this.setVelocidad(this.getVelocidad() + incremento);
	}
	
	void frenar (int decremento) {
		this.setVelocidad(this.getVelocidad() - decremento);	
	}
	
	void imprimirEstado() {
		System.out.printf("Marcha: %d Velocidad: %d %n", this.getMarcha(), this.getVelocidad());
	}
}

```