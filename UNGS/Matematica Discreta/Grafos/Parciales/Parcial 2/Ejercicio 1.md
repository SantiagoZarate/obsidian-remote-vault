## Sea G El Siguiente Grafo

![[Diagrama Parcial 2.1.1.svg]]

a) Hallar el tamaño de una clique máxima y el de un conjunto independiente máximo.

b) Mostrar un subgrafo inducido por ocho vértices que contenga exactamente una arista de corte y al menos dos vértices de corte.

**Respuestas**

### **a)**

- $\alpha(G) = ?$
- $\omega(G) = ?$

Empecemos calculando $\alpha$ de $G$, busquemos a ojo un conjunto independiente del mayor tamaño posible, por ejemplo $\{ a, j, g \}$ es un conjunto independiente de tamaño 3, pues:

- $a \not\sim j$
- $a \not\sim g$
- $j \not\sim g$

Por lo tanto podemos afirmar que $\alpha(G) \ge 3$.

Luego tomemos los siguientes subgrafos de $G$

![[Diagrama Parcial 2.1.2.svg]]

Notemos que la unión disjunta de todos los vértices de cada uno de los subgrafos es igual a $V(G)$, por lo tanto podemos usar el principio para obtener la cota superior de $\alpha(G)$

$$\alpha(G) \le  \alpha(G_1) + \alpha(G_2) + \alpha(G_3)$$

Pasemos a calcular el $\alpha$ de cada subgrafo

- $\alpha(G_1)$ = 1, pues $G_1 \cong K_4$
- $\alpha(G_2)$ = 1, pues $G_2 \cong K_5$
- $\alpha(G_3)$ = 1, pues $G_3 \cong K_5$

Reemplazamos los valores en la fórmula

$$\begin{aligned}
\alpha(G) &\le  \alpha(G_1) + \alpha(G_2) + \alpha(G_3)\\
\alpha(G) &\le  1 + 1+  1\\
\alpha(G) &\le  3\\
\end{aligned}
$$
Entonces sabemos que $\alpha(G) \le 3$. Luego como ya vimos que $\alpha(G) \ge 3 \Rightarrow \alpha(G) = 3$

---

Ahora pasemos a calcular $\omega(G)$, busquemos a ojo una clique del mayor tamaño posible, por ejemplo, los vértices $\{ e, f, g, h, i \}$ forman una clique de tamaño 5, pues todos los vértices de ese conjunto son vecinos entre sí tomados de a pares.

Por lo tanto podemos afirmar que $\omega(G) \ge 5$.

Supongamos que existe una clique tamaño mayor a 5, por ejemplo una de tamaño 6, eso significaría que $G$ tiene al menos 6 vértices de al menos grado $5$, por ejemplo llamemos $T$ al conjunto de vértices de al menos grado 5 que es el siguiente: $\{ d, j, k, n, e, g, j \}$

### **b)**

