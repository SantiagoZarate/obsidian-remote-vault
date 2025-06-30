## Determinar El Tamaño De Una Clique Máxima Y El Tamaño De Un Conjunto Independiente Máximo Para El Siguiente Grafo G

![[Diagrama Entrega 2.1.svg]]

**Respuesta**

Para calcular el tamaño de $\alpha(G)$ podemos definir los siguientes grafos $H_1$ y $H_2$ de $G$:

![[Diagrama Entrega 2.2.svg]]

Según la propiedad sabemos que $\alpha(G) \le \alpha(H_1) + \alpha(H_2)$, por lo tanto podemos saber la cota superior de $\alpha(G)$ si calculamos la suma del alfa de $H_1$ y $H_2$

- $\alpha(H_1)$ = 1, Observemos que $H_1$ es un $K_3$, el alfa de todo $K_n$ es 1
- $\alpha(H_2)$ = 2, Observemos que $H_2$ es un $P_3$, por lo tanto su alfa es $\frac{2 + 1}{n} = 2$

Luego 3 es la cota superior de $\alpha(G)$, por lo tanto $\alpha(G) \le 3$

Ahora tomemos el conjunto $\{ F, D, B \}$ y vemos ques un conjunto independiente de tamaño 3, por lo tanto $\alpha(G) \ge 3$.

Luego como $\alpha(G) \le 3$ y $\alpha(G) \ge 3 \Rightarrow \alpha(G) = 3$

---

Ahora para calcular $\omega(G)$ notemos que tenemos una clique de tamaño 3, conformada por los vertices $A, F, E$, por lo tanto $\omega(G) \ge 3$

Para ver si podemos encontrar una clique podemos analizar todos los posibles subconjuntos de vértices de tamaño 4 tal que sean clique.

| Subconjunto        | ¿Es clique? | Justificación   |
| ------------------ | ----------- | --------------- |
| $\{ A, F, E, D \}$ | No          | $D \not\sim  E$ |
| $\{A, F, E, C \}$  | No          | $C \not\sim A$  |
| $\{A, F, E, B \}$  | No          | $B \not\sim F$  |
| $\{A, F, D, C \}$  | No          | $C \not\sim F$  |
| $\{A, F, D, B \}$  | No          | $B \not\sim F$  |
| $\{A, F, C, B \}$  | No          | $B \not\sim F$  |
| $\{A, E, D, C \}$  | No          | $C \not\sim A$  |
| $\{A, E, D, B \}$  | No          | $B \not\sim D$  |
| $\{F, E, D, C\}$   | No          | $F \not\sim C$  |
| $\{F, E, D, B \}$  | No          | $F \not \sim B$ |
| $\{F, E, B, C \}$  | No          | $F \not \sim C$ |
| $\{E, B, C, D \}$  | No          | $E \not\sim C$  |
| $\{E, B, C, A \}$  | No          | $E \not\sim C$  |
| $\{A, B, C, D \}$  | No          | $A \not\sim C$  |
| $\{B, C, D, F \}$  | No          | $F \not\sim C$  |

Queda demostrado entonces que no existe una clique de tamaño 4, por lo tanto $\omega(G) \le 3$.

Luego como $\omega(G) \ge 3$ y $\omega(G) \le 3 \Rightarrow \omega(G) = 3$
