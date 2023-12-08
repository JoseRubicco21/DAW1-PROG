## Enunciado
Programa java que declare cuatro variables enteras A, B, C y D y asígnale un valor a cada una. A continuación realiza las instrucciones necesarias para que:
B tome el valor de C
C tome el valor de A
A tome el valor de D
D tome el valor de B
Si por ejemplo A = 1, B = 2, C = 3 y D = 4 el programa debe mostrar:
Valores iniciales
A = 1
B = 2
C = 3
D = 4
Valores finales
B toma el valor de C -> B = 3
C toma el valor de A -> C = 1
A toma el valor de D -> A = 4
D toma el valor de B -> D = 2

## Solución
 
```java
public class Ejercicio_4 {
    public static void main(String[] args) { 
    int A=1, B=2, C=3, D=4, aux;
				
		/* B->C
		* C->A
		* A->D
		* D->B
		*/
		
		aux = B;
		// aux(B), A(A), B(B), C(C), D(D)
		B=C;
		// aux(B), A(A), B(C), C(C), D(D)
		C=aux;
		// aux 0 is not needed but it helps 
		aux = 0;
		// aux(0), A(A), B(C), C(B), D(D)
		aux = D;
		// aux(D), A(A), B(C), C(B), D(D)
		D=C;
		// aux(D), A(A), B(C), C(B), D(B)
		C=aux;
		// aux(D), A(A), B(C), C(D), D(B)
		aux = 0;
		// aux(0), A(A), B(C), C(D), D(B)
		aux = A;
		// aux(A), A(A), B(C), C(D), D(B)
		A=C;
		// aux(A), A(D), B(C), C(D), D(B)
		C=aux;
				
		System.out.print("Valores Iniciales:\nA = 1\nB = 2\nC = 3\nD = 4\n");
		System.out.println("Valores finales:");
		System.out.println("B toma el valor de C -> B = " + B);
		System.out.println("C toma el valor de A -> C = " + C);
		System.out.println("A toma el valor de D -> A = " + A);
		System.out.println("D toma el valor de B -> D = " + D);
    }
}
```
