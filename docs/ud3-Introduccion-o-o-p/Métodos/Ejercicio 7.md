## Enunciado

Crea un ejemplo que combine sleep() y algún método static de Math o
Integer

## Solución

```java
import java.lang.Thread;
import java.lang.Math;

class test {
	    public static void main(String[] args){
	    	int n = 0;
	    	do {
	    		System.out.printf("%d %n", n);
	    		n = Math.addExact(n,1);
	    		try {
					Thread.sleep(1000);
				} catch (InterruptedException e) {
					e.printStackTrace();
				}
	    	} while(n < 60);
	    }
	}
```
