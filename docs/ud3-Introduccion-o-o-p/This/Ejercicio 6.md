## Enunciado
Escribe el método sin completar y prueba el código. Observa que ahora mayorAutonomia no
devuelve boolean como en el ejemplo anterior.
```java
class Coche{
    int pasajeros; //número de pasajeros
    int deposito; //capacidad del depositos en litros
    int kpl; //kilometros que se pueden recorrer con un litro,
 
    int calcularAutonomia(){
    return deposito*kpl;
    }

    Coche mayorAutonomia(Coche c){
    //escribe aquí tu código
    }
}

class Unidad2{
    public static void main(String[] args) {
        Coche coche1= new Coche();
        coche1.pasajeros=5;
        coche1.deposito=60;
        coche1.kpl=20;

        Coche coche2= new Coche();
        coche2.pasajeros=7;
        coche2.deposito=100;
        coche2.kpl=30;

        Coche cocheMayorAutonomia=coche1.mayorAutonomia(coche2);
        
        System.out.println("El coche de mayor autonomia tiene de deposito "+ cocheMayorAutonomia.deposito + " y de consumo "+ cocheMayorAutonomia.kpl);
        
        }
}
```

## Solución

```java
class Coche{
    int pasajeros; //número de pasajeros
    int deposito; //capacidad del depositos en litros
    int kpl; //kilometros que se pueden recorrer con un litro,
 
    int calcularAutonomia(){
    return deposito*kpl;
    }

    Coche mayorAutonomia(Coche c){
    return calcularAutonomia()>c.calcularAutonomia() ? this : c;
    }
}
```
