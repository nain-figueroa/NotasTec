---
tags:
  - teoría
  - mateDiscretas
  - programación
---
El sistema de numeración binario utiliza dos dígitos, el cero ( 0 ) y el uno ( 1 ).
De acuerdo a esta regla, el número binario 1111 tiene un valor que se calcula así:
$$
\begin{align*}
1 x 2³ + 1 x 2² + 1 x 2¹ + 1 x 2⁰ &= \\
1 x 8 + 1 x 4 + 1 x 2 + 1 x 1 &= \\
8 + 4 + 2 + 1 &= 15_{10}
\end{align*}
$$
y para expresar que ambos números son iguales, se escribe así:
$$1111_2 = 15_{10}$$
***
### Conversión entre números [[SISTEMA DECIMAL | decimales]] y binarios
Basta con realizar divisiones sucesivas entre 2 y escribir el resto obtenido de cada división y luego anotarlos de forma inversa a como se fueron obteniendo:
$$
\begin{align*}
77 / 2 = 38, Resto&: 1\\
38 / 2 = 19, Resto&: 0\\
19 / 2 = 9, Resto&: 1\\
9 / 2 = 4, Resto&: 1\\
4 / 2 = 2, Resto&: 0\\
2 / 2 = 1, Resto&: 0\\
1 / 2 = 0, Resto&: 1
\end{align*}
$$
Y tomando los restos de forma inversa nos queda:
$$77_{10} = 1001101_2$$
***
### Tamaño de las cifras binarias
Como regla general, con *n* dígitos binarios pueden representarse un máximo de *$2^n$* números. El número más grande que puede escribirse con *n* dígitos es una unidad menos.
***
### Conversión de binarios a [[SISTEMA DECIMAL | decimal]]
Basta con desarrollar el número, teniendo en cuenta el valor de cada dígito en su posición, que es el de una potencia de 2, cuyo exponente es 0 en el bit situado más a la derecha, y se incrementa en una unidad según vamos avanzando posiciones hasta la izquierda.
$$
\begin{array}{1}
1010011\\[1em]
1x2⁶ + 0x2⁵ + 1x2⁴ + 0x2³ + 0x2² + 1x2¹ + 1x2⁰\\
64 + 0 + 10 + 0 + 0 + 2 + 1\\[1em]
1010011_2 = 83_{10}
\end{array}
$$
