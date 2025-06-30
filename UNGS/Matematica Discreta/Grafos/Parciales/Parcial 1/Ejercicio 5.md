## Decidir la Verdad O Falsedad De Las Siguientes Afirmaciones. Justificar En Cada Caso

1. Sea $G$ un grafo simple y 2-regular, entonces $G$ es un ciclo. *falso*
2. Sea $G$ un grafo simple tal que $α(G)$ = 5 entonces $G$ es bipartito. *falso*
3. Sea $G$ un grafo simple con al menos una arista y tal que no tiene ningún subgrafo inducido de tres vértices que sea isomorfo a $C_3$. Entonces ω(G) = 2. *Verdadero*
4. Todo grafo $G$ 4-regular con 7 vértices se puede descomponer en copias de $P_4$.*falso*
5. Todo grafo bipartito con siete vértices tiene un conjunto independiente de tamaño al menos 4. *verdadero (Palomar)*
6. Si el grafo bipartito completo $K_{n,m}$ tal que $n ≥ 2$y $m ≥ 2$ contiene un recorrido cerrado que pasa por todas sus aristas, entonces $n = m$. *falso*
7. Si el grafo bipartito completo $K_{n,m}$ tal que $n ≥ 2$ y $m ≥ 2$ cumple que $n < m,$ entonces contiene un ciclo que pasa por todos los vértices del grafo.
8. Si un grafo $G$ se puede descomponer en dos grafos $H$ y $R$ , y $G$ tiene una cantidad impar de aristas, entonces $H$ o $R$ deben tener un número impar de aristas.
9. Sea $G$ un grafo simple con al menos dos vértices y exactamente un ciclo impar, entonces existe al menos un vértice $v$ en $G$ tal que $G − v$ es bipartito y tiene al menos una arista.
10. Sea $G$ un grafo conexo, entonces todo subgrafo inducido de $G$ es conexo.
11. Todo subgrafo de un grafo bipartito es bipartito.
12. Los grafos simples con al menos una arista que no es de corte tienen por lo menos tres aristas que no son de corte.
13. Los grafos conexos sin aristas de corte que tienen al menos una arista tienen todos su vértices de grado al menos 2.
14. Sea G un ${X;Y }$-bigrafo tal que $|X| ≥ |Y|$, entonces $α(G) = |X|$.
15. Todo subgrafo de un grafo sin aristas de corte es un grafo sin aristas de corte.
16. Sea G un grafo que no es un ciclo pero contiene un ciclo que pasa por todos sus vértices, y además $α(G) = 5$, entonces G tiene al menos 10 vértices y al menos 11 aristas.
17. Si $G$ es un grafo simple tal que $|V(G)| = 25$ y $|E(G)| = 200$ entonces $G$ es isomorfo a un grafo completo.

**Respuesta**

### **1**: Falso

![[Diagrama Parcial 5.1.svg]]

> [!NOTE] Title
> Notemos que G es un grafo simple 2- regular pero no es un ciclo ya que no se pueden ordenar en ronda los siete vértices del grafo G tal que cada vértice sea adyacente al siguiente en la ronda.

---
### **2**: Falso

*Preguntar*

Como contra ejemplo tenemos tenemos un $C_{11}$, cuyo $\alpha$ = 5, pero no es bipartito por ser ciclo impar.

Puede ser que un $C_{10}$ cumpla con la afirmación.

> [!NOTE] Title
> Si G es un grafo tal que α(G) = 5, resulta entonces que ω(G) = 5, luego G contiene como subgrafo una clique de tama ̃no 5, es decir, K5 es un subgrafo de G. Resulta entonces que G contiene ciclos impares (longitud 3 y longitud 5), luego por la caracterizaci ́on de los grafos bipartitos, G no es bipartito.

---
### **3:** Verdadero

Sabemos que $\omega(G)$ = 2 ya que $G$ contiene al menos una arista, los vertices adyacentes a esa arista forman una clique de tamaño 2 ya que sabemos que $G$ es simple.

si $\omega(G)$ fuera mayor a 2, eso quiere decir que $G$ tiene como subgrafo una copia de $C_3$ , luego por afirmación sabemos que $G$ no contiene dicho subgrafo, por lo tanto la afirmación es verdadera.

---
### **4**: Falso

Si hubiera una descomposición de $G$ en $P_4$'s eso significaría que la cantidad de aristas de $G$ es un número múltiplo de 3 ya que en este caso, cada uno de los $P_4$ tiene 3 aristas.

Sabemos que $G$ es 4-regular, y tiene 7 vértices, luego por TAM sabemos que tiene 14 aristas.

Luego como 14 no es múltiplo de 3, no existe dicha descomposición.

> [!NOTE] Title
> Supongamos que G se descompone en k ∈ N copias de P4. En dicho caso, se debe verificar que la suma de las aristas de los subgrafos de la descomposici ́on debe ser la cantidad de aristas del grafo G, es decir, se debe cumplir que 3 · k = 14. Notemos que esto es falso ya que 14 no es m ́ultiplo de 3. La contradicci ́on provino de suponer que G se puede descomponer en copias de P4, por lo tanto queda justificado que no es posible descomponer un grafo 4-regular con 7 v ́ertices en copias de P4.

---

### **5:** Verdadero (Palomar)

