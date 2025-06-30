## Sea $G$ El Siguiente Grafo

![[Diagrama Parcial 4.1.1.svg]]

Calcular α(G), ω(G), α($\overline{G}$) y ω($\overline{G}$)

**Respuestas**

- Calculo de $\alpha(G)$ y $\omega(G)$

Empezamos buscando $\alpha(G)$ a ojo, el conjunto $T$ = $\{ a, c, e, h \}$ es conjunto independiente de tamaño 4, ya que tomados de a pares no son vecinos entre sí, luego por definición de $\alpha$, $T$ es un conjunto independiente de tamaño 4, por lo tanto $\alpha(G) \ge 4$

Tomemos los siguientes subgrafos de $G$:

![[Diagrama Parcial 4.1.2.svg]]Vemos que la union disjunta de los conjuntos de vértices de cada uno de los subgrafos es igual a $V(G)$, por lo que vale la fórmula para hallar la cota superior de $\alpha(G)$

$$ \alpha(G) \le \alpha(G_1) + \alpha(G_2) + \alpha(G_3) +\alpha(G_4)  $$

Ahora calculemos $\alpha$ de cada subgrafo

- $\alpha(G_1) = \alpha(G_2) = 1$, pues tanto $G_1$ y $G_2 \cong K_4$
- $\alpha(G_3) = 1$, pues $G_3 \cong K_3$
- $\alpha(G_4) = 1$, pues $G_4 \cong P_2$

Reemplazamos los valores en la fórmula.

$$\begin{aligned}
\alpha(G) &\le \alpha(G_1) + \alpha(G_2) + \alpha(G_3) +\alpha(G_4)\\
\alpha(G) &\le 1 + 1 + 1 + 1\\
\alpha(G) &\le 4\\
\end{aligned}
$$

Por lo tanto sabemos que $\alpha(G) \le 4$, como ya calculamos que $\alpha(G) \ge 4$, podemos deducir que $\alpha(G) = 4$

Luego $\omega(\overline{G}) = 4$, ya que si fuera mayor, eso significa que $G$ existe un conjunto independiente de tamaño mayor a 4, pero por lo calculado previamente se sabe que no es así.

---

Ahora calculamos $\omega(G)$, como en el calculo anterior encontramos un subgrafo que era una copia de $K_4$ eso significa que hay 4 vértices que tomados de a pares son vecinos todos entre sí, entonces por definición de $\omega$, existe una clique de tamaño 4, por lo tanto $\omega(G) \ge 4$.

Si existiera una clique de tamaño 5, eso significa que hay al menos 5 vértices de al menos grado 4 en $G$ y que tomados de a pares son vecinos, vemos que los vértices $e$ y $d$ no cumplen con la cantidad de grados, por lo tanto plantear el grafo $G - \{e, d, h\}$

![[Diagrama Parcial 4.1.3.svg]]

Luego vemos que en $G - \{e , g, h \}$ no hay 5 vértices de al menos grado 4, por lo tanto no existe una clique de tamaño 5, por lo tanto $\omega(G) \lt 5$, es decir $\omega(G) \le 4$.

Entonces como ya habíamos encontrado una clique de tamaño 4, y sabemos que $\omega(G) \le 4$, podemos deducir que $\omega(G) = 4$


