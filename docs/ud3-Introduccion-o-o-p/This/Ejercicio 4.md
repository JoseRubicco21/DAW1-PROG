## Enunciado
Anteriormente, hicimos el siguiente ejercicio:

```java
class Coche{
    int pasajeros;
    int deposito;
    int kpl;

    void setPasajeros(int p){
    pasajeros = p;
    }

    void setDeposito(int d){
    deposito = d;
    }
 
    void setKpl(int k){
    kpl=k;
    }
 
    int getPasajeros(){
    return pasajeros;
    }
 
    int getDeposito(){
    return deposito;
    }
 
    int getKpl(){
    return kpl;
    }
 
    int autonomia(){
    return deposito*kpl;
    }

    double gasofaNecesaria(int kilometros){
    return (double) kilometros/kpl;
    }
}
```
```java
class Unidad2 {
 public static void main(String[] args) {
    Coche citroenC1= new Coche();
    
    citroenC1.setPasajeros(4);
    citroenC1.setDeposito(50);
    citroenC1.setKpl(25);
    
    System.out.println("un citroen C1 permite sólo " + citroenC1.getPasajeros() + " pasajeros");
    System.out.println("un citroen C1 tiene una autonomía de " + citroenC1.autonomia() + " kilómetros");
    }
}
```
Modifícalo para que los métodos set utilic
## Solución
```java
class Coche{
    int pasajeros;
    int deposito;
    int kpl;

    void setPasajeros(int pasajeros){
    this.pasajeros = pasajeros;
    }

    void setDeposito(int deposito){
    this.deposito = deposito;
    }
 
    void setKpl(int kpl){
    this.kpl=kpl;
    }
 
    int getPasajeros(){
    return pasajeros;
    }
 
    int getDeposito(){
    return deposito;
    }
 
    int getKpl(){
    return kpl;
    }
 
    int autonomia(){
    return deposito*kpl;
    }

    double gasofaNecesaria(int kilometros){
    return (double) kilometros/kpl;
 }
}
```
```java
class Unidad2 {
 public static void main(String[] args) {
    Coche citroenC1= new Coche();
    
    citroenC1.setPasajeros(4);
    citroenC1.setDeposito(50);
    citroenC1.setKpl(25);
    
    System.out.println("un citroen C1 permite sólo " + citroenC1.getPasajeros() + " pasajeros");
    System.out.println("un citroen C1 tiene una autonomía de " + citroenC1.autonomia() + " kilómetros");
    }
}
```