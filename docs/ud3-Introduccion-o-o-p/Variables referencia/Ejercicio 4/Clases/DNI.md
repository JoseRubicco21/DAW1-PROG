## Código

```java
public class DNI {
	char letra;
	int num;
	
	
	
	public char getLetra() {
		return letra;
	}



	public void setLetra(char letra) {
		this.letra = letra;
	}



	public int getNum() {
		return num;
	}



	public void setNum(int num) {
		this.num = num;
	}



	@Override
	public String toString(){
		return (String.format("%08d%s",0, Integer.toString(num) + Character.toString(letra)));
	};
}
```