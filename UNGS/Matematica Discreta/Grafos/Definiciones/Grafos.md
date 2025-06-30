## Definición

Un grafo $G$ es una terna formada por:

- Un conjunto de vértices $V(G)$
- Un conjunto de aristas $E(G)$
- una relación que asocia a cada arista dos vértices (no necesariamente distintos)

$|V(G)|$ = Cantidad de vértices del grafo $G$

$|E(G)|$ = Cantidad de aristas del grafo $G$

## Grafo Simple

1) Las **aristas múltiples** son aquellas que tienen el mismo par de extremos.
2) Un **bucle** es una arista cuyos extremos coinciden

Si un grafo $G$ no tiene bucles ni aristas múltiples se llama **grafo simple**

## Grafo Nulo

Se llama grafo nulo a aquel grafo que la cantidad de vértices es nula.

## Grado

El grado de un vértice $v$ en un grafo $G$, anotado $\delta_G(v)$ es el número de aristas incidentes en $v$, con la excepción de cada bucle se cuenta dos veces.

El grado máximo de un grafo se denota por $\Delta(G)$ y el grado mínimo del grafo por $\delta(G)$

![[Diagrama Grafos 1.1.svg]]

- $|V(G)| = 6$
- $|E(G)| = 7$
- $|\Delta(g)| = 5$
- $|\delta(g)| = 0$

$$\begin{aligned}
d(A) &= 2\\
d(B) &= 5\\
d(C) &= 2\\
d(D) &= 4\\
d(E) &= 1\\
d(F) &= 0\\
\end{aligned}
$$ 
## Vértices Aislados

Los vértices cuyos grados es 0 se denominan vértices aislados.
