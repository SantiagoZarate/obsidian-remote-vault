---
tags:
  - Inclusión-Exclusión
status: Done
---

## Calcule El Número De Permutaciones De Los Números Del 1 Al 9 Tal Que Ninguno De Los Números Ocupa Su Posición Natural

**Respuesta**

Número de 9 dígitos

ej

$$
123456789
$$

pero que no tengan su posición natural

$$
912345678
$$

Definimos el conjunto $S$ cuyos elementos son las permutaciones de los números del 1 al 9, definimos las siguientes propiedades:

$$
p_i = \text{el dígito i ocupa su posición natural}
$$

y los subconjuntos $A_i$ de $S$ con $1 \le i \le 9$ tal que los elementos de $A_i$ satisfacen la propiedad $p_i$. Bajo estas condiciones lo pedido en el enunciado se resuelve obteniendo el cardinal de $\overline{A_1} \cap \overline{A_2} \cap ... \cap \overline{A_9}$ para ello usaremos el principio I-E para 9 propiedades.

Podemos anticipar que las propiedades son simétricas, por lo que podemos representar la expresión de la siguiente manera:

$$  
\begin{aligned}
|A_1 \cap A_2 \cap ... A_9| &=\\ |S|
- \begin{pmatrix} 9 \\ 1 \end{pmatrix} |A_1| 
+ \begin{pmatrix} 9 \\ 2 \end{pmatrix} |A_1 \cap A_2| 
- \begin{pmatrix} 9 \\ 3 \end{pmatrix} |A_1 \cap A_2 \cap A_3| 
+ \begin{pmatrix} 9 \\ 4 \end{pmatrix} |A_1 \cap A_2 \cap A_3 \cap A_4|\\
- \begin{pmatrix} 9 \\ 5 \end{pmatrix} |A_1 \cap A_2 \cap A_3 \cap A_4 \cap A_5|
+ \begin{pmatrix} 9 \\ 6 \end{pmatrix} |A_1 \cap A_2 \cap A_3 \cap A_4 \cap A_5 \cap A_6|\\
-\begin{pmatrix} 9 \\ 7 \end{pmatrix} |A_1 \cap A_2 \cap A_3 \cap A_4 \cap A_5 \cap A_6 \cap A_7|\\
+ \begin{pmatrix} 9 \\ 8 \end{pmatrix} |A_1 \cap A_2 \cap A_3 \cap A_4 \cap A_5 \cap A_6 \cap A_7 \cap A_8|\\
- \begin{pmatrix} 9 \\ 9 \end{pmatrix} |A_1 \cap A_2 \cap A_3 \cap A_4 \cap A_5 \cap A_6 \cap A_7 \cap A_8 \cap A_9|

\end{aligned}
$$ 

Ahora calculemos los cardinales:

- $|S|$ = $9!$
- $|A_1|$ = La cantidad de permutaciones donde el 1 ocupa su posición natural: $8!$
- $|A_1 \cap A_2|$ = La cantidad de permutaciones donde el 1 y el 2 ocupan su posición natural: $7!$
- $|A_1 \cap A_2 \cap A_3|$ = $6!$
- $|A_1 \cap A_2 \cap A_3 \cap A_4|$ = $5!$
- $|A_1 \cap A_2 \cap A_3 \cap A_4 \cap A_5|$ = $4!$
- $|A_1 \cap A_2 \cap A_3 \cap A_4 \cap A_5 \cap A_6|$ = $3!$
- $|A_1 \cap A_2 \cap A_3 \cap A_4 \cap A_5 \cap A_6 \cap A_7|$ = $2!$
- $|A_1 \cap A_2 \cap A_3 \cap A_4 \cap A_5 \cap A_6 \cap A_7 \cap A_8|$ = $1!$
- $|A_1 \cap A_2 \cap A_3 \cap A_4 \cap A_5 \cap A_6 \cap A_7 \cap A_8 \cap A_9|$ = $0!$

Ahora reemplazamos los cardinales

$$
9!
-\begin{pmatrix} 9 \\ 1 \end{pmatrix} 8!
+\begin{pmatrix} 9 \\ 2 \end{pmatrix} 7!
-\begin{pmatrix} 9 \\ 3 \end{pmatrix} 6!
+\begin{pmatrix} 9 \\ 4 \end{pmatrix} 5!
-\begin{pmatrix} 9 \\ 5 \end{pmatrix} 4!
+\begin{pmatrix} 9 \\ 6 \end{pmatrix} 3!
-\begin{pmatrix} 9 \\ 7 \end{pmatrix} 2!
+\begin{pmatrix} 9 \\ 8 \end{pmatrix} 1!
-\begin{pmatrix} 9 \\ 9 \end{pmatrix} 0!
$$

Esto equivale a la cantidad de permutaciones de los número del enunciado con su respectiva restricción.
