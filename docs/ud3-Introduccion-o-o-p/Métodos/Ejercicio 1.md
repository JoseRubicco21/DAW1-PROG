## Enunciado
cambia en el ejercicio anterior calcularAutonomia() y main() como acabamos de indicar. Experimenta la ejecución combinando los siguientes factores:
- Las dos clases se escriben en el mismo .java y cada una en .java diferentes
- Probamos ambas combinaciones en consola y en un IDE.

```java
class Coche{
 int pasajeros; //número de pasajeros
 int deposito; //capacidad del depositos en litros
 int kpl; //kilometros que se pueden recorrer con un litro,
}

class Unidad2 {
 public static void main(String[] args) {
 Coche peugeot308 = new Coche();
 peugeot308.pasajeros=5;
 peugeot308.deposito=60;
 peugeot308.kpl=20;
 System.out.println("pasajeros:" + peugeot308.pasajeros);
 System.out.println("deposito:" + peugeot308.deposito);
 System.out.println("kpl:" + peugeot308.kpl);
 System.out.println("Autonomía:" + peugeot308.deposito*peugeot308.kpl);
 }
}
```
## Solución

### Solución 1: 
Ambas clases en un mismo fichero:

```java
class Coche{
 int pasajeros; //número de pasajeros
 int deposito; //capacidad del depositos en litros
 int kpl; //kilometros que se pueden recorrer con un litro,

 public int calcularAutonomia(){
    return depostio*kpl;
 }
}

class Unidad2 {
 public static void main(String[] args) {
 Coche peugeot308 = new Coche();
 peugeot308.pasajeros=5;
 peugeot308.deposito=60;
 peugeot308.kpl=20;
 System.out.println("pasajeros:" + peugeot308.pasajeros);
 System.out.println("deposito:" + peugeot308.deposito);
 System.out.println("kpl:" + peugeot308.kpl);
 System.out.println("Autonomía:" + peugeot308.calcularAutonomia());
 
 }
}
```

### Solución 2:

En ficheros diferentes

#### Clase Coche

```java
class Coche{
 int pasajeros; //número de pasajeros
 int deposito; //capacidad del depositos en litros
 int kpl; //kilometros que se pueden recorrer con un litro,

 public int calcularAutonomia(){
    return depostio*kpl;
 }
}
```

#### Clase Main

 
```java
public class Unidad2 {
    public static void main(String[] args) { 
     Coche peugeot308 = new Coche();
    peugeot308.pasajeros=5;
    peugeot308.deposito=60;
    peugeot308.kpl=20;
    
    System.out.println("pasajeros:" + peugeot308.pasajeros);
    System.out.println("deposito:" + peugeot308.deposito);
    System.out.println("kpl:" + peugeot308.kpl);
    System.out.println("Autonomía:" + peugeot308.calcularAutonomia());
    }
}
```


