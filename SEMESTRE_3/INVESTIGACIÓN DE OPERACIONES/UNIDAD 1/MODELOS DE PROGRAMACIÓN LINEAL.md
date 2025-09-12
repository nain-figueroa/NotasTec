---
tags:
  - investigaciónDeOperaciones
  - teoría
---
**Constituyen la clase más importante** y ampliamente aplicada de modelos en la investigación de operaciones **debido a su relativa simplicidad matemática y la disponibilidad de métodos de resolución eficientes.**

### Características fundamentales
- Función objetivo lineal:
*Busca maximizar o minimizar una expresión matemática donde todas las variables aparecen en primer grado y no hay productos entre ellas.*
- Restricciones lineales:
*Todas las limitaciones del problema se expresan mediante ecuaciones o inecuaciones lineales.*
- No negatividad:
*Generalmente las variables de decisión deben ser no negativas.*
- Proporcionalidad:
*La contribución de cada variable es directamente proporcional a su valor.*
- Aditividad:
*La contribución total es la suma de las contribuciones individuales*.
***
>[!NOTE] Estructura matemática general
>##### Maximizar / Minimizar
>$$
>\begin{array}{1}
>Z = C_1X_1 + C_2X_2 + ... + C_nX_n
>\end{array}
>$$
>##### Sujeto a las restricciones
>$$
>\begin{array}{1}
>a_11X_1 + a_12X_2 + ... a_1nX_n <= b_1 \\[1em]
>a_12X_1 + a_22X_2 + ... a_2nX_n <= b_2 \\[1em]
>... \\[1em]
>a_m1X_1 + a_m2X_2 + ... + a_mnX_n <= b_m
>\end{array}
>$$
>##### Y a las restricciones de no negatividad
>$$
>\begin{array}{1}
>X_1,X_2,...,X_n >= 0
>\end{array}
>$$


#### Visualización
Se caracterizan por una función objetivo que debe optimizarse dentro de una región factible formada por las restricciones. La solución óptima se encuentra en uno de los vértices de esta región.
___
#### Formulación
La formulación precisa del modelo matemático es el primer paso crucial en el proceso de resolución de problemas mediante investigación de operaciones.

Una formulación  puede llevar a soluciones óptimas para el modelo pero inútiles para el problema real.

 ### Pasos
- **1.- Identificar el problema**
Determine las incógnitas fundamentales cuyo valor óptimo debe encontrarse. Las variables deben ser medibles y controlables para el decisor.

Ejemplo: *En un problema de producción, las variables pueden ser la cantidad de cada producto a fabricar ( $x_1,x_2,...,x_n$ ).*

- **2.- Definir la función objetivo**
Formule la expresión matemática que representa el objetivo a optimizar ( maximizar beneficios, minimizar costes, etc ).

Ejemplo: *Si $C_1,C_2,...,C_n$, son beneficios por unidad, la función objetivo sería $Z = C_1X_1, C_2X_2, ..., C_nX_n$.*

- **3.- Establecer las restricciones**
Identifique todas las limitaciones que afectan a las variables de decisión y expreselas como ecuaciones o inecuaciones lineales.
**Tipos comunes:** Restricciones de recursos ( tiempo, materiales, mano de obra ), restricciones de demanda, restricciones técnicas o regulatorias.

- **4.- Incorporar condiciones de no negatividad**
En la mayoría de los problemas reales, las variables no pueden tomar valores negativos, por lo que se añaden restricciones de no negatividad: $x_1 >= 0, x_2 >= 0, ..., x_n >= 0$.
___
>[!NOTE] EJEMPLO PRÁCTICO
>Una planta automotriz fabrica dos modelos de vehículos: sedanes ( S ) y todoterreno ( T ). La dirección desea determinar cuantas unidades de cada modelo a producir para maximizar el beneficio total.
>
>**Datos del problema**
>- Beneficio: *3.000 € por sedán y 4.000 € por todoterreno*.
>- Tiempo disponible: *4 horas por sedán y 5 horas por todoterreno.*
>- Consumo de aluminio: *100 kg por sedán y 200 kg por todoterreno.*
>- Aluminio disponible: *8.000 kg semanales.*
>- Demanda mínima: *Al menos 10 sedantes semanales.*
>- Demanda máxima: *No más de 30 todoterrenos semanales.*
>**Formulación matemática**
 >- **Variables:** S = *Número de sedanes*, T = *Número de todoterreno*
 >- **Función objetivo:** Maximizar $Z = 3.000S + 4.000T$ 
 >- **Restricciones:** 
>	 - Tiempo: *$4S + 5T <= 200$*
>	 - Aluminio: *$100S +  200T <= 8.000$*
>	 - Demanda mínima sedanes: *$S >= 10$*
>	 - Demanda máxima todoterreno: *$T <= 30$*
>	 - No negatividad: *$S, T >= 0$*

***
>[!NOTE] Formas de resolución
>- [[MÉTODO GRÁFICO]]
>- [[MÉTODO SIMPLEX]]
