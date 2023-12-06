## Enunciado

Comprueba el siguiente código: La instrucción 2º y 3º hacen lo mismo, imprimen el código entero asociado al caracter ‘B’
¿Porque la primera necesita (int) y la segunda no?. ¿Porque la última instrucción imprime el
caracter ‘B’?

## Código

```java 
class Ejercicio_3{
    public static void main(String[] args){
    System.out.println("Código entero del caracter \'A\': "+ (int)'A');
    System.out.println("Código entero del caracter \'B\': "+ (int)'B');
    System.out.println("Código entero del caracter \'B\': "+ ('A'+1));
    System.out.println("Código entero del caracter \'B\': "+ (char)('A'+1));
    }
}
```

## Solución

En la segudna instrucción estamos intentando imprimir el código de caracter de B utilizando un literal de caracter `'B'` en cambio en la linea tres estamos usando un literal de un caracter pero le andamos sumando un entero. Aquí ocurre un casting implicito, y se caste de *char* a *int* sin tener que especificarlo.

En la ultima instrucción sucede lo mismo que lo anterior solo que aquí estamos casteando explicitamente a caracter y el tipo de dato devuelto es un caaracter. En este caso el caracter que corresponde al código de *A+1* es *B* Si hiciesemos lo mismo solo que a la inversa obtendriamos el caracter `A`

```java
System.out.println("Código entero del caracter \'A\': "+ (char)('B'-1)); // Retorna el caracter 'A'
```