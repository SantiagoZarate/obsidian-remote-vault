## Dado El Siguiente Grafo $G$

![[Diagrama Parcial 2.4.1.svg]]

a) Decidir si $G$ es planar

b) Decidir si $G$ tiene recorrido euleriano. ¿Cuál es la mínima cantidad de aristas que hay que agregar para que el grafo resultante sea euleriano?

**Respuestas**

### **a)**

Veamos si $G$ es planar usando la fórmula.

$$ |E(G)| \le 3 \cdot |V(G)| - 6 $$

Reemplazamos los valores

$$\begin{aligned}
11 &\le 3 \cdot 7 - 6\\
11 &\le 21 - 6\\
11 &\le 15\\
\end{aligned}
$$

Se cumple la desigualdad, por lo tanto no podemos afirmar que $G$ no sea planar,

**b)**

![[Diagrama Parcial 2.4.2.svg]]

$G$ tiene recorrido euleriano, por ejemplo.

$$ \{ a, e_1, b, e_2, c, e_3, f, e_4, g, e_5, b, e_6, d, e_7, e, e_8, a, e_9,g, e_{10}, d, e_{11}, e, e_{12}, c \} $$

Vemos que el recorrido contiene todas las aristas de $G$ sin repeticiones, por lo tanto es un recorrido euleriano

La mínima cantidad de aristas que hay que agregar para que el grafo resultante sea euleriano es 1, en concreto una arista que tenga como extremos a $a$ y $c$, de esa forma el grafo resultante tendría todos sus vértices de grado par, y al ser conexo, por teorema de Euler, el grafo resultante sería euleriano.

