
## Determinar Si Las Siguientes Afirmaciones Son Verdaderas O Falsas. Justifique En Cada Caso

**a)** Todo grafo bipartito conexo con al menos tres vértices y una cantidad par de aristas es euleriano.

**b)** Si $G$ es un grafo simple que no posee vértices de grado 1, entonces G no es un bosque.

**c)** Sea $G$ planar tal que $|V (G)| ≥ 3$ y $|E(G)| ≤ 2|V (G)| − 4$ entonces G es bipartito.

**d)** El grafo $G$ es planar si y sólo si al agregar una arista de corte a G se obtiene un grafo $G^{`}$ que también es planar.

**Respuesta**

### **a)**

Falso, como contra ejemplo tenemos un $P_3$, es bipartito conexo con una cantidad par de aristas, sin embargo no es euleriano ya que por ejemplo no tiene todos sus vértices de grado par, en concreto los vértices extremos de $P_3$ son de grado 1.

### **b)**

Falso, como contra ejemplo podemos tener $G$ tal que tenga un solo vértices aislado, el mismo no posee vértices de grado 1, es simple y sin embargo es bosque ya que no hay ciclos.

### **c)**

### **d)**

Verdadero, como la arista que agregamos es de corte, $G^{`}$ no va a generar un ciclo a partir de esa arista, por lo tanto no cabe la posibilidad de que $G^{`}$ sea una subdivision de $K_5$ o $K_{3,3}$, Luego por teorema de ... $G^{`}$ sigue siendo planar

Otra forma de justificarlo seria que la arista de corte que se agrega va a ser con un vértice aislado, o con un vértice perteneciente a una componente conexa distinta, por lo tanto $G^{'}$ sigue siendo planar.
