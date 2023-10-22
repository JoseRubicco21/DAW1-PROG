## Enunciado
Escribe un programa que almacene en variables y luego imprima por pantalla, 4 características
de una de una persona: Su nombre completo, su sexo, su edad y su peso. Elige para cada
variable el tipo de dato más económico en bits. Obtén una salida similar a la siguiente:

```
nombre: Juan Lopez Salvado
sexo: v
edad: 49
peso: 70.8
```
## Solución
 
```java
public class Ejercicio_1 {
    public static void main(String[] args) { 
        String nombre;
        char sexo;
        short edad; // Podría ser int perfectamente. 
        float peso;

        nombre = "Juan Lopez Salvado";
        sexo = 'v';
        edad = 49;
        peso = 70.8f;
    
        System.out.println("nombre: " + nombre);
        System.out.println("sexo: " + sexo);
        System.out.println("edad: " + edad);
        System.out.println("peso: " + peso);
    }
}
```

## Razonamiento

Es un programa simple. Vemos que necesitamos guardar 4 datos principales:
- Nombre
- Sexo
- Edad
- Peso

Según el ejemplo estos datos deberian de tener cierto formato. Por ejemplo, la variable *sexo* tiene como valor *v* asi que podemos asumir que el otro tipo de dato es *f*. También podemos asumir que la variable peso no será ni un **short**, **int** o **long** puesto que tiene decimales. Solo puede ser **float** o **double** porque son las que permiten decimal.

Otra cosa importante que debemos tener en cuenta es que dato estamos guardando allí realmente. A pesar de que se nos pida que usemos el tipo de dato mas económico en número de bits también es imprescindible pensar en quien leera el código en caso de que otra persona o uno mismo lo quiera mantener. Por este motivo es importante colocar tipos de datos que tengan sentido.

:::info Variable "Peso"
La variable peso necesita de un f al final del número puesto que si no se indica Java pensará que se esta trabajando con un *double* en vez de un *float* ya que los literales *double* se reprensenta como un número decimal sin mas.
:::

Si vamos a los técnicismos con número de bits ahorrado se pueden hacer los siguientes cambios:

- sexo: char --> boolean
- edad: int --> byte

¿Por qué? realmente en el caso de sexo representar las opciones que tenemos como *v* o *f* es exactamente lo mismo que representarlo con *1* o *0*.  En el caso de edad, no hay ningún humano que realmente tenga una edad superior a 127.

| Tipo | Espacio ocupado |
|:--:|:--:|
| char | 16 bits |
| boolean | 1 bit |


| Tipo | Espacio ocupado |
|:--:|:--:|
| int | 32 bits |
| short | 16 bits |
| byte | 8 bits |
