## Enunciado:

Descomenta la última instrucción y observa el error del compilador en este código. Razona el error.

## Código Fuente:

```java
public class Unidad1 {
    public static void main(String[] args) {
   
    int edad; //declaramos (definimos) una variable
    edad=60; //le damos un valor a una variable
    int peso=75; //al mismo tiempo que se define una variable se le puede asignar un valor
    
    System.out.println(edad);
    System.out.println(peso);
    
    //el valor de la variable se puede imprimir junto a cadenas de caracteres
    System.out.println("mi edad es: "+edad);
    peso=80;
    System.out.println(peso);
    
    //puedo hacer operaciones con las variables
    System.out.println("el peso de los años ..." + peso*edad);
    
    //el resultado de una operacion puede almacenarse en otra variable
    int salud;
    salud=peso*edad;
    System.out.println("la variable salud contiene el valor: " + salud);
    
    //el valor que se le asigna a una variable deber ser compatible con su tipo
    //edad="jamones para todos";
 }
}
```

## Solución

```java
public class Unidad1 {
    public static void main(String[] args) {
   
    int edad; //declaramos (definimos) una variable
    edad=60; //le damos un valor a una variable
    int peso=75; //al mismo tiempo que se define una variable se le puede asignar un valor
    
    System.out.println(edad);
    System.out.println(peso);
    
    //el valor de la variable se puede imprimir junto a cadenas de caracteres
    System.out.println("mi edad es: "+edad);
    peso=80;
    System.out.println(peso);
    
    //puedo hacer operaciones con las variables
    System.out.println("el peso de los años ..." + peso*edad);
    
    //el resultado de una operacion puede almacenarse en otra variable
    int salud;
    salud=peso*edad;
    System.out.println("la variable salud contiene el valor: " + salud);
    
    //el valor que se le asigna a una variable deber ser compatible con su tipo
    edad="jamones para todos";
 }
}
```

### Razonamiento: 

La variable edad esta definida como tipo *int*. En este caso estamos intentando introducir un tipo de dato *String* cosa que simplemente no sé puede hacer ya que el tipo de la variable no coincide con el dato introducido. El programa espra en edad una variable dde tipo *int*.