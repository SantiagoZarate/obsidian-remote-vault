---
tags:
  - Inclusión-Exclusión
  - Ecuación-Linear
status: Done
---

## Contar El Número De Soluciones Enteras no Negativas De la Ecuación

$$r + s + t + u = 35$$

bajo las restricciones

$$  
\begin{aligned}
2 \lt r \le 5\\
4 \lt s \lt 22\\
3 \le u \lt 7
\end{aligned}
$$ 
**Respuesta**

Reescribamos las restricciones de la siguiente manera:

$$  
\begin{aligned}
3 \le r \le 5\\
5 \le s \le 21\\
3 \le u \le 6
\end{aligned}
$$

Realizamos una corrección a cada variable para que la cota inferior sea 0.

$$  
\begin{aligned}
0 \le r - 3 \le 2\\
0 \le s - 5 \le 16\\
0 \le u - 3 \le 3
\end{aligned}
$$

definimos las siguientes variables:

$$  
\begin{aligned}
a &= r - 3\\
b &= s - 5\\
c &= u - 3\\
d &= u
\end{aligned}
$$ 

Reescribimos la ecuación:

$$  
\begin{aligned}
a + b + c + d &= (r - 3) + (s - 5) + (u - 3)\\
a + b + c + d &= (r + s + u) - (3 + 5 + 3)\\
a + b + c + d&= 35 - 11\\
a + b + c + d&= 24\\
\end{aligned}
$$ 

Definimos el conjunto $S$ cuyos elementos son las soluciones a la ecuación anterior en $\mathbb{Z} \ge 0$, definimos las siguientes propiedades:

$$  
\begin{aligned}
p_1 &= a \gt 2\\
p_2 &= b \gt 5\\
p_3 &= c \gt 6\\
\end{aligned}
$$

y los subconjuntos $A_i$ de $S$ con $1 \le i \le 3$ tal que los elementos de $A_i$ satisfacen la propiedad $p_i$. Bajo estas condiciones lo pedido en el enunciado se resuelve calculando el cardinal de $\overline{A_1} \cap \overline{A_2} \cap \overline{A_3}$, para ello usaremos el principio I-E para tres propiedades

$$  
\begin{aligned}
|\overline{A_1} \cap \overline{A_2} \cap \overline{A_3}| =
|S| - |A_1| - |A_2| - |A_3| +
|A_1 \cap A_2| + |A_1 \cap A_3| + |A_2 \cap A_3| -\\
|A_1 \cap A_2 \cap A_3|
\end{aligned}
$$

Ahora calculemos los cardinales:

- $|S|$ = La cantidad de soluciones, por teorema 2 sabemos que es $C(27, 3)$
- $|A_1|$ = La cantidad de soluciones con $a \gt 2$, reescribimos la restricción:
$$ a \ge 3 $$
Definimos la siguiente variable:
$$
a^{'} = a - 3
$$

Reescribimos la ecuación:

$$  
\begin{aligned}
(a^{'} + 3) + b + c + d &= 24\\
a^{'} + b + c + d &= 24 - 3\\
a^{'} + b + c + d &= 21\\
\end{aligned}
$$Luego la cantidad de soluciones para esa ecuación en $\mathbb{Z} \ge 0$ es $C(24, 3)$ 

- $|A_2|$= La cantidad de soluciones con $b \gt 5$, reescribimos la restricción:
$$ b \ge 6 $$
Definimos la siguiente variable:
$$

b^{'} = b - 6

$$

Reescribimos la ecuación:

$$  

\begin{aligned}

a + (b^{'} + 6) + c + d &= 24\\

a + b^{'} + c + d &= 24 - 6\\

a + b^{'} + c + d &= 18\\

\end{aligned}

$$Luego la cantidad de soluciones para esa ecuación en $\mathbb{Z} \ge 0$ es $C(21, 3)$

- $|A_3|$ = La cantidad de soluciones con $c \gt 6$, reescribimos la restricción:
$$ c \ge 7 $$
Definimos la siguiente variable:
$$

c^{'} = c - 7

$$

Reescribimos la ecuación:

$$  

\begin{aligned}

a + b + (c^{'} + 7) + d &= 24\\

a + b + c^{'} + d &= 24 - 7\\

a + b + c^{'} + d &= 17\\

\end{aligned}

$$Luego la cantidad de soluciones para esa ecuación en $\mathbb{Z} \ge 0$ es $C(20, 3)$

- $|A_1 \cap A_2|$ = La cantidad de soluciones con $a \gt 2$ y $b \gt 5$, reescribimos las restricciones de la siguiente manera:

$$  

\begin{aligned}

a \ge 3\\

b \ge 6\\

\end{aligned}

$$
declaramos las siguientes variables:
$$  

\begin{aligned}

a^{'} = a - 3\\

b^{'} = b - 6\\

\end{aligned}

$$
reescribimos la ecuación:
$$  

\begin{aligned}

(a^{'} + 3) + (b^{'} + 6) + c + d &= 24\\

a^{'} + b^{'} + c + d &= 24 - 3 - 6\\

a^{'} + b^{'} + c + d &= 15\\

\end{aligned}

$$
Luego la cantidad de soluciones para esa ecuación en $\mathbb{Z} \ge 0$, por teorema 2 es $C(18, 3)$

- $|A_1 \cap A_3|$ = La cantidad de soluciones de:
$$

\begin{aligned}

(a^{'} + 3) + b + (c^{'} + 7) + d &= 24\\

a^{'} + b + c^{'} + d &= 24 - 3 - 7\\

a^{'} + b + c^{'} + d &= 14\\

\end{aligned}

$$
Luego la cantidad de soluciones a esa ecuación es $C(17,3)$

- $|A_2 \cap A_3|$= La cantidad de soluciones de:
  
$$

\begin{aligned}

a + (b^{'} + 6) + (c^{'} + 7) + d &= 24\\

a + b^{'} + c^{'} + d &= 24 - 6 - 7\\

a + b^{'} + c^{'} + d &= 11\\

\end{aligned}

$$
Luego la cantidad de soluciones es $C(14,3)$

- $|A_1 \cap A_2 \cap A_3|$ = La cantidad de soluciones de la ecuación

$$

\begin{aligned}

(a^{'} + 3 ) + (b^{'} + 6) + (c^{'} + 7) + d &= 24\\

a^{'} + b^{'} + c^{'} + d &= 24 - 3 - 6 - 7\\

a^{'} + b^{'} + c^{'} + d &= 8\\

\end{aligned}

$$
Luego la cantidad de soluciones a esa ecuación es $C(11, 3)$

Ahora reemplazamos los cardinales en la expresión del principio I-E

$$

C(27,3) - C(24,3) - C(21,3) - C(20,3) + C(18,3) + C(17,3) + C(14,3) - C(11,3)

$$
Esto equivale a la cantidad de soluciones de la ecuación del enunciado con sus respectivas restricciones
