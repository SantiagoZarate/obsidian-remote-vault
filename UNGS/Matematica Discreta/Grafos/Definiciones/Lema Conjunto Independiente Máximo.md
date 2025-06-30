## Definición

*(Sirve para encontrar la cota superior de $\alpha(H)$)*

Sea $G$ un grafo simple. si $H$ y $R$ son subgrafos de $G$ tales que $V(G) = V(H) \cup V(R)$ entonces $\alpha(G) \le \alpha(H) + \alpha(R)$

Ejemplo:

![[Diagrama Lema CIM 1.1.svg]]

$\alpha(G) = ?$

$J = \{a, d, f, h \}$

$J$ es un conjunto ind. de tamaño 4, luego $\alpha(G) \ge 4$

Sugerimos los siguientes subgrafos $H_i$ de $G$ con $1 \le i \le 4$

![[Diagrama Lema CIM 1.2.svg]]$$V(H_1) \cup V(H_2) \cup V(H_3) \cup V(H_4) = V(G)$$

$$\begin{aligned}
\alpha(G) &\le \alpha(H_1) +  \alpha(H_2) +  \alpha(H_3) +  \alpha(H_4) \\
\alpha(G) &\le 1 + 1+ 1+ 1\\
\alpha(G) &\le 4\\
\end{aligned}
$$

Luego como $\alpha(G) \le 4$ y $\alpha(G)\ge 4 \Rightarrow \alpha(G) = 4$
