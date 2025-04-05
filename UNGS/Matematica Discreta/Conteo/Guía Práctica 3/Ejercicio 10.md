---
tags:
  - Inclusión-Exclusión
  - Ecuación-Linear
status: Done
---

## Encuentre la Cantidad De Soluciones De la Ecuación

$$x_1 + x_2 + x_3 + x_4 + x_5 + x_6 = 34$$

En los números enteros positivos menores o iguales a 10.

**Respuesta**

Sea $S$ el conjunto de soluciones para la ecuación del enunciado, definimos las siguientes propiedades

$$  
\begin{aligned}
p_1 = x_1 \gt 10\\
p_2 = x_2 \gt 10\\
p_3 = x_3 \gt 10\\
p_4 = x_4 \gt 10\\
p_5 = x_5 \gt 10\\
p_6 = x_6 \gt 10\\
\end{aligned}
$$

y los subconjuntos $A_i$ de $S$ con $i \le i \le 6$ tal que los elementos de $A_i$ satisfacen la propiedad $p_i$, Bajo estos términos resolver lo pedido en el enunciado se obtiene calculando el cardinal de $\underline{A_1} \cap \underline{A_2}... \cap \underline{A_6}$ para ello usaremos el principio inclusion-exclusion para 6 propiedades.

Debido a que el desglose de la expresión es muy extensa representamos a los subconjuntos con letras, donde las letras son mayores o iguales a 1 y menores o iguales a 6.

$$  
\begin{aligned}
|\overline{A_1} \cap \overline{A_2} \cap \overline{A_3} \cap \overline{A_4} \cap \overline{A_5} \cap \overline{A_6}| = \\
|S|
-\begin{pmatrix} 6 \\ 1 \end{pmatrix} |A_i|
+\begin{pmatrix} 6 \\ 2 \end{pmatrix} |A_i \cap A_j|
-\begin{pmatrix} 6 \\ 3 \end{pmatrix} |A_i \cap A_j \cap A_k|\\
+\begin{pmatrix} 6 \\ 4 \end{pmatrix} |A_i \cap A_j \cap A_k \cap A_m|
-\begin{pmatrix} 6 \\ 5 \end{pmatrix} |A_i \cap A_j \cap A_k \cap A_m \cap A_n|\\
+ \begin{pmatrix} 6 \\ 6 \end{pmatrix} |A_i \cap A_j \cap A_k \cap A_m \cap A_n \cap A_o|
\end{aligned}
$$

Al calcular los cardinales, como las propiedades tienen la misma restricción pero en distinta variable, representamos los subconjuntos con letras:

- $|S|$ = La cantidad de soluciones de la ecuación en $\mathbb{N}$ por teorema eso es igual a $C(33, 5)$
- $|A_i|$ = La cantidad de soluciones donde $x_i \gt 10$, reescribimos la restricción de la siguiente manera:

  $$ x_i \ge 11 $$

  Definimos la siguiente variable

  $$x_i^{'} = x_i - 11 $$

  Reescribimos la ecuación con la nueva variable:

  $$  

\begin{aligned}

(x_i^{'} + 11) + x_2 + x_3 + x_4 + x_5 + x_6 &= 34\\

x_i^{'} + x_2 + x_3 + x_4 + x_5 + x_6 &= 34 - 11\\

x_i^{'} + x_2 + x_3 + x_4 + x_5 + x_6 &= 23 \\

\end{aligned}

$$
La cantidad de soluciones para esa ecuación en $\mathbb{N}$ es $C(22, 5)$, esto equivale al cardinal de $|x_i|$

- $|A_i \cap A_j|$ = La cantidad de soluciones de la ecuación donde $x_i \gt 10$  y $x_j \gt 10$, reescribimos las restricciones de la siguiente manera:
  $$ x_i \ge 11; x_j \ge 11 $$
  definimos las siguientes variables:
  $$  

\begin{aligned}

x_i^{'} &= x_i - 11\\

x_j^{'} &= x_j - 11\\

\end{aligned}

$$
Reescribimos la ecuación:
$$  

\begin{aligned}

(x_i^{'} + 11) + (x_j^{'} + 11) + x_3 + x_4 + x_5 + x_6 &= 34\\

x_i^{'} + x_j^{'} + x_3 + x_4 + x_5 + x_6 &= 34 - 11 - 11\\

x_i^{'} + x_j^{'} + x_3 + x_4 + x_5 + x_6 &= 12 \\

\end{aligned}

$$
La cantidad de soluciones a esa ecuación en $\mathbb{N}$ es $C(11, 5)$, esto equivale al cardinal de $|A_i \cap A_j|$

- $|A_i \cap A_j \cap A_k|$ = La cantidad de soluciones con $x_i \gt 10$, $x_j \gt 10$ y $x_k \gt 10$, reescribimos las restricciones de la siguiente forma:
  $$  

\begin{aligned}

x_i \ge 11\\

x_j \ge 11\\

x_k \ge 11\\

\end{aligned}

$$
declaramos las siguientes variables:
$$  

\begin{aligned}

x_i^{'} &= x_i - 11\\

x_j^{'} &= x_i - 11\\

x_k^{'} &= x_i - 11\\

\end{aligned}

$$
Reescribimos la ecuación con las nuevas variables:
$$  

\begin{aligned}

(x_i^{'} + 11) + (x_j^{'} + 11) + (x_k^{'} + 11) + x_4 + x_5 + x_6 &= 34\\

x_i^{'} + x_j^{'} + x_k^{'} + x_4 + x_5 + x_6 &= 34 - 11 - 11 -11\\

x_i^{'} + x_j^{'} + x_k^{'} + x_4 + x_5 + x_6 &= 1 \\

\end{aligned}

$$
Notar que si queremos resolver esa ecuación en $\mathbb{N}$ no va a ser posible porque como mínimo cada variable tendría un valor de 1, lo que equivale a 6, en este caso tenemos un absurdo, por lo tanto $A_i \cap A_j \cap A_k = \emptyset$ 

Para los demás cardinales nos vamos a encontrar con el mismo escenario.

Ahora reemplazamos los cardinales en la expresión inclusión-exclusión

$$

C(33,5) - \begin{pmatrix} 6 \\ 1 \end{pmatrix} C(22,5)

+ \begin{pmatrix} 6 \\ 2 \end{pmatrix} C(11,5)

$$
Esto equivale a la cantidad de soluciones de la ecuación del enunciado con las restricciones dadas.
