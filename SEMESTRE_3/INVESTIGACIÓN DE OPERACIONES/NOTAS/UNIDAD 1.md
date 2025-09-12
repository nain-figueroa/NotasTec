---
tags:
  - notas
  - investigaciónDeOperaciones
---
La investigación de operaciones es un disciplina en la que se aplican métodos matemáticos, análisis estadísticos y algoritmos para optimizar procesos y tomar decisiones en situaciones complejas.

Se origina en las segunda guerra mundial y ha evolucionado al punto de que aplica prácticamente en cualquier area donde se tengan que gestionar recursos y procesos.

>[!TIP] Historia
>- En 1776 **Gaspard Morge**, desarrolla la **programación geométrica**, que con el paso del tiempo pasaría a ser a Investigación de operaciones.
>- De 1939 a 1945, un grupo conocido como el "**Circulo de Blackett**" liderado por Patrick Blackett, fueron los **primeros** en **aplicar** la **investigación de operaciones**.
>- En 1947 **George Dantzig** desarrolla el algoritmo **simplex**.
>- de 1950 a 1970, **Narenda Karmakar** desarrolló algoritmos de **punto interior** aumentando las posibilidades de la programación lineal.

>[!TIP] Modelos
>Es un representación matemática de un problema real, en el que se simplifica lo posible, para tener un modelo más manejable, capturando todos los aspectos importantes.
>En si hay 4 componentes esenciales:
>- **Variables de decisión**: que son las incógnitas en el problema
>- **Función objetivo:** La expresión matemática que se va a maximizar o minimizar
>- **Restricciones:** Los limites a cumplir
>- **Parámetros:** Los valores que caracterizan al problema
>___
>#### Beneficios
>Permiten analizar diferentes escenarios, facilitan la toma de decisiones, proporciona insights e identifica cuellos de botella y posibles mejoras.
>___
>#### Tipos de modelos
>Se dividen por 3 condiciones
>##### Según la naturaleza de las variables
>En esta hay 2 tipos ya sean variables que son conocidas con certeza (**Deterministicos**) o  variables que incorporan incertidumbre y probabilidad, incluso aleatoriedad (**Estocástico**).
>##### Según sus relaciones matemáticas
>SI es que son **lineales** o **no lineales**
>##### Según las dimension temporal
>Donde se pueden considerar cambios temporales (**Dinámicos**) o donde no (**Estáticos**)

>[!NOTE] Modelo de programación lineal
>Se considera de los modelos más importantes debido a su simplicidad matemática y la disponibilidad de método de resolución eficientes.
>#### Caracteristicas
>Consta de 4 características fundamentales:
>- **Función objetivo lineal**
>todas las variables aparecen en primer grado y no hay productos entre ellas.
>- **Restricciones lineales**
>Todas se representan con ecuaciones o inecuaciones lineales
>- **No negatividad**
>No puede haber variables de decisión negativas
>- **Aditividad**
>La contribución total es la suma de contribuciones individuales
>[[MODELOS DE PROGRAMACIÓN LINEAL | -> Estructura matemática general ]]
>#### Visualización
>En si es una función objetivo que debe optimizarse dentro de las restricciones establecidas. La solución factible se encuentra dentro de esa región.
>#### Formulación
>- **1.- Identificar el problema**
>- **2.- Definir función objetivo**
>- **3.- Establecer restricciones**
>- **4.- Incorporar la no negatividad**

>[!NOTE] Método gráfico
>Es una forma gráfica de resolver problemas de programación lineal, con la limitación de que está limitada a 2 variables.
>**Procedimiento**
>- Se representa cada restricción como una linea
>- Se identifica la región factible
>- Se determinan puntos de intersección de la región
>- Se evalúa la función objetivo en cada vértice
>- Seleccionar el vértice que mejor optimiza la función
>#### Tipos de soluciones
>Al aplicar este método, pueden darse 4 situaciones:
>- Que la función objetivo alcance su valor optimo en único punto (**Solución optima**)
>- Que la función objetivo tenga multiples valores óptimos (**múltiples óptimas**)
>- Que no exista un valor óptimo finito (**No acotada**)(Usualmente es por una errónea formulación del modelo)
>- Que ningún punto satisfaga todas las restricciones (**Sin solución factible**)(Mayormente por una mala formulación de las restricciones)

>[!NOTE] Método simplex
>Este es un método iterativo que funciona para resolver métodos de programación lineal  con cualquier tipo de variable y restricciones.
>#### Principios fundamentales
>- El algoritmo se mueve de un vértice a otro de la región factible
>- Con cada vuelta se mejora la función objetivo
>- Se detiene cuando la función objetivo no se puede mejorar más
>#### Ventajas
>- **Capacidad para problemas complejos:** no importa la cantidad de variable y restricciones
>- **Base de software moderno**
>- **Eficiencia computacional**
>- **Flexibilidad y adaptabilidad**

>[!TIP] Sectores que usan programación lineal
>- Logística y transporte
>- Manufactura y producción
>- Finanzas e inversiones
>- Energía y recursos
>- Sector público
>- Telecomunicaciones

>[!TIP] [[INNOVACIÓN Y HERRAMIENTAS ACTUALES|->Modelos avanzados de programación lineal]]
