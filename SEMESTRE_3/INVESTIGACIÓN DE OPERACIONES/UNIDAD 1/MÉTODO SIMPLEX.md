---
tags:
  - teoría
  - investigaciónDeOperaciones
---
Es un algoritmo iterativo diseñado para resolver problemas de programación lineal con cualquier tipo de variables y restricciones.
***
## Principios fundamentales
- **Exploración sistemática**
El algoritmo se mueve de un vértice a otro de la región factible, mejorando el valor de la función objetivo en cada iteración.
- **Mejora iterativa**
En cada paso, se selecciona la variable que más contribuye a mejorar la función objetivo (variable entrante) y  se determina cuánto puede aumentar sin valor las restricciones.
- **Criterio de optimalidad**
El algoritmo se detiene cuando no se puede mejorar más la función objetivo, lo que garantiza haber encontrado la solución óptima.
***
##### Ventajas
- **Capacidad para problemas complejos**
Puede mejorar problemas con decenas, cientos o incluso miles de variables y restricciones, imposibles de resolver gráficamente. Problemas industriales reales con +500 variables son rutinariamente resueltos mediante implementaciones modernas del simplex.
- **Base de software moderno**
El algoritmo simplex forma la columna vertebral de prácticamente todas los solucionadores de programación lineal comerciales y de código abierto.
- **Eficiencias computacional**
Aunque en teoría puede requerir un número exponencial de iteraciones en el peor caso, en la práctica el simplex es sorprendentemente eficiente. La implementaciones moderna incorporan técnicas avanzadas como *presolving*, *scaling* y *stepest-edge pricing* para mejorar el rendimiento. 
- **Flexibilidad y adaptabilidad**
El método se ha extendido para mejorar variantes como programación entera, programación entera mixta y problemas de flujo de red.
Permite incorporar análisis de sensibilidad para evaluar el impacto de cambios en los parámetros del modelo.
___
##### Ejemplo
**Modelo matemático**
Maximizar $Z = 3.000S + 4.000T$
Sujeto a:
- $4S + 5T <= 200$ (tiempo)
- $100S + 200T <= 8.000$ (aluminio)
- $S >= 10$ (Demanda mínima sedanes)
- $T <= 30$ (Demanda máxima todoterrenos)
- $S,T >= 0$ (No negatividad)

##### Procedimiento simplex simplificado:
- Convertir todas las restricciones a igualdades introduciendo variables de holgura
- Formar tabla inicial del simplex
- Identificar la variable de entrada y salida
- Realizar operaciones de pivote hasta alcanzar la optimalidad

**Solución óptima**
Tras aplicar el algoritmo simplex, se obtiene:
- $S=15$ 
- $T=28$
- $Z=257.000€$ de beneficios máximos
Esta solución satisface todas las restricciones y no puede mejorarse más

##### Interpretación de resultados:
- La restricción de tiempo está activa (se utiliza todas las 200 horas disponibles)
- La restricción de aluminio está activa (se utilizan 6700 kg de los 800 disponibles)
- Se producen más sedanes que el mínimo requerido
- Los todoterreno no alcanzan el limite máximo