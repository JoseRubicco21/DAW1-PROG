## Enunciado

comprueba que una vez que se inicializa una constante no se le puede cambiar de
valor


## Solución

```java
final int VELOCIDAD_LUZ=300000;
VELOCIDAD_LUZ=20;//¡error!
```

## Razonamiento

Las *constantes* no se pueden reasignar. Son precisamente **constantes** a lo largo de la ejecución del programa al utilizar el operado de asignacion `=` tira un error que precisamente advierte de esto.