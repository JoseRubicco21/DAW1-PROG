## Enunciado
En el boletín anterior, vimos este ejemplo
```java
class Coche{
    int pasajeros;
    int deposito;
    int kpl;
    
    int calcularAutonomia(){
    return deposito*kpl;
    }

    boolean mayorAutonomia(Coche c){
    return calcularAutonomia()>c.calcularAutonomia();
    }
}

class Unidad2 {
 public static void main(String[] args) {
    Coche coche1= new Coche();
    coche1.pasajeros=5;
    coche1.deposito=60;
    coche1.kpl=20;

    Coche coche2= new Coche();
    coche2.pasajeros=7;
    coche2.deposito=1000;
    coche2.kpl=30;
 
    System.out.println("Tiene coche1 más autonomía que coche2? "+ coche1.mayorAutonomia(coche2));
 }
}
```
e indicamos que mayorAutonomia() se entendería mejor si usamos this. Usa this y
explica el funcionamiento del método.

## Solución
```java
class Coche{
    int pasajeros;
    int deposito;
    int kpl;
    
    int calcularAutonomia(){
    return deposito*kpl;
    }

    boolean mayorAutonomia(Coche c){
    return this.calcularAutonomia()>c.calcularAutonomia();
    }
}
```
## Razonmaiento

El método `mayorAutonomia` recibe como parametro una variable de tipo `Coche` llamada `c`. Esta variable se usa en una comparación que retornará verdadero o falso. Al utilizar `this` estamos diciendo que se comparará este objeto (El objeto desde cual se llama el método) con el que pasamos como parametro.

En este caso, en el main ese `this` del método `calcularAutonomia` hace referencia a *coche1* ya que *coche1* es quien invoca o llama al método.