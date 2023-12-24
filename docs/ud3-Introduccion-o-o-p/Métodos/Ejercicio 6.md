## Enunciado

más difícil todavía. Ahora mayorAutonomia() debe devolverme el
objeto coche que es mayor.

## Solución

```java
	private int pasajeros;
	private int deposito;
	private int kpl;

	public Coche(int pasajeros, int deposito, int kpl) {
		this.pasajeros = pasajeros;
		this.deposito = deposito;
		this.kpl = kpl;
	}

	public int getPasajeros() {
		return pasajeros;
	}

	public void setPasajeros(int pasajeros) {
		this.pasajeros = pasajeros;
	}

	public int getDeposito() {
		return deposito;
	}

	public void setDeposito(int deposito) {
		this.deposito = deposito;
	}

	public int getKpl() {
		return kpl;
	}

	public void setKpl(int kpl) {
		this.kpl = kpl;
	}

	public int calcularAutonomia(Coche c) {
		int autonomia1 = deposito * kpl;
        int autonomia2 = c.deposito * c.kpl;

        return (autonomia1 > autonomia2) ? this : c;
	}

	public double gasofaNecesaria(int kilometros) {
		return 0;
	}
```
