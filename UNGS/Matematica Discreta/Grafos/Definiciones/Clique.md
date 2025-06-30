## Definición

Una clique es un conjunto de vértices adyacentes de a pares, llamaremos $\omega(G)$ a la cantidad de vértices de una clique de $G$ de tamaño máximo

Ejemplo:

![[Diagrama Clique 1.1.svg]]

Posible conjuntos cliques

- $\{a, b \} \rightarrow$ Si es, de tamaño 2
- $\{a, c, d\} \rightarrow$ No es, $a \not\sim c$
- $\{a, b, d\} \rightarrow$ Si es, de tamaño 3
- $\{a, b, d, c\} \rightarrow$ No es, $a \not\sim c$

Luego $\omega(G) = 3$

---

Sea $H$ un grafo tal que:

- $|V(H)| = 57$
- $|E(H)| = 60$
- $\{v_1, v_2, v_3, v_4 \}$ es una clique de tamaño 4
- $H$ no tiene cliques de tamaño 5

Hallar $\omega(G)$

Notemos que si $C$ fuera una clique de tamaño $\gt$ 5 podría tomar 5 de sus vértices y forma un conjunto con ellos tal que todos sus vértices sean vecinos de a pares, es decir, podría formar una clique de tamaño 5.

Luego, por enunciado, no hay cliques de tamaño 5 o mayor, entonces $\omega(H) \le 4 \Rightarrow \omega(H) = 4$
