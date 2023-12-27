## Enunciado
Reescribe Ejercicio 6 con this.

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
    return this.calcularAutonomia()>c.calcularAutonomia() ? this : c;
    }
}
```