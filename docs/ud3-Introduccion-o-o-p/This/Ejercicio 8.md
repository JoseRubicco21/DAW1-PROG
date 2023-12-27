## Enunciado
Crea una clase Cuenta con los siguientes atributos privados
 - String numeroCuenta;
 - String titular;
 - double saldo;

La clase cuenta debe de ser manejada por la clase Unidad2 de la siguiente forma:
```java
public class Unidad2{
 public static void main(String[] args) {
 
    Cuenta c1= new Cuenta("111-222","Epi",50.0);
    System.out.println("el saldo inicial de Epi es: "+ c1.getSaldo());
 
    Cuenta c2= new Cuenta("999-888","Blas",100.0);
    System.out.println("el saldo inicial de Blas es: "+ c2.getSaldo());
 
    //no es posible utilizar el constructor sin parámetros
    //Cuenta c3= new Cuenta();
    
    // modificamos el saldo de Epi
    c1.setSaldo(250.0);
    System.out.println("el nuevo saldo de Epi es: "+ c1.getSaldo());
 
    // modificamos el saldo de Blas
    c2.setSaldo(877.5);
    System.out.println("el nuevo saldo de Blas es: "+ c2.getSaldo());
 }
}
```
**SALIDA**
el saldo inicial de Epi es: 50.0
el saldo inicial de Blas es: 100.0
el nuevo saldo de Epi es: 250.0
el nuevo saldo de Blas es: 877.5

Que usa el siguiente código
```java
class Coche{
 int pasajeros; //número de pasajeros
 int deposito; //capacidad del depositos en litros
 int kpl; //kilometros que se pueden recorrer con un litro,
 
 void autonomia(){
 System.out.println("Autonomía:" + deposito*kpl); //equivalentemente this.deposito*this.kpl
 }
}
```
```java
class DemoCoche {
 public static void main(String[] args) {
 Coche coche1 = new Coche();

 coche1.pasajeros=5;
 coche1.deposito=60;
 coche1.kpl=20;
 coche1.autonomia();
 }
}
```
## Solución

```java
class Cuenta {
    String numeroCuenta;
    String titular;
    double saldo;

    Cuenta(){

    }

    Cuenta(String numeroCuenta, String titular, double saldo){
        this.numeroCuenta = numeroCuenta;
        this.titular = titular;
        this.saldo = saldo;
    }

    public void setNumeroCuenta(String numeroCuenta){
        this.numeroCuenta = numeroCuenta;
    }

    public void setTitular(String titular){
        this.titular = titular;
    }

    public void setSaldo(double saldo){
        this.saldo = saldo
    }

    public String getNumeroCuenta(){
        return this.numeroCuenta        
    }

    public String getTitular(){
        return this.titular
    }

    public double getSaldo(){
        return this.saldo
    }

}
```