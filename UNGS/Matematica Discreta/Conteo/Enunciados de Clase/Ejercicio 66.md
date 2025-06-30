Demostrar que para todo $n$ natural vale que:

$$ \displaystyle \sum_{i = 1}^{n} (3\cdot i + 5) =
\frac{n\cdot(3n + 13)}{2}$$
**Respuesta**

Sea $n_0 = 1$ y $p(n) = $\displaystyle \sum_{i = 1}^{n} (3\cdot i + 5) =\frac{n\cdot(3n + 13)}{2}$ 
**Caso Baso**

Queremos verificar que $P(1)$ es verdadero

por un lado tenemos;
$$ 3 \cdot 1 + 5 = 8 $$
y por el otro lado:
$$ \frac{3 + 13}{2} = 8 $$
como ambos son iguales, entonces se cumple que $p(1)$ es verdadero


**Paso Inductivo**
Sea $k \ge 1$, suponemos que $p(k)$ es verdadero, es decir asumimos que se cumple la siguiente igualdad:

$$ \displaystyle \sum_{i = 1}^{k} (3\cdot i + 5) =
\frac{k\cdot(3k + 13)}{2}$$
$$ Hipótesis Inductiva $$

Queremos probar que $p(k+1)$ es verdadero, es decir que se cumple que:
$$ \displaystyle \sum_{i = 1}^{k+1} (3\cdot i + 5) =
\frac{(k + 1)\cdot(3\cdot(k+1) + 13)}{2}
= \frac{(k + 1)\cdot(3k + 16)}{2}
= \frac{3k² + 16k + 3k + 16}{2}$$
Verifiquemos la sumatoria:
$$\begin{aligned}
\displaystyle \sum_{i = 1}^{k+1}
&= \displaystyle \sum_{i = 1}^{k} (3\cdot i + 5)
+ (3\cdot (k+1) + 5)
\\
H.I&= \underline{\frac{k\cdot(3k + 13)}{2}} + (3\cdot (k+1) + 5)
\\
&= {\frac{k\cdot(3k + 13)}{2}} + (3k+ 8)
\\
&= {\frac{k\cdot(3k + 13) + 2 \cdot (3k+ 8)}{2}}
\\
&= {\frac{3k^2 + 13k + 6k + 16}{2}}
\end{aligned}
$$

Como $P(1)$ es verdadero y para todo $k \ge 1$ es verdadero que $p(k) \Rightarrow p(k+1)$ entonces por el principio de inducción queda demostrado que $\forall n \in \mathbb{N}$ vale que

$$ \displaystyle \sum_{i = 1}^{n} (3\cdot i + 5) =
\frac{n\cdot(3n + 13)}{2}$$
