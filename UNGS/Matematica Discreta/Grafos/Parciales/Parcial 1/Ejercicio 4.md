## Calcule El Tamaño De Una Clique Máxima Y El Tamaño De Un Conjunto Independiente Máximo, Del Siguiente Grafo

![[Diagrama Parcial 4.1.svg]]

**Respuesta**

- $\alpha(G) = ?$
- $\omega(G) = ?$

Para calcular $\alpha(G)$ empecemos buscando un conjunto independiente del mayor tamaño posible a ojo, por ejemplo $\{ a, h, i, e \}$ es un conjunto ind. de tamaño 4, ya que

- $a \not\sim h$
- $a \not\sim i$
- $a \not\sim e$
- $h \not\sim i$
- $h \not\sim e$
- $i \not\sim e$

Por lo tanto podemos afirmar que $\alpha(G) \ge 4$.

Ahora tomemos los siguientes subgrafos de $G$

![[Diagrama Parcial 4.2.svg]]

Vemos que la unión disjunta de los conjuntos de vértices de cada uno de los subgrafos es igual a $V(G)$, por lo que podemos usar el principio para obtener la cota superior de $\alpha(G)$

$$ \alpha(G) \le \alpha(G_1) + \alpha(G_2) +\alpha(G_3) $$

Ahora calculemos el $\alpha$ de cada subgrafo.

- $\alpha(G_1) = 1$, pues $G_1 \cong K_4$
- $\alpha(G_2) = 2$, pues $G_2 \cong C_5$
- $\alpha(G_3) = 1$, pues $G_3 \cong P_2$

Reemplazamos los valores en la fórmula anterior

$$\begin{aligned}
\alpha(G) &\le \alpha(G_1) + \alpha(G_2) +\alpha(G_3) \\
\alpha(G) &\le 1 + 2 +1 \\
\alpha(G) &\le 4 \\
\end{aligned}
$$

Entonces encontramos la cota superior para $\alpha(G)$, que es 4

Luego como $\alpha(G) \le 4$ y sabemos que $\alpha(G) \ge 4 \Rightarrow \alpha(G) = 4$
