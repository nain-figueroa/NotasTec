---
tags:
  - teoría
  - estructuraDeDatos
  - programación
---
Es una técnica de programación que nos permite que un bucle de instrucciones se ejecute $n$ veces. Reemplaza en ocasiones a estructuras repetitivas.

![[Recursión]]

***
### Condición de fin de recursividad
Cuando se implementa una función recursiva será preciso considerar una condición de terminación, ya que en caso contrario la función continuará indefinidamente llamándose a sí misma y llegaría un momento en que la pila de memoria que registra las llamadas se desbordaría.
***
### Ejemplo
##### Recursividad directa
```c#
public class Program {
	public static void Main() {
		recursiva();
	}
	
	public static void recursiva(){
		...
		recursiva();
	}
}
```
##### Recursividad indirecta
```c#
public class Program {
	public static void Main() {
		Recursiva();
	}
	
	public static void Recursiva(){
		...
		Recursiva2();
	}
	
	public class void Recursiva2(){
		...
		Recursiva();
	}
}
```
#### Impresión descendente de números
```c#
public class Program {
	public static void Main() {
		ImprimirNumeros();
		Console.ReadKey();
	}
	
	public static void ImprimirNumeros(Int32 nCantNumeros){
		if(nCantNumeros < 0){
			return;
		}
		Console.WriteLine(nCantNumeros.ToString());
		
		nCantNumeros--;
		ImprimirNumeros(nCantNumeros);
	}
}
```
