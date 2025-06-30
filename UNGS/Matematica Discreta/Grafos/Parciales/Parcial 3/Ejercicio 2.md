## Sea $G$ El Grafo Del Ejercicio 1

a) Decidir si $G$ tiene recorrido euleriano. ¿Cuántas aristas como mínimo se le deben agregar a $G$ para que el grafo resultante sea euleriano?

b) ¿Cuántas aristas se le deben eliminar a G para que el grafo resultante sea un árbol? ¿Hay m ́as de una cantidad?

**Respuestas**

### **a)**

$G$ no tiene recorrido euleriano pues, esto lo sabemos gracias al corolario de Euler, si tuviera recorrido euleriano, $G$ a lo sumo tendría 2 vértices de grado impar, no es el caso en este grafo ya que $a, f, e$ y $d$ tienen grado impar.

Como mínimo se debería agregar dos aristas para que el grafo resultante sea euleriano, por ejemplo una arista que tenga como extremos a $f$ y $e$, e y otra con extremos $a, d$, de esta manera todos los vértices del grafo resultante tendrían grado par, y al ser conexo, por teorema de Euler, el grafo resultante sería euleriano.

### **b)**

Sabemos que un árbol de $n$ vértices tiene $n-1$ aristas, en este caso si queremos obtener grafo árbol a partir de $G$, sabemos que $G$ tiene 11 vértices y 20 aristas, por lo tanto habría que eliminar 10 aristas para que el grafo resultante sea un árbol.

No hay más de una cantidad, pero si hay más de un conjunto de aristas elegidas a eliminar, pero eso no viene al caso.
