---
tags:
  - teoría
  - estructuraDeDatos
  - programación
---
Un módulo es una **secuencia léxicamente continúa de instrucciones que se encuentra limitado por elementos de fronteras** y además se caracteriza por disponer de un nombre o identificador.
Es aquel que **está constituido por una o varias instrucciones físicamente contiguas y lógicamente encadenadas**, las cuales **se pueden referenciar mediante un nombre**  y pueden ser llamadas desde diferentes puntos del programa.

Un módulo puede ser:
- Un programa
- Una función
- Una subrutina (procedimiento o función).

La modularidad se basa en la descomposición de un problema en una serie de subproblemas, dividiendolo en pequeños módulos.
$$''DIVIDE\hspace{1em}Y \hspace{1em}VENCERAS''$$
Esta división exige la existencia de un módulo que se denomina *principal* o *base*, y su función es que controle a todos lo demás.
*Mayormente es todo los lenguajes, este módulo es conocido como método main o Main*. Este coordina las llamadas a los módulos secundarios y pasas los datos necesarios en forma de parámetros.
***
## Principios para asegurar diseños modulares
- **Pocas interfaces** 
Cada módulo debe de comunicarse con tan pocos como sea posible.
- **Interfaces pequeñas (Acoplamiento débil)**
Si dos módulos se comunican, deben intercambiar la menor información posible.
- **Interfaces explicitas**
Si dos módulos se comunican, debe estar claro en el texto de uno o de ambos.
- **Ocultación de información**
Toda la información de un módulo debe ser privada.