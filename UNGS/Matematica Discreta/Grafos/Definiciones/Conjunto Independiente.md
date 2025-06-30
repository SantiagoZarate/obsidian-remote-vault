Definición

Un conjunto independiente en un grafo $G$ es un subconjunto de $V(G)$ tal que sus elementos no son vecinos de a pares.

Llamaremos $\alpha(G)$ al tamaño máximo de los conjuntos independientes en $G$

Ejemplo:

![[Diagrama Conjunto Independiente 1.1.svg]]

Posibles conjuntos independientes

- $\{a, b\} \rightarrow$ No es, son vecinos
- $\{a, e\} \rightarrow$ Si es, de tamaño 2
- $\{a, b, d\} \rightarrow$ No es, $a \sim b$
- $\{a, e, d\} \rightarrow$ Si es, de tamaño 3

Veamos si hay algún conjunto de tamaño mayor a 3

$\alpha(G) \ge 3$

Como tengo 5 vértices, a lo sumo puedo tener un conj. ind. de tamaño 5, es decir $\alpha \le 5$, notemos que $V(G)$ no es un conjunto independiente pues $a \sim b$, luego $\alpha(G) \le 4$ (Básicamente no puede ser 5 porque hay al menos una arista)

Notemos que $c \sim e, c \sim b, c \sim d$ luego si $c$ forma parte de un conj. ind. el mismo será de tamaño menor a 4.

Luego el restante candidato a conj. ind. de tamaño 4 es $\{a, b, d, e \}$ pero $a \sim b$ con lo que no es un conj. ind.

Finalmente $\alpha(G) \le 3$

Como $\alpha(G) \le 3$ y $\alpha(G) \ge 3 \Rightarrow \alpha(G) = 3$
