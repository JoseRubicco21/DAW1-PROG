## Diagrama de Clase:

Este diagrama de clase esta como referencia para más adelante, por ahora no os preocupeis mucho con esto, es para dar una visión general de la clase. Se puede decir que es como un "Índice"

```mermaid
classDiagram
    note for Direccion "Asumimos que existe un método Getter y Setter para cada atributo"
    class Direccion {
        -pais: String
        -ciudad: String
        -provincia: String
        -tipoVia: String
        -calle: String
        -numeroDeVivienda: int
        Direccion()
        Direccion(pais: String, ciudad: String, provincia: String, tipoVia: String, calle: String, numeroDeVia: int)
        +toString() String
        +crearDireccion(Scanner) Direccion
    }
```
## Atributos

### pais

- Modificador de acceso: private (Privado)
- Descripción: Un atributo de tipo *String* que guardará el país de un Objeto Direccion

### ciudad

- Modificador de acceso: private (Privado)
- Descripción: Un atributo de tipo *String* que guardará el país de un Objeto Direccion

### provincia

- Modificador de acceso: private (Privado)
- Descripción: Un atributo de tipo *String* que guardará la provincia de un Objeto Direccion

### tipoVia

- Modificador de acceso: private (Privado)
- Descripción: Un atributo de tipo *String* que guardará el tipo de via de un Objeto Direccion

### calle

- Modificador de acceso: private (Privado)
- Descripción: Un atributo de tipo *String* que guardará la calle de un Objeto Direccion

### numeroDeVia

- Modificador de acceso: private (Privado)
- Descripción: Un atributo de tipo *int* que guardará el número de via de un Objeto Direccion

## Métodos

### Constructores

#### Direccion()

- Modificador de acceso: public (Público)
- Parametros: N/A
- Sobrecarga / Sobreescritura: Si (Sobrecarga)
- Dato de retorno: N/A
- Descripción: Constructor por defecto utilizado para crear un objeto Direccion vacío. Este constructor es utilizado en métodos como crearDirección para inicializar un Objeto donde se guardaran los datos. 

#### Direccion(String p, String ci, String pro, String tpv, String ca, int nvi)

- Modificador de acceso: public (Público)
- Parametros: String p, String ci, String pro, String tpv, String ca, int nvi
- Sobrecarga / Sobreescritura: Si (Sobrecarga)
- Dato de retorno: N/A
- Descripción: Constructor que se utiliza si queremos crear un objeto Direccion con todos sus datos.

### Métodos no constructores

#### toString()

- Modificador de acceso: public (Público)
- Parametros: N/A
- Sobrecarga / Sobreescritura: Si (Sobreescritura)
- Dato de retorno: String
- Descripción: Método que sobreescribe el método toString() existente con los datos del objeto. La sobreescritura viene denotada por el *decorador* "@". 

#### crearDireccion(Scanner scanner)

- Modificador de acceso: public (Público)
- Parametros: Scanner (Objeto)
- Sobrecarga / Sobreescritura: No
- Dato de retorno: Direccion (Objeto)
- Descripción: Método que crea una dirección a partir de los datos introducidos por el teclado. Estos datos del teclado salen del objeto Scanner que se le ha pasado como parametro. [Información del parametro Scanner en este método](../Descripción%20del%20programa.md#m%C3%A9todos-creardireccion-crearcientifico-crearproyecto)

#### Diagrama de flujo de funcionamiento:
```mermaid
flowchart TD
    start([Método es Invocado]) --> 
    scAssignation[Se asigna el Scanner pasado como parametro a la variable sc] --> scAskPais[Se pregunta por el pais al usuario] --> paisIsValid{Tipo de dato válido?}

    paisValid[Se rellena con los datos introducidos por el usuario]
    paisNotValid[Queda vacio]
    scAskProvincia[Se pregunta por la provincia]
    
    paisIsValid -- Si --> paisValid --> scAskProvincia
    paisIsValid -- No --> paisNotValid --> scAskProvincia

    scAskProvincia --> provinciaIsValid{Tipo de dato válido?} 

    scAskCiudad[Se pregunta por la ciudad]
    provinciaIsValid -- No --> provinciaValid[Queda vacio] --> scAskCiudad
    provinciaIsValid -- Si --> provinciaNotValid[rellenado con datos del usuario] --> scAskCiudad -. Se repite para todos los atributos .->

    scAskNVI[Se pregunta por el número de vivienda] -->
    scNVIIsValid{Tipo de dato?}
    scNVIValid[rellenado con datos del usuario]
    scNVINotValid[Queda vacio]

    scNVIIsValid -- Si --> scNVIValid --> return
    scNVIIsValid -- No --> scNVINotValid --> return

    return([Se devuelve el valor del los datos introducidos como un objeto de dirección])
```


## Código fuente:

```java
package proyecto_cientifico;

import java.util.Scanner;

public class Direccion {

	private String pais;
	private String ciudad;
	private String provincia;
	private String tipoVia;
	private String calle;
	private int numeroDeVivienda;
	
	public Direccion(String p, String ci, String pro, String tpv, String ca, int nvi) {
		pais = p;
		ciudad = ci;
		provincia = pro;
		tipoVia = tpv;
		calle = ca;
		numeroDeVivienda = nvi;
	}

	public Direccion() {
		
	}
	
	public String getPais() {
		return pais;
	}

	public void setPais(String pais) {
		this.pais = pais;
	}

	public String getCiudad() {
		return ciudad;
	}

	public void setCiudad(String ciudad) {
		this.ciudad = ciudad;
	}

	public String getProvincia() {
		return provincia;
	}

	public void setProvincia(String provincia) {
		this.provincia = provincia;
	}

	public String getTipoVia() {
		return tipoVia;
	}

	public void setTipoVia(String tipoVia) {
		this.tipoVia = tipoVia;
	}

	public String getCalle() {
		return calle;
	}

	public void setCalle(String calle) {
		this.calle = calle;
	}

	public int getNumeroDeVivienda() {
		return numeroDeVivienda;
	}

	public void setNumeroDeVivienda(int numeroDeVivienda) {
		this.numeroDeVivienda = numeroDeVivienda;
	}
	
	@Override
	
	public String toString() {
		return "\t\t\tPais: " + getPais() +"\n\t\t\tProvincia: " + getProvincia() + "\n\t\t\tCiudad: " + getCiudad() + "\n\t\t\tCalle: " + getTipoVia() + ", " + getCalle() + ", " + getNumeroDeVivienda();
	}
	
	public Direccion crearDireccion(Scanner scanner) {
		
		Scanner sc = scanner;
		
		System.out.println("Introduzca el pais: ");
		setPais(sc.nextLine());
		
		System.out.println("Introduca la provincia: ");
		setProvincia(sc.nextLine());
		
		System.out.println("Introduzca la ciudad: ");
		setCiudad(sc.nextLine());
		
		System.out.println("Introduzca el tipo de via: ");
		setTipoVia(sc.nextLine());
		
		System.out.println("Introduzca el nombre de la calle: ");
		setCalle(sc.nextLine());
		
		System.out.println("Introduzca el número de la vivienda");
		setNumeroDeVivienda(Integer.parseInt(sc.nextLine()));
		
		return this;
	}
}

```