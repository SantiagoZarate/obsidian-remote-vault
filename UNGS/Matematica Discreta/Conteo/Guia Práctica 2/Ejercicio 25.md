## En Un Negocio Se Venden Cajas De Cartas, Cada Caja Tiene 30 Cartas Elegidas Entre 7 Tipos Distintos, Con Al Menos 2 Del Tipo 1, Al Menos 3 Del Tipo 2, Al Menos 3 Del Tipo 3 Y Más De 5 Del Tipo 7. ¿Cuántas Cajas Distintas Se Pueden Armar?

Nota: No importa el orden de las cartas en cada caja

**Respuesta**

Tengamos en cuenta las siguientes restricciones

$$  
\begin{aligned}
\text{Tipo 1} &\ge 2\\
\text{Tipo 2} &\ge 3\\
\text{Tipo 3} &\ge 3\\
\text{Tipo 7} &\ge 8\\
\end{aligned}
$$

Del total de cartas , que era 30, restamos las 16 cartas que se necesitan como mínimo para cumplir las restricciones, por lo que nos quedan 14 cartas por seleccionar de 7 tipos distintos, por teorema de combinatoria con elementos repetidos, en este caso siendo el tipo de carta que se puede repetir, sabemos que esto es igual a $C(20, 6)$

Luego la cantidad de cajas distintas que se pueden armar es $C(20,6)$
