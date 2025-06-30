Probar la igualdad

$$ 
\displaystyle \sum_{k = 3}^{n} (k² - 5k - 3) = \frac{n(n-8) \cdot (n+2)}{3} + 16
$$

vale $\forall n \ge 3$. Hallar una fórmula cerrada para la sumatoria

$$\displaystyle \sum_{k = 1}^{n} (k²-5k+6) $$

**Respuesta**

Sea $n_0 = 3$ y $p(n) : \displaystyle \sum_{k = 3}^{n} (k² - 5k - 3) = \frac{n(n-8) \cdot (n+2)}{3} + 16$

**Caso base**

Queremos validar que $p(3)$ es verdadero.

Por un lado tenemos:

$$ 3² - 15 - 3 = -9 $$

y por el otro lado tenemos:

$$ \frac{3(3 - 8) \cdot (3 + 2)}{3} + 16 = \frac{\cancel{3} \cdot -5 \cdot 5}{\cancel{3}} + 16 = -25 + 16= -9$$

por lo tanto se verifica que $p(3)$ es verdadero

**Paso inductivo**

Sea $t \ge 3$ y suponemos que $p(t)$ es verdadero, es decir, asumimos que se cumple la siguiente igualdad:

$$ 
\displaystyle \sum_{k = 3}^{t} (k² - 5k - 3) = \frac{t(t-8) \cdot (t+2)}{3} + 16 $$
Queremos probar que $p(t + 1)$ es verdadero, es decir que vale la siguiente igualdad:

$$\displaystyle \sum_{k = 3}^{t + 1} (k² - 5k - 3) = \frac{(t + 1)\cdot(t-7) \cdot (t+3)}{3} + 16 $$
Calculemos la sumatoria:

$$\begin{aligned}
\displaystyle \sum_{k = 3}^{t + 1} (k² - 5k - 3)
&=\displaystyle \sum_{k = 3}^{t} (k² - 5k - 3) = (t + 1)² - 5(t + 1) - 3
\\
H.I&=\frac{t(t-8) \cdot (t+2)}{3} + 16  + (t + 1)² - 5(t + 1) - 3
\\
&=\frac{t(t-8) \cdot (t+2) + 3 \cdot (t + 1)² - 15(t + 1) - 9)}{3} + 16 
\\
&=\frac{t(t-8) \cdot (t+2) + 3 \cdot (t² + 2\cdot t + 1) - 15t + 15 - 9)}{3} + 16 
\end{aligned}
$$
**Calculo auxiliar**

$$\begin{aligned}
t(t-8) \cdot (t+2) + 3 \cdot (t² + 2\cdot t + 1) - 15t - 15 - 9) =\\
(t² - 8t) \cdot (t + 2) + 3t² + 6t + 3 - 15t - 24 =\\
t³ + 2t² - 8t² - 16t + 3t² + 6t - 15t - 21 =\\
t³ - 3t² - 25t - 21 = \\
\end{aligned}
$$ 
