## Enunciado

Escribe un programa que compruebe en la tabla anterior la fila de char de la tabla de casting:


| Tipo de dato | boolean | byte | short | char | int | long | float | double |
| :--: | :--: |:--:  |:--:  |:-:|:--:|:--:|:--:| :--:|
| char | no | cast | cast | N/A | si | si | si | si |

```java
public Class Ejercicio_1 {


    public static void main(String[] args) {
    	char variableACastear = 'a';

	        boolean pruebaDeBoolean;
	        byte pruebaDeByte;
	        short pruebaDeShort;
	        int pruebaDeInt;
	        long pruebaDeLong;
	        float pruebaDeFloat;
	        Double pruebaDeDouble;

            // No se puede castear de Char a bool. Esta linea debe dar error.
	        pruebaDeBoolean = ()variableACastear;
	        pruebaDeByte = (byte)variableACastear; // Casteo Explicito
	        pruebaDeShort = (short)variableACastear; // Casteo Explicito
	        pruebaDeInt = variableACastear; // Casteo Implicito
	        pruebaDeLong = variableACastear; // Casteo Implicito
	        pruebaDeFloat = variableACastear; // Casteo Implicito
	        pruebaDeDouble = (double)variableACastear; // Casteo Explicito
    }
}
```