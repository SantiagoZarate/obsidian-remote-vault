---
tags:
  - Inclusión-Exclusión
status: Done
correcto: true
---

## Calcule El Número De Permutaciones De 1, 2, 3, 4, 5, 6, 7 Tales Que El 1 no Está En El Primer Lugar, El 4 no Está En El Cuarto Lugar Y El 7 no Está En El Séptimo Lugar

**Respuesta**

Sea $S$ el conjunto de números de 7 dígitos teniendo en cuenta los dígitos del enunciado, definimos las siguientes propiedades

$$  
\begin{aligned}
P_1 &= \text{El 1 esta en el primer lugar}\\
P_2 &= \text{El 4 esta en el cuarto lugar}\\
P_3 &= \text{El 7 esta en el septimo lugar}\\
\end{aligned}
$$

y los subconjuntos $A_i$ de $S$ con $1 \le i \le 2$ tal que los elementos de $A_i$ cumplen la propiedad $P_i$. Bajo estas restricciones lo pedido en el enunciado se resuelve calculando el cardinal de $\overline{A_1} \cup \overline{A_2} \cup \overline{A_3}$ y para ello usaremos el principio inclusión-exclusión para 3 propiedades.

$$  
\begin{aligned}
|\overline{A_1} \cap \overline{A_2} \cap \overline{A_3}| =
|S| - |A_1| - |A_2| - |A_3| +
|A_1 \cap A_2| + |A_1 \cap A_3| + |A_2 \cap A_3| -\\
|A_1 \cap A_2 \cap A_3|
\end{aligned}
$$ 

Ahora calculamos los cardinales.

- $|S|$ = La cantidad de permutaciones de un número de 7 dígitos es igual a $7!$
- $|A_1|$ = La cantidad de elementos de $S$ que tengan al 1 en el primer lugar, para ello fijamos el número 1 a la primera posición y permutamos los 6 restantes, lo que es igual a $6!$
- $|A_2|\, y \,|A_3|$ = De manera análoga al calculo de $|A_1|$ , es 6!
- $|A_1 \cap A_2|$ = La cantidad de elementos de $S$ donde el número 1 ocupa la primer posición y el 4 ocupa la cuarta posición, fijamos esos números a sus posiciones y permutamos los 5 restantes dígitos, lo que equivale a $5!$ ordenamientos
- $|A_1 \cap A_3|$ y $|A_2 \cap A_3|$ = De manera análoga al calculo de $|A_1 \cap A_2|$ esto es $5!$
- $|A_1 \cap A_2 \cap A_3|$ = La cantidad de elementos de $S$ donde la primer posición esta ocupada por el 1, la cuarta por el 4 y la séptima por el 7, donde nos quedan por contar las permutaciones de los 4 restantes dígitos, lo que equivale a $4!$

Como las propiedades son simétricas, al reemplazar los cardinales en la expresión del principio inclusión-exclusión nos queda:

$$
7! - \begin{pmatrix} 3 \\ 1 \end{pmatrix} 6! + 
\begin{pmatrix} 3 \\ 2 \end{pmatrix} 5! -
\begin{pmatrix} 3 \\ 3 \end{pmatrix} 4!

$$

Esto equivale a la cantidad de permutaciones de los dígitos del enunciado teniendo en cuenta sus restricciones.
