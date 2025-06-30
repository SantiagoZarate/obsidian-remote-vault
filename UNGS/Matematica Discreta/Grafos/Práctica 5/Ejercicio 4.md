## Encuentre El Tamaño Máximo De Una Clique Y El Tamaño Máximo De Un Conjunto Independiente En Los Grafos De Los Ejercicios 1 Y 2

**Respuesta**

### 1 - H)
- $\omega(H) = 4$
- $\alpha(H) = 2$

Haciendo uso de la propiedad, definimos los sub grafos $P_1$ y $P_2$ de $H$

![[Diagrama 4.1.svg]]

Como $P_1$ y $P_2$ son $C_3$ y $C_4$, la suma de sus $\alpha$ es igual a 2, por lo que mediante el principio, $\alpha(H) = 2$

Para hallar $\omega(H)$ seleccionamos un conjunto $\in V(G)$ a ojo, por ejemplo $\{ v_2, v_3, v_3, v_4 \}$, este conjunto forma una clique de tamaño 4, por lo tanto $\omega(H) \ge 4$

Observemos que si hubiera una clique de tamaño 5, tendrían que haber 4 vertices $v_i$ de $H$ tal que $d_H(v_i) \ge 4$, como no existen 4 vertices que cumplan esta condición aseguramos que $\omega(H) \le 4$

Luego como $\omega(H) \ge 4$ y $\omega(H) \le 4 \Rightarrow \omega(H) = 4$

### 1 - F)
- $\omega(F) = 3$
- $\alpha(F) = 2$

Para hallar $\alpha(F)$ seleccionamos el conjunto de vertices $\{ a, d \}$ y vemos que no son vecinos entre sí, por lo tanto podemos afirmar que $\alpha(F) \ge 2$, ahora si queremos agregar algún otro vértice a nuestra elección con la condición que se forme un conjunto independiente vemos que no es posible, ya que $a \sim c, a\sim b, a \sim e$ y a la vez $d \sim c, d \sim e, d \sim b$, por lo tanto $\alpha(F) \le 2$.

Luego como $\alpha(F) \ge 2$ y $\alpha(F) \le 2 \Rightarrow \alpha(F) = 2$

Para hallar $\omega(F)$ tomamos los vertices $a, b, e$ , como todos son vecinos entre sí podemos afirmar que $\omega(F) \ge 3$, luego vemos que no podemos tomar ninguno de los dos restantes vertices ya que el conjunto que se formaría no sería una clique, por lo tanto $\omega(F) = 3$

### 1 - G)

Definimos los siguientes sub grafos de $G$

![[Diagrama 4.2.svg]]

calculamos los $\alpha$ de cada sub grafo

$$\begin{aligned}
\alpha(H_1) = \alpha(K_3) = 1 \\
\alpha(H_2) = \alpha(C_6) = 3 \\
\alpha(H_3) = \alpha(K_3) = 1 \\
\end{aligned}
$$

La suma de los $\alpha$ de los sub grafos nos da la cota superior de $\alpha(G)$, es decir, la cota superior es 5

![[Diagrama 4.3.svg]]

==TODO==
