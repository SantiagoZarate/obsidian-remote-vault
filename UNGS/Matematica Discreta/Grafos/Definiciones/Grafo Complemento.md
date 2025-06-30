## Definición

Sea $G$ un grafo simple su complemento notado $\overline{G}$ es el grafo simple cuyo conjunto de vértices es $V(G)$ y su conjunto de aristas como $uv \in E(\overline{G})$ si y solo sí $uv \notin E(G)$

![[Diagrama Grafo Complemento 1.1.svg]]

- $|V(\overline{G})|$ = $\{a, b, c\}$
- $|E(\overline{G})|$ = $\{ab\}$

## Observaciones

- $|V(G)| = |V(\overline{G})|$
- $|E(G)| + |E(\overline{G})| = \begin{pmatrix} n \\ 2 \end{pmatrix}$ (La cantidad de aristas si fuera $K_n$)

---

¿Cuál es el máximo número de aristas que podemos tener en un grafo simple de $N$ vértices?

Sea $G$ un grafo simple tal que $V(G) = \{ v_1, ..., v_2\}$

Como cada arista la puedo asociar a dos vértices distintos el problema se transforma en ¿De cuantas maneras puedo elegir dos vértices?

La respuesta es $\begin{pmatrix} N \\ 2 \end{pmatrix}$
