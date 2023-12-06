## Enunciado

## Código

```java
public class Ejercicio_4 {

	public static void main(String[] args) {
		// You probably want to make this a for loop.
		/*
		byte n127 = (byte)127;
		byte n128 = (byte)128;
		byte n129 = (byte)129;
		byte n130 = (byte)130;
		byte n255 = (byte)255;
		
		System.out.println("int 127 es en byte:" + n127);
		System.out.println("int 128 es en byte:" + n128);
		System.out.println("int 129 es en byte:" + n129);
		System.out.println("int 130 es en byte:" + n130);
		System.out.println("int 255 es en byte:" + n255);
		*/
        
		//El resultado es asi puesto que el ultimo bit se utiliza para denominar si el número es positivo o negativo
	
		for (int i = 125; i < 271 ; i++) {
			
			byte intToByte = (byte)i;
			
			System.out.println("int " + i + " pasa a byte y es: " + intToByte);
		}
	}

}
```