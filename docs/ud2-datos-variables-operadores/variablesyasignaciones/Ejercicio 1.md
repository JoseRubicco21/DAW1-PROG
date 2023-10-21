## Enunciado

En una clase AreaCuadrado escribe un programa que guarde en una variable entera
la longitud del lado de un cuadrado, con dicha variable calcule el área del cuadrado y almacene
este valor en otra variable. Imprime por pantalla el valor de esta última variable. 

## Solución

```java
public Class AreaCuadrado {
    int ladoCuadrado;
    int areaCuadrado;

    ladoCuadrado = 4;
    areaCuadrado = ladoCuadrado * ladoCuadrado;

    System.out.println("El área del cuadrado es: " + areaCuadrado);
}
```
## Razonamiento: 

- Creamos una variable de tipo entero llamado ladoCuadrado y otra areaCuadrado. La formula del lado de un cuadrado no es más que $lado * lado$ o $l^2$. Asignamos el valor de `areaCuadrado` a `ladoCuadrado * ladoCuadrado` e imprimimos por pantalla el resultado con:

```java
System.out.println("El área del cuadrado" + areaCuadrado)
```