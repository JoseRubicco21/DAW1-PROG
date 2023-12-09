## Enunciado
```java
class Coche{
 int pasajeros; //número de pasajeros
 int deposito; //capacidad del depositos en litros
 int kpl; //kilometros que se pueden recorrer con un litro,
}

class Unidad2{
 public static void main(String[] args) {
 Coche golf = new Coche();//se crea el objeto
 golf.pasajeros=5;//se usa el objeto
 System.out.println("pasajeros:" + golf.pasajeros); //se usa el objeto
 }
}
```
Añade instrucciones para que que cree también un objeto megane para el que almacenamos
que tiene un depósito 60 litros e imprimimos este atributo por pantalla.

Observa que un programa java es un conjunto de clases, como mínimo una. Una y sólo una
clase debe contener el método main() que es el punto de entrada al programa y por tanto
sólo puede haber un método main en todo el programa. 

## Solución

```java

class Coche{
 int pasajeros; //número de pasajeros
 int deposito; //capacidad del depositos en litros
 int kpl; //kilometros que se pueden recorrer con un litro,
}

class Unidad2{
 public static void main(String[] args) {
    Coche golf = new Coche();//se crea el objeto
    golf.pasajeros=5;//se usa el objeto
    System.out.println("pasajeros:" + golf.pasajeros); //se usa el objeto

    Coche megane = new Coche();
    megane.deposito=60;
    System.out.println("deposito: " + megane.deposito)
 }
}
```
