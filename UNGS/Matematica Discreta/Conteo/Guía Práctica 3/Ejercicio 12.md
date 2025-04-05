---
tags:
  - Ecuación-Linear
  - Inclusión-Exclusión
status: Done
---

## Calcule El Número De Soluciones En Los Enteros Positivos De la Ecuación

$$x_1 + x_2 + x_3 + x_4 = 25$$

tales que

$$  
1 ≤ xi ≤ 8  \,\text{para}\, 1 ≤ i ≤ 4.
$$ 
**Respuesta**

Sea $S$ el conjunto cuyos elementos son las soluciones a la ecuación del enunciado en $\mathbb{N}$, definimos las siguientes propiedades

$$
p_i : x_i \gt 8
$$

y definimos los subconjuntos $A_i$ de $S$ donde $1 \le i \le 4$ tal que los elementos de $A_i$ satisfacen la propiedad $p_i$. Bajo estos términos la solución al problema del enunciado se resuelve obteniendo el cardinal de $\overline{A_1} \cap \overline{A_2} \cap \overline{A_3} \cap \overline{A_4}$, para ello usaremos el principio inclusión-exclusión para 4 propiedades.

Notar que las propiedades tienen la misma restricción pero en distinta variable, por lo que podemos deducir que son propiedades simétricas, por lo que podemos sintetizar la expresión del principio I-E:

$$
\begin{aligned}
|\overline{A_1} \cap \overline{A_2} \cap \overline{A_3} \cap \overline{A_4} \cap| =\\
|S|
- \begin{pmatrix} 4 \\ 1 \end{pmatrix} |A_1|
+ \begin{pmatrix} 4 \\ 2 \end{pmatrix} |A_1 \cap A_2| 
- \begin{pmatrix} 4 \\ 3 \end{pmatrix} |A_1 \cap A_2 \cap A_3| 
+ \begin{pmatrix} 4 \\ 4 \end{pmatrix} |A_1 \cap A_2 \cap A_3 \cap A_4| 
\end{aligned}
$$

Ahora calculemos los cardinales:

- $|S|$ = La cantidad de soluciones, por teorema 1 es igual a $C(24, 3)$
- $|A_1|$ = La cantidad de soluciones con $x_1 \gt 8$, podemos reescribir la restricción como
$$ x_1 \ge 9 $$
definimos la siguiente variable:
$$ x_1^{'} = x_1 - 8  $$
Reescribimos la ecuación:
$$  
\begin{aligned}
(x_1^{'} + 8) + x_2 + x_3 + x_4 &= 25\\
x_1^{'}  + x_2 + x_3 + x_4 &= 25 - 8\\
x_1^{'}  + x_2 + x_3 + x_4 &= 17\\
\end{aligned}
$$

La cantidad de soluciones para esa ecuación en $\mathbb{N}$ por teorema 1 es $C(16, 3)$, esto equivale al cardinal de $A_1$

- $|A_1 \cap A_2|$ = La cantidad de soluciones con $x_1 \gt 8$ y $x_2 \gt 8$, podemos reescribir las restricciones de la siguiente manera:

$$  
\begin{aligned}
x_1 \ge 9\\
x_2 \ge 9\\
\end{aligned}
$$ Declaramos las siguientes variables:
$$  

\begin{aligned}

x_1^{'} &= x_1 - 8\\

x_2^{'} &= x_2 - 8\\

\end{aligned}

$$
Reescribimos la ecuación:
$$  

\begin{aligned}

(x_1^{'} + 8) + (x_2^{'} + 8) + x_3 + x_4 &= 25\\

x_1^{'} + x_2^{'} + x_3 + x_4 &= 25 - 8 - 8\\

x_1^{'} + x_2^{'} + x_3 + x_4 &= 9\\

\end{aligned}

$$ La cantidad de soluciones para esa ecuación en $\mathbb{N}$ por teorema 1 es igual a $C(8, 4)$

- $|A_1 \cap A_2 \cap A_3|$ = La cantidad de soluciones con $x_1, x_2$ y $x_3 \gt 8$, podemos reescribir la restricción de la siguiente manera:
$$  
\begin{aligned}
x_1 \ge 9\\
x_2 \ge 9\\
x_3 \ge 9\\
\end{aligned}
$$

Declaramos las siguientes variables:

$$  
\begin{aligned}
x_1^{'} &= x_1 - 8\\
x_2^{'} &= x_2 - 8\\
x_3^{'} &= x_3 - 8\\
\end{aligned}
$$ Reescribimos la ecuación:

$$  

\begin{aligned}

(x_1^{'} + 8) + (x_2^{'} + 8) + (x_3^{'} + 8) + x_4 &= 25\\

x_1^{'} + x_2^{'} + x_3^{'} + x_4 &= 25 - 8 - 8 - 8\\

x_1^{'} + x_2^{'} + x_3^{'} + x_4 &= 1\\

\end{aligned}

$$
Notar que no hay solución para esta ecuación en $N$, por lo tanto $A_1 \cap A_2 \cap A_3 = \emptyset$, lo mismo ocurre cuando vamos a calcular el cardinal de $A_1 \cap A_2 \cap A_3 \cap A_4$.

Ahora reemplazamos los cardinales:

$$

C(24,3) -

\begin{pmatrix} 4 \\ 1 \end{pmatrix} C(16,3) +

\begin{pmatrix} 4 \\ 2 \end{pmatrix} C(8,4)

$$
Esto equivale a la cantidad de soluciones para la ecuación del enunciado con sus respectivas restricciones.
