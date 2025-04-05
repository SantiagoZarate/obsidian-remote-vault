---
tags:
  - Inclusión-Exclusión
status: Done
correcto: true
---

## ¿Cuántos De Los Números Del 1 Al 33000, Ambos Inclusive, no Son Divisibles Ni Por 3, Ni Por 5, Ni Por 11?

**Respuesta**

Sea S el conjunto de los números del 1 hasta el 33000 ambos inclusive, definimos las siguientes propiedades.

$$  
\begin{aligned}
P_1 &= \text{Divisible por 3}\\
P_2 &= \text{Divisible por 5}\\
P_3 &= \text{Divisible por 11}\\
\end{aligned}
$$

Definimos los subconjuntos de $S$, sean $A_i$ con $1 \le i \le 2$ , donde $A_i$ satisface $P_i$

Resolver lo pedido en el enunciado se resuelve usando el principio inclusión-exclusión con tres propiedades

$$  
\begin{aligned}
|\overline{A_1} \cup \overline{A_2} \cup \overline{A_3}| =\\
|S| - |A_1| - |A_2| - |A_3|\\
 + |A_1 \cap A_2| + |A_1 \cap A_3| + |A_2 \cap A_3|\\
 - |A_1 \cap A_2 \cap A_3| 
\end{aligned}
$$

Calculamos los cardinales de los conjuntos.

- $|S|$ = 33000
- $|A_1|$ = $?$
Necesitamos calcular la cantidad de elementos de S que sean divisibles por 3, así que planteamos la siguiente cuenta:

$$
\frac{33000}{3} = 11000
$$

Entonces $|A_1|$ es 11000

- $|A_2|$ = $\frac{33000}{5}$ = 6600
- $|A_3|$ = $\frac{33000}{11}$ = 3000
- $|A_1 \cap A_2|$ = $?$
Necesitamos encontrar el cardinal de la intersección entre esos dos conjuntos, para ello tenemos que encontrar el mínimo común múltiplo de 3 y 5, que es 15.
$$
\frac{33000}{15} = 2200
$$

Entonces $|A_1 \cup A_2| = 2200$

- $|A_1 \cap A_3|$ = $?$
El mínimo común múltiplo de 3 y 11 es 33.
$$
\frac{33000}{33} = 1000
$$

Entonces $|A_1 \cap A_3| = 1000$

- $|A_2 \cup A_3|$ = $?$
El MCM de 5 y 11 es 55.
$$
\frac{33000}{55} = 600
$$

Entonces $|A_2 \cup A_3| = 600$

- $|A_1 \cup A_2 \cup A_3|$ = $?$
El MCM de 3, 5 y 11 es 165
$$
\frac{33000}{165} = 200
$$

Entonces $|A_1 \cup A_2 \cup A_3| = 200$

Ahora reemplazamos los cardinales en la expresión del principio inclusión-exclusión.

$$|\overline{A_1} \cap \overline{A_2} \cap \overline{A_3}| = 33000 - 11000 - 6600 - 3000 + 2200 + 1000 + 600 - 200$$

Eso equivale a la cantidad números del conjunto $S$ que no son divisibles por los números del enunciado.
