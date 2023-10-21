## Enunciado

Realiza otro programa muy parecido al [Ejercicio 1](./Ejercicio%201.md) pero para círculos. Calcular a área dun círculo de radio 2 e mostrar por pantalla o resultado. Utiliza la constante "Math.PI"

## Solución

```java
public Class AreaCuadrado {
    int radio;
    int areaCirculo;

    radio = 4;
    areaCirculo = Math.PI * Math.pow(radio, 2); 

    System.out.println("El área del cuadrado es: " + areaCirculo);
}
```

## Razonamiento

Basandonos en el primer programa es muy simple crear uno semejante para el área de un círculo. Sabiendo que la formula es $\pi * r^2$ pues utilizamos la constante `Pi` de la clase `Math` con `Math.PI` y el método `Math.Pow(double a, double b)` para hacer una potencia donde:

- A es la base
- B es el exponente
