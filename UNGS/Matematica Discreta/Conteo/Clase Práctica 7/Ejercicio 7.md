## Probar Mediante El Principio De Inducción Las Siguientes Identidades

a) $1^3 + 2^3 + 3^3 + 4^3 + ..... + n^3 = \frac{n^2 \cdot (n+1)^2}{4}$

b) $1 \cdot 2^1 + 2 \cdot 2^2 + 3 \cdot 2^3 + ... + n · 2^n = 2 + 2^{n+1} \cdot (n − 1)$

c) $1 \cdot 1! + 2 \cdot 2! + ··· + n × n! = (n + 1)! − 1$

**Respuesta**

> [!NOTE] Mal
> En la sumatoria estan mal definidas las variables, el iterador tiene que ser otra letra

### **a)**

Sea $n \in \mathbb{N}$ y $P(n) = \displaystyle \sum_{n=1}^\mathbb{n} n^3 = \frac{n^2 \cdot (n+1)^2}{4}$

**Caso Base**

Queremos probar que $P(1)$ es verdadero

Por un lado tenemos

$$
1^3 = 1
$$

y por el otro

$$
\frac{1^2 \cdot (1+1)^2}{4} = \frac{1 \cdot 4}{4} = 1
$$

Como son iguales se verifica que $P(1)$ es verdadero.

**Paso Inductivo**

Sea $k \ge 1$ suponemos $P(k)$ es verdadero, es decir asumimos la siguiente igualdad:

$$
\displaystyle \sum_{n=1}^{k} n^3 = \frac{n^2 \cdot (n+1)^2}{4} \,\,\,\,\,\,\text{Hipótesis Inductiva}
$$

Queremos probar que $P(k + 1)$ es verdadero, es decir queremos probar que vale la siguiente igualdad

$$\displaystyle \sum_{n=1}^{k+1} n^3 = \frac{n^2 \cdot (n+1)^2}{4}$$

Calculemos la sumatoria:

$$  
\begin{aligned}
\displaystyle \sum_{n=1}^{k + 1} n^3 &=
\displaystyle \sum_{n=1}^{k} n^3 + (k +1)^3\\ \\ 
\text{H.I} &=\frac{n^2 \cdot (n+1)^2}{4} + (k +1)^3 \\ \\ 
&= \frac{n^2 \cdot (n+1)^2 + 4 \cdot(k +1)^3}{4}

\end{aligned}
$$ 
### **b)**

Sea $n_0 = 1$ y $P(n) = \displaystyle \sum_{i = 1}^{n} (i \cdot 2^i) = 2 + 2^{n + 1} \cdot (n - 1)$

Probamos la igualdad $\forall \,n \in \mathbb{N}$ usando el principio de inducción

**Caso base**

Queremos probar que $P(1)$ es verdadero

Notemos que:

$$
1 \cdot 2^1 = 2
$$

por otro lado tenemos:

$$
2 + 2^{1 + 1}\cdot(1 - 1) = 2 + 4 \cdot 0 = 2
$$

Como son iguales se comprueba que $P(1)$ es verdadero

**Paso Inductivo**

Sea $k \ge 1$ suponemos que $P(k)$ es verdadero, es decir asumimos que se cumple la siguiente igualdad.

$$
\displaystyle \sum_{i = 1}^{k} = (i \cdot 2^i) = 2 + 2^{k+1} \cdot (k - 1)
$$

$$H.I$$

Queremos probar que $P(k+1)$ es verdadero, es decir queremos decir que vale la siguiente igualdad:

$$
\displaystyle \sum_{i = 1}^{k+1} (i \cdot 2^i) = 2 + 2^{k+2} \cdot k = 2 + 2^k \cdot 2 \cdot k
$$

Calculemos la sumatoria

$$  
\begin{aligned}
\displaystyle \sum_{i = 1}^{k+1} 
&= \displaystyle \sum_{i = 1}^{k} (i \cdot 2^i) + (k+1) \cdot 2^{k+1}\\ \\
H.I &= \underline{2 + 2^{k+1} \cdot (k - 1)} + (k+1) \cdot 2^{k+1} \\ \\
&= 2 + 2^{k+1}\begin{bmatrix}(k-1) + (k+1) \end{bmatrix}\\ \\
&= 2 + 2^{k+1}\cdot (2\cdot k)\\ \\
&= 2 + 2^{k+1}\cdot 2\cdot k\\ \\
&= 2 + 2^{k+2}\cdot k\\ \\
\end{aligned}
$$Como $P(1)$ es verdadero y para todo $k\ge1$ es verdadero que $P(k) \Rightarrow P(k+1)$ entonces por principio de inducción  queda demostrado que $\forall n \in \mathbb{N}$ vale que:
$$

\displaystyle \sum_{i=1}^{n} (i \cdot 2^i) = 2 + 2^{n+1} \cdot (k - 1)

$$

### **c)**

Sea $n_0 = 1$ y $P(n) = \displaystyle \sum_{i = 1}^{n} (i \cdot i!) = (n + 1)! - 1$
Queremos probar la igualdad $\forall n \in \mathbb{N}$ usando el principio de inducción

**Caso Base**

Queremos probar que $P(1)$ es verdadero.

Notemos que tenemos:
$$1 \cdot 1! = 1$$
Por otro lado tenemos:
$$(1 + 1)! - 1 = 1$$
Como son iguales podemos asegurar que $P(1)$ es verdadero


**Paso Inductivo**

Sea $k \ge 1$ suponemos que $P(k)$ es verdadero, es decir asumimos que se cumple la siguiente igualdad:
$$\displaystyle \sum_{i = 1}^{k} (i \cdot i!) = (k + 1)! - 1$$
$$H.P $$
Queremos probar que $P(k+1)$ es verdadero, es decir que vale la siguiente igualdad:
$$\displaystyle \sum_{i = 1}^{k+1} (i \cdot i!) = (k + 2)! - 1$$
Calculemos la sumatoria

$$  

\begin{aligned}

\displaystyle \sum_{i=1}^{k+1}

&= \displaystyle \sum_{i=1}^{k} (i \cdot i!) + (k + 1) \cdot (k + 1)!\\ \\

H.I&= \underline{(k + 1)! - 1} + (k + 1) \cdot (k + 1)!

\end{aligned}

$$ 
