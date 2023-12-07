## Enunciado
Escribe código equivalente al siguiente sin utilizar el operador unario ++

```java
    class Incremento_1 {
       public static void main(String[] args){
        int x=3;
        int y;
        y=x++*2;
        System.out.println("x: " + x + " y:" + y);
    }
}
```
## Código 

```java
    class Incremento_1 {
        public static void main(String[] args){
            int x = 3;
            int y;
            // Opción 1:
            int z = x + 1;
            int n =  z * 2;
            
            // Opción 2:
            y = (x += 1) * 2;
            
          
            System.out.println("x: " + x + " y: " + y);
            System.out.println("x: " + z + " y: " + n);
        }
    }
```
## Razonamiento

Con la primera opción creamos dos variables auxiliares que remplazan a `y` y a `x++`. En el segundo caso hacemos el mismo procedimiento solo que de forma más condensada y sin la necesidad de crear variables auxiliares. 

Podriamos decir que `+=` replica el comportamiento de `++` ya que estamos adicionando 1, si fuese otro número ya no seria el caso. 