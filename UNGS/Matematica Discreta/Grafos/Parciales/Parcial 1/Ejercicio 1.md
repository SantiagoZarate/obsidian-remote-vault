## Considere El Siguiente Grafo Y Calcule El Tamaño De Una Clique Máxima Y El Tamaño De Un Conjunto Independiente Máximo

![[Diagrama Parcial 1.1.svg]]

- $\omega(G)= ?$
- $\alpha(G)= ?$

Calculemos primero $\alpha(G)$, busquemos a ojo un conjunto de vértices que no sean vecinos entre sí del mayor tamaño posible, por ejemplo el conjunto $\{ e, f, g, h \}$ es un conjunto independiente de tamaño 4, ya que $e \not\sim f,  e \not\sim g, e \not\sim h, f \not\sim g, f \not\sim h$ y $g \not\sim h$. Por lo tanto sabemos que $\alpha(G) \ge 4$.

Ahora definamos los siguientes subgrafos de $G$.

![[Diagrama Parcial 1.2.svg]]

Luego como la unión disjunta de los vértices de los anteriores subgrafos es igual a $V(G)$ {$V(G_1) \cup V(G_2) \cup V(G_3) \cup V(G_4) = V(G)$} podemos usar la fórmula para conocer la cota superior de $\alpha(G)$.

$$\alpha(G) \le \alpha(G_1) + ... + \alpha(G_4) $$

Luego como cada uno de los subgrafos son isomorfos a $K_4$, $\alpha(G_n) = 1$, ahora podemos reemplazar ese valor en la fórmula.

$$\begin{aligned}
\alpha(G) &= 1 + 1+ 1 + 1\\
\alpha(G) &= 4\\
\end{aligned}
$$

Se observa que cualquier otra elección de subgrafos de $G$ que permita utilizar la propiedad anterior nos da como resultado la misma cota o una cota superior.

Entonces $\alpha(G) \le 4$, luego como ya sabemos que $\alpha(G) \ge 4$ y $\alpha(G) \le 4 \Rightarrow \alpha(G) = 4$

