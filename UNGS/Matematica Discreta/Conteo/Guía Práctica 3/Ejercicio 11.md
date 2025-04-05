---
tags:
  - Inclusión-Exclusión
  - Ecuación-Linear
status: Done
---

## Encuentre El Número De Soluciones En Los Enteros Positivos De la Ecuación

$$x_1 + x_2 + x_3 + x_4 = 20$$

que satisfagan las siguientes condiciones

$$  
\begin{aligned}
1 ≤ &x1 ≤ 6\\
1 ≤ &x2 ≤ 7\\
3 ≤ &x3 ≤ 9\\
4 ≤ &x4 ≤ 11.
\end{aligned}
$$ 
**Respuesta**

Primero realizamos una corrección a las variables para que todas tengan como cota inferior el 1, en concreto a $x_3$ y $x_4$.

$$  
\begin{aligned}
1 \le x_3 - 2 \le 7\\
1 \le x_4 - 3 \le 8\\
\end{aligned}
$$

Reasignamos las variables:

$$  
\begin{aligned}
a &= x_1\\
b &= x_2\\
c &= x_3 - 2\\
d &= x_4 - 3\\
\end{aligned}
$$

Reescribimos la ecuación:

$$  
\begin{aligned}
a + b + c + d &= x_1 + x_2 + x_3 - 2 + x_4 - 3\\
a + b + c + d &= (x_1 + x_2 + x_3 + x_4) - (2 - 3)\\
a + b + c + d &= 20 - 5\\
a + b + c + d &= 15\\
\end{aligned}
$$

Entonces el problema se resume en encontrar la cantidad de soluciones para esa ecuación en $\mathbb{N}$ con las siguientes restricciones:

$$  
\begin{aligned}
c \le 7\\
d \le 8\\
\end{aligned}
$$

Definimos el conjunto $S$ cuyos elementos son las soluciones en $\mathbb{N}$ de la siguiente ecuación

$$
a + b + c + d = 15
$$

Sean las propiedades:

$$  
\begin{aligned}
p_1 &= c \gt 7\\
p_2 &= d \gt 8\\
\end{aligned}
$$

Definimos los subconjuntos $A_1$ de $S$ tal que sus elementos satisfacen la propiedad $p_1$ y $A_2$ de $S$ tal que sus elementos satisfacen $p_2$. Bajo estos términos el problema del enunciado se resuelve calculando el cardinal de $\overline{A_1} \cap \overline{A_2}$, para ello vamos a usar el principio inclusión-exclusión para 2 propiedades.

$$  
\begin{aligned}
|\overline{A_1} \cap \overline{A_2}| = |S| - |A_1| - |A_2| + |A_1 \cap A_2|
\end{aligned}
$$ 

Ahora calculemos los cardinales:

- $|S|$ = La cantidad de soluciones para la ecuación en $\mathbb{N}$, por teorema 1 es igual a $C(14, 3)$
- $|A_1|$ = La cantidad de soluciones para la ecuación en $N$ donde $c \gt 7$, podemos reescribir la restricción de la siguiente manera:
  $$ c \ge 8 $$
  definamos la siguiente variable:
  $$ c^{'} = a - 7 $$
  y reescribimos la ecuación:
  $$  

\begin{aligned}

a + b + (c^{'} + 7) + d &= 15\\

a + b + c^{'} + d &= 15 - 7\\

a + b + c^{'} + d &= 8\\

\end{aligned}

$$
Entonces la cantidad de soluciones para esa ecuación en $\mathbb{N}$, por teorema 1 es $C(7, 3)$

- $|A_2|$ = La cantidad de soluciones con $d \gt 8$, reescribamos la restricción como:
  $$ d \ge 9 $$
  Definamos la siguiente variable:
  $$ d^{'} = d - 8 $$
  Reescribamos la ecuación:
  
  
$$

\begin{aligned}

a + b + c + (d^{'} + 8) &= 15\\

a + b + c + d^{'} &= 15 - 8\\

a + b + c + d^{'} &= 7\\

\end{aligned}

$$
Luego la cantidad de soluciones para esa ecuación en $N$, por teorema 1 es $C(6, 3)$
- $|A_1 \cap A_2|$ =  La cantidad de soluciones con $c \gt 7$ y $d \gt 8$, reescribamos las restricciones de la siguiente manera:
  
  $$ 

\begin{aligned}

c \ge 8 \\

d \ge 9 \\

\end{aligned}

$$
definamos las siguientes variables:
$$  

\begin{aligned}

c^{'} &= c - 7\\

d^{'} &= d - 8\\

\end{aligned}

$$
Reescribamos la ecuación:

$$  

\begin{aligned}

a + b + (c^{'} + 7 ) + (d^{'} + 8) &= 15\\

a + b + c^{'} + d^{'} &= 15 - 7 - 8\\

a + b + c^{'} + d^{'} &= 0\\

\end{aligned}

$$
Notemos que no hay soluciones para esa ecuación en $N$, por lo que $A_1 \cap A_2 = \emptyset$

Reemplazamos los cardinales en la expresión del principio inclusión-exclusión
$$

C(14,3) - C(7,3) - C(6,3)

$$
Esto equivale a la cantidad de soluciones de la ecuación del enunciado con sus respectivas restricciones.
