## Sea G Un Grafo Conexo Con 8 Aristas, Exactamente 6 Vértices De Grado 1, Al Menos Un Vértice De Grado 3, Sin Vértices De Grado 5 Y Exactamente Un Vértice De Grado Par. ¿Cuántos Vértices Tiene G Y Cuáles Son Los Grados De Los Vértices Restantes?

**Respuesta**

Como $G$ es un grafo, entonces vales el T.A.M, es decir:

$$ \sum_{v\in V(G)}^{} d(v) = 2 \cdot |E(G)|$$

por enunciado, $|E(G)| = 8$, luego:

$$ \sum_{v\in V(G)}^{} d(v) = 16$$

Por enunciado tomemos $v_1, ..., v_6$ vértices de grado 1, $v_7$ vértice de grado par.

Luego reemplazamos los valores para formar la siguiente ecuación:

$$\begin{aligned}
6 \cdot 1 + X + 3 \cdot Y &= 16\\
X + 3 \cdot Y &= 16 - 6\\
X + 3 \cdot Y &= 10
\end{aligned}
$$

Siendo $X$ un número par e Y la cantidad de vértices de grado 3. Luego la única combinación de valores que satisfacen esa ecuación es $X = 4$ e $Y = 2$

Notemos que $|V(G)| = 9$ (los 6 de grado 1, 2 de grado 3 y 1 de grado par)
