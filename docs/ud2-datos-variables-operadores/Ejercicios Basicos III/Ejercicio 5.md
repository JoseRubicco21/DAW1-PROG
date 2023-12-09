## Enunciado
Desarrolla un programa con la siguiente salida usando las posibilidades de printf():

```
1,0/3,0 = 0,333 
1,0/3,0 = 0,33333 
1,0/2,0 = 0,500 
1000/3,0 = 3,33e+02 
3,0/4567,0.0 = 6,569e-04 
-1,0/0,0 = -Infinity 
0,0/0,0 = NaN 
pi = 3,142, e =  2,7183 
C = 2 * 3,14159 * 1,1 A = 1,1 * 1,1 * 3,14159
```

## Solución

 
```java
public class Ejercicio_5 {
    public static void main(String[] args) { 
    	
		System.out.printf("%.1f/%.1f = %.3f %n", 1.0,3.0, 1.0/3.0);
		System.out.printf("%.1f/%.1f = %.5f %n", 1.0,3.0,1.0/3.0);
		System.out.printf("%.1f/%.1f = %05.3f %n", 1.0,2.0,1.0/2.0);
		System.out.printf("%d/%.1f = %.2e %n", 1000,3.0,1000/3.0);
		System.out.printf("%.1f/%.1f.0 = %.3e %n", 3.0,4567.0,3.0/4567.0);
		System.out.printf("%+.1f/%.1f = %f %n", -1.0,0.0,-1.0/0.0);
		System.out.printf("%1$.1f/%1$.1f = %2$f %n", 0.0, 0.0/0.0);
		System.out.printf("pi = %.3f, e =  %.4f %n", Math.PI, Math.E);
		System.out.printf("C = %1$d * %2$.5f * %3$.1f A = %3$.1f * %3$.1f * %2$.5f", 2, 3.14159, 1.1);
    }
}
```
