## Sea $G$ El Siguiente Grafo

![[Diagrama Parcial 3.1.1.svg]]

Calcular $\alpha(G), \omega(G), \alpha(\overline{G}), \omega(\overline{G})$

**Respuestas**

Empecemos calculando $\alpha(G)$, busquemos a ojo un conjunto independiente del mayor tamaño posible, por ejemplo $\{ b, f, i, k \}$ es un conjunto independiente ya que tomados dos a dos no son vecinos entre sí, por lo tanto $\alpha(G) \ge 4$.

![[Diagrama Parcial 3.1.2.svg]]

Luego tomemos los siguientes subgrafos de $G$:

![[Diagrama Parcial 3.1.3.svg]]Veamos que $V(G) = V(G_1) \cup V(G_2) \cup V(G_3)$, por lo tanto vale la fórmula para calcular la cota superior de $\alpha(G)$

$$ \alpha(G) \le \alpha(G_1) + \alpha(G_2) + \alpha(G_3) $$

Calculemos los $\alpha$ de cada subgrafo de $G$:

- $\alpha(G_1) = 1$, pues $G_1 \cong K_4$
- $\alpha(G_2) = 1$, pues $G_2 \cong K_4$
- $\alpha(G_3) = 2$, pues $G_3 \cong C_5$

Reemplazamos los valores en la fórmula

$$\begin{aligned}
\alpha(G) &\le 1 + 1 + 2\\
\alpha(G) &\le 4\\
\end{aligned}
$$

Luego $\alpha(G) \le 4$, por lo tanto como previamente sabíamos que $\alpha(G) \ge 4$, se deduce que $\alpha(G) = 4$

---

Ahora pasamos a calcular $\omega(G)$, por ejemplo sea $T$ = $\{ a, b, g, h \}$ es un conjunto donde todos los vertices son vecinos entre sí, por definición de $\omega$, $T$ es una clique de tamaño 4, luego $\omega(G) \ge 4$.

Ahora si hubiera una clique de tamaño 5 en $G$, tendría que haber al menos 5 vértices de al menos grado 4
