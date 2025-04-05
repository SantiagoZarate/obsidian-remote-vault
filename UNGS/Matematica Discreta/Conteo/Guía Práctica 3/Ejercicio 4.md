---
tags:
  - Inclusión-Exclusión
status: Done
correcto: true
---

## ¿Cuántas Permutaciones Hay De Las Letras De la Palabra PROPONER Donde Letras Iguales no Aparecen En Posiciones Consecutivas?

**Respuesta**

Observemos que la palabra dada esta compuesta por 8 letras, donde para las letras P, R y O contamos con 2 repeticiones de cada una, definamos $S$ el conjunto cuyos elementos son las distintas formas de ordenar las letras de la palabra del enunciado, definimos los siguientes conjuntos:

$$  
\begin{aligned}
p_1 &= \text{Las letras P estan consecutivas}\\
p_2 &= \text{Las letras R estan consecutivas}\\
p_3 &= \text{Las letras O estan consecutivas}\\
\end{aligned}
$$

y los subconjuntos $a_i$ de $S$ con $1 \le i \le 2$ tal que los elementos de $a_i$ cumplen la propiedad $p_i$. Bajo estas condiciones resolver lo pedido en el enunciado se resuelve calculando el cardinal de $\overline{a_1} \cap \overline{a_2} \cap \overline{a_3}$ para ello usamos el principio inclusión-exclusión para 3 propiedades.

$$  
\begin{aligned}
|\overline{A_1} \cap \overline{A_2} \cap \overline{A_3}| =
|S| - |A_1| - |A_2| - |A_3| +
|A_1 \cap A_2| + |A_1 \cap A_3| + |A_2 \cap A_3| -\\
|A_1 \cap A_2 \cap A_3|
\end{aligned}
$$

Ahora necesitamos calcular los cardinales.

- $|S|$ = La cantidad de ordenamientos del siguiente multiconjunto:
  $$\{ 2 \cdot P, 2 \cdot R, 2 \cdot O, 1 \cdot N, 1 \cdot E \} $$ eso es igual a
$$\frac{8!}{2!\cdot2!\cdot2!} = 5040$$
Entonces el cardinal de $S$ es 5040

- $|a_1|$ = La cantidad de ordenamientos de $S$ donde las letras P están consecutivas, por lo que definimos la variable $X$, que compone a las 2 letras P, y nos queda el siguiente multiconjunto:
$$\{ 2 \cdot R, 2 \cdot O, 1 \cdot N, 1 \cdot E, 1 \cdot X \}  $$
Contar las permutaciones de ese multiconjunto de 7 elementos, con 2 tipos de elementos con 2 repeticiones es igual a:
$$
\frac{7!}{2!\cdot2!} = 1260
$$

Entonces el cardinal de $a_1$ es 1260

- $|a_2|$ y $|a_3|$ = De manera análoga al calculo para obtener $|a_1|$, es 1260
- $|a_1 \cap a_2|$ = La cantidad de elementos de $S$ donde las letras P estén consecutivas y las letras R estén consecutivas, definimos las variables donde tomamos a las dos letras que tienen repetición, $X$ e $Y$ respectivamente y definimos el siguiente multiconjunto:
  $$\{ 2 \cdot O, 1 \cdot N, 1 \cdot E, 1 \cdot X , 1 \cdot Y\}  $$
Contar las permutaciones de ese multiconjunto con 6 elementos, con un tipo de elemento con 2 repeticiones es igual a:
$$
\frac{6!}{2!} = 360
$$

Entonces el cardinal de $a_1 \cap a_2$ es 360

- $|a_1 \cap a_3|$ y $|a_2 \cap a_3|$ = De manera análoga al calculo para obtener $|a_1|$, es 360
- $|a_1 \cap a_2 \cap a_3|$ = La cantidad de elementos de $S$ donde las letras P están consecutivas, las letras R están consecutivas y las letras O están consecutivas, por lo que por cada letra repetida definimos variables que las agrupen, $X, Y$ y $Z$ respectivamente, luego definimos el siguiente multiconjunto:
$$\{ 1 \cdot N, 1 \cdot E, 1 \cdot X , 1 \cdot Y, 1 \cdot Z\}  $$
Calcular los ordenamientos de 5 elementos sin repeticiones es igual a $5!$, entonces el cardinal de $a_1 \cap a_2 \cap a_3$ es 120

Como las propiedades son simétricas, al sustituir los cardinales en la expresión del principio inclusión-exclusión nos queda de la siguiente manera:

$$
5040 - \begin{pmatrix} 3 \\ 1 \end{pmatrix} 1260 +
\begin{pmatrix} 3 \\ 2 \end{pmatrix} 360 - 
\begin{pmatrix} 3 \\ 3 \end{pmatrix} 120
$$

Esto equivale a la cantidad de permutaciones de la palabra dada con las restricciones del enunciado.
