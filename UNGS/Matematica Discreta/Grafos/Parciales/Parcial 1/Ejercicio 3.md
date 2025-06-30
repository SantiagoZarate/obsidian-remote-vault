## Sea G Un Grafo Simple Con Exactamente Dos Componentes Conexas. Suponiendo Que Una Componente Conexa Es Isomorfa a $K_{10}$ Y la Otra a $K_{11}$

1. ¿Cuántas aristas tienen G ?
2. ¿Cuántos vértices y aristas tiene $\overline{G}$?
3. Mostrar que $\overline{G}$ es bipartito completo.

**Respuestas**

---
### **1:**

$|E(G)| = ?$

Obtener la cantidad de aristas de $G$ se resume a sumar la cantidad de aristas de cada una de las componentes conexas, en este caso tenemos componentes conexas isomorfas a grafos completos, y la cantidad de aristas de un grafo completo es $\begin{pmatrix} n \\ 2 \end{pmatrix}$

Entonces calculemos la cantidad de aristas de cada component conexa.

Sea la componente conexa 1 la isomorfa a $K_{10}$ la cantidad de aristas de la misma es $\begin{pmatrix} 10 \\ 2 \end{pmatrix} = \frac{10 \cdot 9}{2} = 45$

Sea la componente conexa 2 la isomorfa a $K_{11}$ la cantidad de aristas de la misma es $\begin{pmatrix} 11 \\ 2 \end{pmatrix} = \frac{11 \cdot 10}{2} = 55$

Luego $|E(G)| = 45 + 55 \Rightarrow 100$

---
### **2:**

La cantidad de vértices de $G$ y su complemento es la misma.

Para saber la cantidad de aristas de $\overline{G}$ sabemos que va a ser la cantidad de aristas máximas que puede tener $G$ con la condición que sea simple menos la cantidad de aristas de $G$, por que si una arista existe en un grafo, la misma no existe en su complemento y viceversa, para hallar dicha cantidad podemos usar la siguiente fórmula:

Como $|V(G)| = 21$, el grafo que se formaría al agregar todas las aristas posibles con la condición que siga siendo simple va a ser isomorfo a $K_{21}$

$$|E(\overline{G})| = |E(K_{21})| - |E(G)|$$

Como ya sabemos $|E(G)|$ nos queda por saber la cantidad de aristas de $K_{21}$ que sería el grafo que tendriamos si $G$ fuera completo.

$$|E(K_{21})| = \begin{pmatrix} 21 \\ 2 \end{pmatrix} = \frac{21 \cdot 20}{2} = 210$$

Luego reemplazamos los valores en la fórmula

$$\begin{aligned}
|E(\overline{G})| &= 210 - 100\\
|E(\overline{G})| &= 110\\
\end{aligned}
$$ Luego la cantidad de aristas del complemento de $G$ es 110.

---
### **3:**

Primero analicemos $G$, tiene dos conjuntos de vértices, un $K_{10}$ donde todos sus vértices son vecinos tomados de a pares, y $K_{11}$ que también cumple con esa condición.

También notar que no tiene aristas que vayan de un vértice de $K_{10}$ a un vértice de $K_{11}$, si hubiera, $G$ sería conexo.

entonces en su complemento tenemos que todos los vértices de $K_{10}$ son vecinos de con todos los vértices de $K_{11}$, y no existen aristas que tengan como extremos dos vértices de $K_{10}$  o $K_{11}$

Luego, por definición de grafo bipartito completo tenemos que $\overline{G}$ es bipartito completo, específicamente $K_{10,11}$ , ya que tiene dos conjuntos disjuntos de vértices de tamaño $10$ y $11$
