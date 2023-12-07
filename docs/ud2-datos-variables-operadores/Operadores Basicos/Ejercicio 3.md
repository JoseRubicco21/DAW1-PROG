## Enunciado
Comprueba si ++x*y es equivalente o no a (++x)*y. Idem respecto a ++(x*y).

Al probar esta situaciones debes también detectar un error de compilación en la última
expresión

## Código

```java

public class Ejercicio_3 {
    public static void main(String[] args){
            int x =  3;
	        int y = 1;
	        int z = ++x*y;
	        int n =(++x)*y;
	        int m = ++(x*y); // Operación invalida

	        System.out.println("x: " + x + " y: " + y);
	        System.out.println("z: " + z + " n:" + n);
    }
}
```