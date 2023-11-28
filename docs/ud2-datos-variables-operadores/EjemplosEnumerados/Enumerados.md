## Definición

Los enumerados no son más que un conjunto de datos que tienen un valor fijo. Ejemplos de enumerados pueden ser: 

- Dias de la semana.
- Tallas de ropa.
- Niveles de experiencia.

Es importante denotar que, por lo menos en java, los valores de los enumerados son escritos en mayusculas. 

### Ejemplos escritos en JAVA:

Un ejemplo de enumerado con tallas de ropa:

```java
   enum Size {
    SMALL, MEDIUM, LARGE, EXTRALARGE
   } 
```

Otro ejemplo de enumerado con los dias:

```java
    enum Dias {
        LUNES, MARTES, MIERCOLES, JUEVES, VIERNES, SABADO, DOMINGO
    }
```

Para poder accesar a los valores de un enumerado debemos de utilizar el nombre de dicho enumerado.

```java
    enum Size {
        SMALL, MEDIUM, LARGE, EXTRALARGE
    } 

    // Imaginemos que todas las camisetas serán de tamaño SMALL en un principio
    
    public class Camiseta {
        private Size tamaño = Size.SMALL;
    }
```

:::Note

Los enumerados en **Java** son considerados una clase "Especial". Esto permite tener cosas mucho más complejas e útiles. Por ejemplo:

:::

Un pequeño ejemplo con un enumerado de experiencia seria:

```java
enum Experiencia {
    BAJA, MEDIA, ALTA;
	
	public String getExperiencia(){
        switch(this){
            case BAJA:
                return "Baja";
            case MEDIA:
                return "Media";
            
            case ALTA:
                return "Alta";
			default:
            	return "";
        }
    }
}

public class Test {
	// Método main para probar si nuestro método de la clase Experiencia funciona correctamente:
	public static void main(String[] args){
	    System.out.println("La experiencia del trabajador es: " + Experiencia.ALTA.getExperiencia());
	}
}
```
