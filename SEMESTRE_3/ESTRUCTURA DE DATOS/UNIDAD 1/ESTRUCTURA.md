---
tags:
  - programación
  - estructuraDeDatos
---
Es un [[Tipos de Datos Abstractos| tipo de dato abstracto]] de uno o más elementos, cada uno de los cuales puede ser un tipo de dato diferente.
- Cada elemento se denomina miembro.
- La cantidad de miembros es ilimitada.
- También se les llama registros.
***
## Definición
Antes de poder usar una estructura es necesario definirla:
```c++
struct nombre_estructura {
	tipo_dato nombre_miembro_1;
	...
	tipo_dato nomber_mienbro_n;
};
```

*Solo se especifica el nombre y el formato,, no se reserva espacio en memoria como tal.*
***
## Declaración de variables
Se pueden declarar variables de dos forma, como cualquier otra o después de definir la estructura.
```c++
struct nombre_estructura {
	tipo_dato nombre_miembro_1;
	...
	tipo_dato nomber_mienbro_n;
}estructa1, estructura2, estructuraN;
//O
nombre_estructura estructura1;
```
***
## Inicializar variables
Una forma es inicializarla al declararla, colocando los valores dentro de las llaves.
```c++
struct nombre_estructura {
	tipo_dato nombre_miembro_1;
	...
	tipo_dato nomber_mienbro_n;
}estructa1 = {dato1, ..., dato_n};
//O
nombre_estructura estructura1 = {dato1, ..., dato_n};
```
***
## Acceso a miembros
Una vez declarada una variable de tipo estructura, podemos acceder a los miembros de dicha variable:
**Hay dos formas de acceder:**
- Por el operador punto  ( . ) => Directo.
- Por el operador puntero ( -> ) => Indirecto.
***
#### EJEMPLO
```c++
struct persona {
	string nombre;
	int edad;
}persona_1 = {"Goku", 40};

persona persona_2 = {"Vegeta", 42};
cout << persona_1.nombre << endl; // => "Goku"
cout << persona_2->nombre << endl; // => "Vegeta"
```
