## Enunciado

imprimir los códigos enteros de los siguientes caracteres: A B C a b c 1 2 3 . 
Observa que los números asignados tienen cierta lógica entre sí. Por ejemplo, entre las 
letras mayúsculas los códigos se van asignando por orden alfabético, identico para las 
minúsculas y para los números se les van también asignando códigos con lógica (el código 
de ‘2’, es el siguiente al de ‘1’ etc.)

### Código

```java
public Class Ejercicio_2 {

    public static void main(String[] args){

        System.out.println((int)'A'); // La salida por consola es 65
        System.out.println((int)'B'); // La salida por consola es 66
        System.out.println((int)'C'); // La salida por consola es 67
        System.out.println((int)'a'); // La salida por consola es 97
        System.out.println((int)'b'); // La salida por consola es 98
        System.out.println((int)'c'); // La salida por consola es 99
        System.out.println((int)'1'); // La salida por consola es 49
        System.out.println((int)'2'); // La salida por consola es 50
        System.out.println((int)'3'); // La salida por consola es 51
    }
}
```