Demostrar para todo $n \in \mathbb{N}$ tal que:

$$ 5^n \ge 2^n + 3^n $$

Sea $n = 1$ y $P(n) = 5^n \ge 2^n + 3^n$

**Caso Base**

Notemos que es cierto que $5¹ \ge 2¹ + 3¹$, luego $P(1)$ es verdadero

**Paso Inductivo**

Sea $k \le 1$, suponemos que $P(k)$ es verdadero, es decir, asumimos que vale que $5^k \ge 2^k + 3^k$ $(H.I)$

Luego queremos probar que $P(k+1)$ es verdadero, es decir, queremos probar que

$$ 5^{k+1} \ge 2^{k+1} + 3^{k+1}$$

Veamos la justificación:

$$  
\begin{aligned}
5^{k + 1} &= 5^k  \cdot 5 \ge (2^{k} + 3^{k}) \cdot 5\\
&= 5^k  \cdot 5 \ge 2^{k} \cdot 5 + 3^k \cdot 5\\
\end{aligned}
$$
**Cálculos auxiliares**

Notemos que $(I)$

$$\begin{aligned}
5 &\ge 2\\
5 \cdot 2^k &\ge 2 \cdot 2^k\\
\end{aligned}
$$

Por otro lado $(II)$

$$  
\begin{aligned}
5 &\ge 3\\
5 \cdot 3^k &\ge 3 \cdot 3^k
\end{aligned}
$$

$$  
\begin{aligned}
(I) &= a \ge b\\
(II) &= c \ge d\\
(III) &= a + c \ge b + d\\
\end{aligned}
$$ 

luego se tiene que:

$$ 5\cdot 2^k  + 5 \cdot 3^k \ge 2 \cdot 2^k + 3 \cdot 3^k $$
