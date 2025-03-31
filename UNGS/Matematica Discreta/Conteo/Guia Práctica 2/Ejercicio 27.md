---
tags:
  - Combinación-Repetidos
status: Incomplete
---

## Se Tienen 25 Libros Para Repartir En Tres Pilas. Suponiendo Que la Primera Pila Debe Tener Más De 7 Libros, la Segunda Al Menos 5 Y la Tercera Como Mínimo 7

**a)** Suponiendo que los libros son todos iguales, ¿de cuántas formas distintas se pueden distribuir los libros en las tres pilas?

**b)** Suponiendo que los libros son todos distintos, ¿de cuántas formas distintas se pueden distribuir los libros en las tres pilas?

**Respuesta**

### **a)**

Teniendo en cuenta las restricciones para cada pila:

$$  
\begin{aligned}
\text{Cantidad de libros pila 1} \ge 8\\
\text{Cantidad de libros pila 2} \ge 5\\
\text{Cantidad de libros pila 3} \ge 7\\
\end{aligned}
$$

Del total de 25 libros, restamos 20 libros que se necesitan para satisfacer las restricciones mínimas de libros por pila, ahora nos quedan 5 quedan libros, que pueden ser seleccionados para ubicarse en una de las 3 pilas, por teorema 1 de combinatoria con elementos repetidos sabemos que esto es $C(7,2)$.

Entonces la cantidad de formas distintas de distribuir los libros en las tres pilas es $C(7,2)$

**b)**
