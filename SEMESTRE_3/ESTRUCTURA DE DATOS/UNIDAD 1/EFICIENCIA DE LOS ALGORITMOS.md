---
tags:
  - estructuraDeDatos
  - teoría
  - programación
---
Para que un algoritmos sea eficiente debemos tener en cuenta el tiempo de ejecución  y la cantidad de memoria que va a requerir para funcionar.
Aunque el problema se pueda resolver de varias maneras debemos optar por implementar la solución más eficiente, es decir, la que se realice en el menor tiempo posible y con la menor cantidad de memoria.
***
#### Complejidad en el espacio
Se refiere a la **memoria que utiliza el un programa para su ejecución**; Es decir el espacio de memoria que ocupan todas las variables propias del programa.
Para calcular **memoria estática**, se **suman la cantidad de memoria que ocupan cada una de las variables declaradas en el programa**. Dicha memoria se divide en [[Memoría estática| memoria estática]] y [[Memoria Dinámica| memoria dinámica]].
El **cálculo** de la **memoria dinámica**, no es tan simple ya que **depende de cada ejecución del programa o algoritmo** y el tipo de estructuras dinámicas que estén utilizando.

#### Selección de un algoritmo
Una de las **características primordiales** en la selección de un algoritmo es que **este sea sencillo de entender, calcular, codificar y depurar**, así mismo que **utilice eficientemente los recursos de la computadora y se ejecute con la mayor rapidez posible** con un eficaz uso de memoria dinámica  y estática.
También para seleccionar correctamente el mejor algoritmo es necesario realizar preguntas:
- **¿Que grade de orden tendrá la información que vas a manejar?**
Entra más desordenada esté la información, el algoritmo debe ser más robusto.
- **¿Que cantidad de datos vas a manipular?**
Una cantidad muy grande puede hacer prohibitivo utilizar un algoritmo que requiera de mucha memoria adicional.
- **¿Qué tipo de datos quieres ordenar?**
Alguno algoritmos solo funcionan con un tipo específico de datos (enteros, enteros positivos, etc) y otros son aplicables a cualquier tipo de dato.
- **¿Que tamaño tienen los registros de tu lista?**
Algunos algoritmos realizan múltiples intercambios. si los registros son de gran tamaño estos intercambios son lentos.