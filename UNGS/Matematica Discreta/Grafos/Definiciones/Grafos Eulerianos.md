Si $G$ es un [[Grafo Disconexo]] y por lo menos dos componentes conexas tienen aristas entonces el grafo no puede tener un [[Recorrido Eulereano]]

![[Diagrama Grafos Euleriano 1.1.svg]]

## Definición 2

Sea $G$ un grafo. Un camino en $G$ es *maximal* si no está contenido en otro camino en $G$ más largo.

Un grafo es euleriano si contiene un recorrido euleriano cerrado.

**Lema 1** Si todo vértice de un grafo $G$ tiene grado al menos 2, entonces $G$ contiene un ciclo, es decir

$\delta(G) = 2$, $G$ contiene un ciclo

**Demostración**

Sea $G$ un grafo tal que $d(v) \ge 2$ para todo $v \in V(G)$. Como $G$ tiene vértices con grado distinto de cero, entonces $E(G)$ no es vacío. Sea $e$ una arista de $G$

Si $e$ es un bucle, entonces $G$ contiene un ciclo de longitud 1.

Si $e$ no es un bucle, entonces es un camino de dos. Este camino es maximal o se puede extender a uno maximal en $G$. Llamaremos $P$ a este camino maximal en $G$ Sea $u$ uno de los extremos de $P$,
