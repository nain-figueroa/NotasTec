---
tags:
  - teoría
  - estructuraDeDatos
  - programación
---
La complejidad de un algoritmo o complejidad computacional, **estudia los recursos y  esfuerzos requeridos durante el cálculo para resolver un problema** los cuales se dividen en: *tiempo de ejecución y espacio en memoria*.
El **factor tiempo**, por lo general es **más importante que el factor espacio**, pero existen algoritmos que ofrecen el peor de los casos en un menor tiempo que el mejor de los casos, lo cual no es la mejor de las soluciones.
El **factor tiempo** de un algoritmo **depende de la cantidad de datos que se quieren procesar.**
- *En computación al momento de realizar un programa se debe de obtener su algoritmo.*
- *Cada programador puede tener un método diferente de un mismo problema.*
- *Para ello está el análisis de algoritmos cuyo objetivo es: La búsqueda de algoritmos eficientes.*
***
#### Complejidad de algoritmos
La mayoría de los problemas que se plantean en la actualidad se pueden resolver con algoritmos que difieren en su eficiencia. Dicha diferencia puede ser irrelevante cuando el número de datos es pequeño pero cuando la cantidad es mayor la diferencia crece:
$$
\begin{align*}
1+2+3+4 = 10 &| 3 \hspace{4em} 3 | 4*(4+1)/2 = 10\\
&| \hspace{1em} tiempo \hspace{1em} |\\
1+2+ \dots + 10 = 55 &| 9 \hspace{4em} 9|10*(10+1)/2 = 55\\
\end{align*}
$$
***
### Complejidad en el tiempo
Definiciones:
- $T(n)$ Tiempo de ejecución del algoritmo.
- $F(n)$ Tiempo el introducir los datos al algoritmo

El tiempo en ejecución de un algoritmo: *Se refiere a la suma de los tiempos en los que el programa tarda en ejecutar una a una todas sus instrucciones.*
Tomando en cuenta que cada instrucción requiere una unidad de tiempo, dicho tiempo se puede calcular en función de $n$ (el número de datos), lo que se denomina $T(n)$.

Si hacemos un análisis de forma directa al programa para determinar el tiempo de ejecución del mismo, **debemos definir el conjunto de operaciones primitivas, que son independientes del lenguaje de programación que se use**. Algunas de las funciones primitivas son las siguientes:
- Asignación de un valor a una variable
- Llamada a un método
- Ejecución de una operación aritmética
- Comparar dos números
- Poner indices a un arreglo
- Retorno de un método
En forma especifica, **una operación primitiva corresponde a una instrucción en el lenguaje de bajo nivel**, cuyo tiempo de ejecución depende del ambiente de hardware y software, pero es constante.
