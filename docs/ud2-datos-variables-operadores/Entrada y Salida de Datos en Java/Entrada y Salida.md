## Salida por consola

Una de las operaciones más básicas que podemos utilziar en Java es la salida por consola. O lo que se conoce como imprimir por consola.

Para lograr esto disponemos de una clase **System** que proporciona accesos a recursos del sistema. Esta clase posee 2 atributos importantes referente a la entrada y la salida:

- out: Esta conectado a la salida "Estándar" del sistema y nos proporciona métodos para poder escribir en ella
- in: Esta conectado a la entrada "Estándar" del sistema y nos proporciona métodos para poder obtener datos de ella.

### Métodos de salida

Usualmente se utilizan 3 métodos para mostrar una salida por consola:

- `System.out.println();`
- `System.out.print();`
- `System.out.printf();`

#### Método println()

Imprime un objeto String pasado como argumento con un salto de linea al final

#### Método print()

Imprime un objeto String pasado como argumento

#### Método printf()

Imprime un objeto String pasado como argumento con un formato especificado.

`printf()` utiliza *secuencias de formato* o lo que se puede entender como "Sustituciones"

| Cáracter de conversión | imprime | 
| :--: | :--: |
| c | caracter individual |
| C | caracter individual (Mayúsculas) |
| b | booleano |
| B | booleano (Mayúsculas) |
| d | número entero |
| f | número en punto flotante |
| e | número en punto flotante con notación cientifica |
| s | cadena de caracteres |
| S | cadena de caracter (Mayúsculas) |
| n | Salto de linea |
| t**M** | fecha y hora (M establece el modificador de formato de la fecha) |    

Es importante también enteder que una sentencia de sustitución de `printf()` consta de varias partes:

- Indicador de sustitución: %
- flags: establece modificadores de salida, especialmente con numeros
- ancho: El espacio minimo de caracteres que ocupara el campo
- precision: Número de digitos decimales de punto flotante
- emparejamiento: Indica que en esa sustitución se utilizara el argumento *n*

## Entrada de datos

Una de las formas mas simple de obtener datos en Java es mediante la utilización de la clase *Scanner*. Esta nos permite utilziar valores primitivos sin tener que hacer conversiones.

Algunos de los métodos mas usados para obtener datos:
- `nextBoolean();` : Lee un valor de tipo *boolean*
- `nextByte();` : Lee un valor de tipo *byte*
- `nextDouble();` : Lee un valor de tipo *double*
- `nextFloat();` : Lee un valor de tipo *float*
- `nextInt();` : Lee un valor de *int*
- `nextLine()`; : Lee la entrada como un *String*
- `nextLong();` : lee la entrada como un *long*
- `nextShort();` : lee la entrada como un *short*

:::warning

Si se utilizan en conjunto los métodos `nextLine()` con cualquier otro es importante recordar de hacer un `nextLine()` de nuevo ya que si no solo se quedaria con el *carriage return*

:::

Si en algún momento el dato recibido no es convertible el programa finalizará su ejecución tirando un error.