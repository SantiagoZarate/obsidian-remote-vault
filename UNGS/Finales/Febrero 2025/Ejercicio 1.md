---
tags:
  - Inclusión-Exclusión
---

En la Isla Zevil se encuentran 24 aspirantes a cazadores, numerados del 1 al 24. Se reparten entre ellos 24 tarjetas numeradas del 1 al 24, una tarjeta a cada uno.

(a) ¿De cuántas formas se pueden distribuir las 24 tarjetas entre los 24 aspirantes con la condición de que el aspirante 1 no reciba la tarjeta 1, el 2 no reciba la 2 y el 3 no reciba la 3?

(b) ¿De cuántas formas se pueden distribuir las 24 tarjetas entre los 24 aspirantes con la condición de que no se formen 12 parejas?

Nota: Dos aspirantes A y B forman una pareja si A recibe el número de B y B el de A.

**Respuestas**

## A -

El aspirante 1 tiene 23 posibles tarjetas asignadas a el, cualquiera de las 24 a excepción de la número 1.

El aspirante 2 tiene 22 posibles tarjetas asignadas a el, cualquiera de las 24 a excepción de la que fue asignada al aspirante 1, y la que tiene el número 2.

Este razonamiento pareciera tener sentido, pero que pasa si al aspirante 1 se le asigna la tarjeta numerada con el 2? en ese caso, el aspirante 2 tendría 23 posibles tarjetas que pueden ser asignadas a el, es decir, la cantidad de tarjetas asignadas al segundo aspirante no es independiente de la tarjeta que le toque al primer aspirante.

Es por eso que tengo que usar el principio de inclusion exclusión, en concreto con 3 propiedades.

---

Sea $S$ el conjunto de formas de asignar cada una de las 24 tarjetas a cada uno de los aspirantes, definimos las siguientes propiedades:

$$  
\begin{aligned}
P_1 = \text{El aspirante 1 recibe la tarjeta 1}\\
P_2 = \text{El aspirante 2 recibe la tarjeta 2}\\
P_3 = \text{El aspirante 3 recibe la tarjeta 3}\\
\end{aligned}
$$ 

y los subconjuntos $A_i$ con $1 \le i \le 3$, tal que los elementos de $A_i$ satisfacen $P_i$. Bajo estas definiciones el problema se resuelve calculando el cardinal de $\overline{A_1} \cap \overline{A_2} \cap \overline{A_3}$ y para ello usaremos el principio I-E para 3 propiedades.

$$
|\overline{A_1} \cap \overline{A_2} \cap \overline{A_3}| = |S| -
|A_1| - |A_2| - |A_3|
+ |A_1 \cap A_2| + |A_1 \cap A_3| + |A_2 \cap A_3|
- |A_1 \cap A_2 \cap A_3|
$$

Ahora necesitamos calcular los cardinales.

- $|S|$ = $24!$, todas las posibles formas de asignar cada una de las tarjetas a cada aspirante
- $|A_1|, |A_2|, |A_3|$ = $23!$, pues el aspirante $i$, con $1\le i \le 3$, se le asigna la tarjeta con el número $i$ y al resto de aspirantes se le puede asignar cualquier otra tarjeta
- $|A_1 \cap A_2|$ = $22!$, pues al aspirante 1 y 2 se le asignan las tarjetas 1 y 2 respectivamente, y al resto de aspirantes se le pueden asignar cualquiera de las 22 restantes.
- $|A_1 \cap A_3|, |A_2 \cap A_3|$ = $22!$, pues se cumple el mismo escenario que en el calculo del cardinal del conjunto anterior, solo que con otros números de aspirantes y numeraciones de tarjetas.
- $|A_1 \cap A_2 \cap A_3|$ = $21!$, pues a los aspirantes 1, 2 y 3 se le asignan las tarjetas numeradas 1, 2 y 3 respectivamente, y al resto de aspirantes se le pueden asignar cualquiera de las restantes 21 tarjetas.

Vemos que tenemos propiedades son isométricas por lo que podemos resumir la fórmula para calcular el cardinal de $\overline{A_1} \cap \overline{A_2} \cap \overline{A_3}$

$$
|\overline{A_1} \cap \overline{A_2} \cap \overline{A_3}| = 24!
- \begin{pmatrix} 3 \\ 1 \end{pmatrix} 23!
+ \begin{pmatrix} 3 \\ 2 \end{pmatrix} 22!
- \begin{pmatrix} 3 \\ 3 \end{pmatrix} 21!
$$

Esto equivale a la cantidad de combinaciones posibles de asignar las tarjetas de modo tal que se cumplan las condiciones propuestas en el enunciado.

---
## B -

Se me ocurre primero calcular el total de formas de asignar las tarjetas a cada uno de los aspirantes pero sin restricciones (24!) y luego restarle las formas en las que se formarían 12 parejas, haciendo uso del principio de sustracción.

Para calcular las formas en las que se pueden formar 12 parejas aun tengo algunas dudas, se me ocurrió primero contar las formas de tomar dos aspirantes entre 24 disponibles, lo que equivale a $\begin{pmatrix} 24 \\ 2 \end{pmatrix}$, luego las formas de tomar 2 entre 22 disponibles (descarto los primeros 2 elegidos), lo que equivale a $\begin{pmatrix} 20 \\ 2 \end{pmatrix}$, y así sucesivamente
