---
tags:
  - teoría
  - investigaciónDeOperaciones
---
Un método gráfico es una técnica visual para resolver problemas de programación lineal que involucran exactamente dos variables de decisión. Aunque su aplicabilidad práctica es limitada, proporciona una comprensión intuitiva de los conceptos fundamentales que se extienden a problemas más complejos.

##### Procedimiento
- Representa gráficamente cada restricción como una línea en un plano cartesiano
- Identificar la región factible (área que satisface todas las restricciones)
- Determinar las vértices (puntos de intersección) de la región factible
- Evaluar la función objetivo en cada vértice
- Seleccionar el vértice que optimiza la función objetivo
***
### Tipos de soluciones
- **Solución Optima**
La función objetivo alcanza su valor óptimo en un único punto (vértice) de la región factible, es el caso más común en aplicaciones prácticas.

Características: *Las líneas de nivel de la función objetivo tienen una pendiente distinta a cualquier restricción activa en la solución.*

- **Soluciones múltiples óptimas**
La función objetivo alcanza el mismo valor óptimo en múltiples puntos, típicamente a lo largo de una arista de la región factible.

Características: *La pendiente de la función objetivo coincide exactamente con la pendiente de una restricción activa*.

- **Solución no acotada**
La función objetivo puede mejorar indefinidamente dentro de la región factible. No existe un valor óptimo finito.

Implicación: *Generalmente indica errores con la formulación del modelo, ya que la mayoría de los problemas reales tienen limitaciones naturales*.

- **Problema sin solución factible**
No existe ningún punto que satisfaga simultáneamente todas las restricciones, la región factible está vacía. 

Causas: *Restricciones contradictorias o mal formuladas. Requiere revisar y reformular el modelo*.