> [!NOTE] Resolucion del profe
> Si G es un grafo bipartito, tiene una bipartición {X, Y }, es decir, X ∪Y = V (G) , X ∩Y = ∅ y X e Y son conjuntos independientes. Por otro lado cada vértice de G debe pertenecer al conjunto X o bien al conjunto Y , luego por el principio generalizado del palomar, al menos 4 vértices pertenecen a uno de los dos conjuntos independientes. Resulta entonces que G tiene un conjunto independiente de tamaño al menos 4.

---

### **6:** Falso

*Preguntar*

*El profe dió un contra ejemplo con un $K_{2,4}$, pero nosotros probamos el caso donde $n = m$

Como contra ejemplo tenemos $K_{3,3}$ que no admite un recorrido cerrado que pase por todas sus aristas, ya que por *teorema de euler*, si eso sucediera, todos los vértices del grafo deberían ser de grado par, en esto ejemplo, es un grafo 3-regular.

---
### **7:** Falso

---
### **8:** Si Un Grafo $G$ Se Puede Descomponer En Dos Grafos $H$ Y $R$ , Y $G$ Tiene Una Cantidad Impar De Aristas, Entonces $H$ O $R$ Deben Tener Un Número Impar De Aristas

Verdadero

Sabemos que la cantidad de aristas de $G$ es igual a la suma de $|E(H)|$ y $|E(R)|$, ya que al ser una descomposición, cada una de las aristas de $G$ puede aparecer en un único subgrafo de la lista de descomposición.

Sabemos que $G$ tiene una cantidad impar de aristas, para que esto suceda, $H$ o $R$ deben tener una cantidad impar de aristas, ya de que si ambos tienen una cantidad impar de aristas, $G$ tendría una cantidad par de aristas.

En el caso de que $H$ y $R$ tengan una cantidad par de aristas, $G$ tendría una cantidad par de aristas.

Dejándonos el único escenario donde solo uno de los dos subgrafos tenga una cantidad impar de aristas.

> [!NOTE] Title
> Luego, si un n ́umero impar es suma de dos enteros, claramente uno es impar y el otro es par, por lo tanto H o R deben tener un n ́umero impar de aristas.

---

### **9:** Sea $G$ Un Grafo Simple Con Al Menos Dos Vértices Y Exactamente Un Ciclo Impar, Entonces Existe Al Menos Un Vértice $v$ En $G$ Tal Que $G − v$ Es Bipartito Y Tiene Al Menos Una Arista

*Preguntar*

> [!NOTE] Title
> El grafo G es simple con al menos dos vértices y exactamente un ciclo impar. Sea uv ∈ E(G) tal que además es una de las aristas del ́unico ciclo impar contenido en G. Eliminemos de G uno de los dos v ́ertices u o v. Al eliminar un vértice recordemos que también se eliminan las aristas que inciden en dicho vértice, por lo tanto, en este caso se elimina la arista uv que pertenece al ́unico ciclo impar en G. Obtenemos así el grafo G − v que no contiene ning ́un ciclo impar, luego por la caracterizaci ́on de los grafos bipartitos, G − v es bipartito.Falta probar que el grafo G − v tiene al menos una arista. Esto es fácil de justificar ya que el grafo de menor longitud que sea un ciclo impar simple es un C3. Luego al eliminar uno de sus vértices del ciclo, el subgrafo obtenido contiene al menos una arista del ciclo impar, por lo tanto el grafo G − v tiene al menos una arista.

![[Diagrama Parcial 5.9.svg]]

---

### **10:** Sea $G$ Un Grafo Conexo, Entonces Todo Subgrafo Inducido De $G$ Es Conexo

Falso

Como contraejemplo si tomamos el subgrafo inducido por el conjunto de vértices T = $\{a, d \}$, como resultado tenemos un grafo disconexo ya que no existe un camino que contenga como extremos a $a$ y $d$

![[Diagrama Parcial 5.10.svg]]

---

### **11:** Todo Subgrafo De Un Grafo Bipartito Es Bipartito

*Preguntar*

*Si se puede usar como caracterizacion*

---

### **12:** Los Grafos Simples Con Al Menos Una Arista Que no Es De Corte Tienen Por Lo Menos Tres Aristas Que no Son De Corte

Verdadero.

Las aristas son de corte si y solo si, no forman parte de un ciclo, luego los grafos simples con al menos una arista que no es de corte, contienen como mínimo un $C_3$ ya que es el ciclo más pequeño que se puede formar respetando la condición de que el grafo sea simple, luego la cantidad de aristas de un $C_3$ es 3, y ninguna es de corte.

### **13:**

---

3) b - Todo subgrafo de K5 que no es isomorfo a K5, es planar.

*Preguntar*

Si puedo armar un subgrafo con los mismos vértices pero quitando alguna arista, tengo entendido que si los vértices están presentes en el subgrafo, y en el grafo original había una arista, esa arista tiene que estar presente en el subgrafo.

Ver si lo planteado por nosotros, Al ser un grafo no isomorfo a $K_5$ ni $K_{3,3}$ por observacion de grafos planares, tiene sentido, o combiene hacerlo como lo hizo el profe, mostrando el caso donde eliminar una arista, y el caso donde elimina un vértice y justificando que los subgrafos de grafos planares siguen siendo planares.
