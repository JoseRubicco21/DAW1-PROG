## Enunciado
Crea un objeto peugeot308 con las siguientes características:
5 pasajeros
60 litros de deposito
20 kpl
El programa da los datos anteriores a los atributos correspondientes, calcula la autonomía del
coche (kpl*deposito) y finalmente imprime los atributos del coche y su autonomía.
## Solución

```java
class Coche{
 int pasajeros; //número de pasajeros
 int deposito; //capacidad del depositos en litros
 int kpl; //kilometros que se pueden recorrer con un litro,
}

class Unidad2{
 public static void main(String[] args) {
    Coche peugeot308 = new Coche();
    peugeot308.pasajeros = 5;
    peugeot308.deposito = 60;
    peugeot308.kpl = 20;

    System.out.println("Pasajeros: " + peugeot308.pasajeros);
    System.out.println("Deposito: " + peugeot308.deposito);
    System.out.println("KPL: " + peugeot308.kpl);
    System.out.println("Autonomia: " + (peugeot308.kpl * peugeot308.deposito));
 }
}
```
