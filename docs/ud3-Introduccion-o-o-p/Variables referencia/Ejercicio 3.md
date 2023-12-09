## Enunciado
Observa este código.
```java
class Unidad2 {
    public static void main(String[] args) {
        Coche coche1 = new Coche();
        coche1.pasajeros=5;
        coche1.deposito=60;
        coche1.kpl=20;

        Coche coche2 = new Coche();
        coche2.pasajeros=5;
        coche2.deposito=60;
        coche2.kpl=20;

        Coche coche3=coche1;
    }
}
```
coche1 y coche2 apuntan realmente a objetos distintos, cada uno de estos objetos
tiene los mismos valores pero son objetos distintos. Por el contrario coche3 y coche1
referencia al mismo objeto.
SE PIDE: Demuestra esto utilizando el operador == obteniendo una salida similar a la
siguiente

## Solución

### Clase Coche
```java
public class Coche {

	String color;
	float velocidad;
	float tamaño;
	String carburante;
	String modelo;
	int deposito;
	int pasajeros;
	int kpl;
	
	void ir(){
		
	};
	
	void parar() {
		
	};
	
	void girarDerecha(){
		
	};
	
	void girarIzquierda(){
		
	};
	
	void arrancar(){
		
		System.out.println("Arrancando " + modelo + " de color " + color + " con " + kpl + " en el tanque. pasajeros: " + pasajeros + "deposito:" +deposito);
	};
	
	void autonomia(){
		System.out.println("Autonomia: " + kpl*deposito);
	}
}
```

### Clase Ejercicio_3 (Main)

```java
public class Ejercicio_3 {
    public static void main(String[] args) { 
        
        Coche coche1 = new Coche();
		coche1.pasajeros = 5;
		coche1.deposito = 60;
		coche1.kpl = 20;
		
		Coche coche2 = new Coche();
		coche2.pasajeros = 5;
		coche2.deposito = 60;
		coche2.kpl = 20;
		
		Coche coche3 = coche1;
		
		System.out.printf("coche1 == coche2: %B %n", coche1 == coche2);
		System.out.printf("coche1 == coche3: %B ", coche1 == coche3);
		coche2.autonomia();
    }
}
```