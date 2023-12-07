## Enunciado

Escribe código equivalente al siguiente sin utilizar el operador ++

```java
class Incremento_2{
    public static void main(String args[]){
    int x=3;
    int y;
    y=++x*2;
    System.out.println("x: "+ x+ " y:"+y);
    }
}
``` 

## Solución 

```java
class Incremento_2{
        public static void main(String[] args){
    	int x=3;
        int y;
        
        int z = x + 1;
        int n = z * 2;
        y=++x*2;
        System.out.println("x: "+ x+ " y: "+ y);
        System.out.println("x: " + z+ " y: " + n);
    }
}
```