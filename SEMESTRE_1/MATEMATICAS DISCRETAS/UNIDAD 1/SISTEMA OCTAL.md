---
tags:
  - teoría
  - mateDiscretas
---
**Se representan los números mediante 8 dígitos: *0, 1 , 2, 3, 4, 5, 6, 7*.** El valor de cada una de las posiciones vienen determinado por las potencias base 8.
$$
\begin{array}{1}
273_8\\[1em]
2x8² + 7x8¹ + 3x8⁰\\
= 128 + 56 + 3\\
= 187_{10}
\end{array}
$$
***
### Conversión de [[SISTEMA DECIMAL | decimal]] a octal
Se usa la misma técnica que con la [[SISTEMA BINARIO | conversión a binario]], mediante divisiones sucesivas por 8 y colocando los restos obtenidos en orden inverso:
$$
\begin{array}{1}
122_{10}\\[1em]
122 / 8 = 15, Resto: 2\\
15 / 8 = 1, Resto: 7\\
1 / 8 = 0, Resto: 1\\[1em]
= 172_8
\end{array}
$$
