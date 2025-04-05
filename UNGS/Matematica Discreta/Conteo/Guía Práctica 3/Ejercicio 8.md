---
tags:
  - Ecuación-Linear
  - Inclusión-Exclusión
status: Incomplete
correcto: false
---

## ¿De Cuántas Formas Se Pueden Ordenar 18 Bolas Negras Iguales Entre Sí En 3 Cajas Numeradas De Forma Tal Que Se Cumplan Las Siguientes Condiciones?

**a)** La primera caja contiene al menos 2 bolas y a lo sumo 5.

**b)** La primera caja contiene al menos 3 bolas y a lo sumo 7.

**c)** La primera caja contiene al menos 4 bolas y a lo sumo 8.

**Respuesta**

> [!NOTE] Soy un boludo
> Junté todas las restricciones en un solo punto

$$
x_1 + x_2 + x_3 = 18
$$

con las restricciones:

$$ 
\begin{aligned}
2 \le x_1 \le 5\\
3 \le x_2 \le 7\\
4 \le x_3 \le 8\\
\end{aligned}
$$

Hacemos una corrección para cada una de las restricciones para que la cota inferior sea 0.

$$  
\begin{aligned}
2 \le x_1 \le 5 = 0 \le x_1 - 2 \le 3 \\
3 \le x_2 \le 7 = 0 \le x_2 - 3 \le 4 \\
4 \le x_3 \le 8 = 0 \le x_3 - 4 \le 4 \\
\end{aligned}
$$

Definimos las siguientes variables:

$$  
\begin{aligned}
a &= x_1 - 2\\
b &= x_2 - 3\\
c &= x_3 - 4\\
\end{aligned}
$$ 

Luego reescribimos la ecuación:

$$  
\begin{aligned}
a + b + c &= x_1 - 2 + x_2 - 3 + x_3 - 4\\
a + b + c &= (x_1 + x_2 + x_3) - (2 + 3 +4)\\
a + b + c &= 18 - 9\\
a + b + c &= 9
\end{aligned}
$$

nos queda por resolver la ecuación $a + b + c = 9$ con las siguientes restricciones:

$$  
\begin{aligned}
a \le 3\\
b \le 4\\
c \le 4
\end{aligned}
$$

Para eso definimos $S$ el conjunto cuyos elementos son las soluciones en $\mathbb{Z} \ge 0$ de la ecuación planteada, definimos las siguientes propiedades:

$$  
\begin{aligned}
p_1 &= a \gt 4\\
p_2 &= b \gt 5\\
p_1 &= c \gt 5\\
\end{aligned}
$$

Y los subconjuntos $A_i$ de $S$ con $1 \le i \le 2$ tal que los elementos de $A_i$ satisfacen la propiedad $p_i$. Bajo estos términos resolver el problema es igual a calcular el cardinal de $a_1 \cap a_2 \cap a_3$ para ello haremos uso del principio inclusión-exclusión para tres propiedades:

$$  
\begin{aligned}
|\overline{A_1} \cap \overline{A_2} \cap \overline{A_3}| =
|S| - |A_1| - |A_2| - |A_3| +
|A_1 \cap A_2| + |A_1 \cap A_3| + |A_2 \cap A_3| -\\
|A_1 \cap A_2 \cap A_3|
\end{aligned}
$$

Ahora nos toca calcular los cardinales.

- $|S|$= La cantidad de soluciones de la ecuación en $\mathbb{Z} \gt 0$, por teorema 2 sabemos que es $C(11, 2)$
- $|A_1|$= La cantidad de soluciones de la ecuación con $a \gt 4$, podemos reescribir la restricción de la siguiente manera:
$$
a \ge 5
$$

Definimos la siguiente variable:

$$
a^{'} = a - 5
$$

Reescribimos la ecuación con la nueva variable:

$$  
\begin{aligned}
(a^{'} + 5) + b + c &= 9\\
a^{'}  + b + c &= 9 - 5\\
a^{'}  + b + c &= 4\\
\end{aligned}
$$

Entonces el cardinal de $A_1$ es la cantidad de soluciones de esa ecuación en $\mathbb{Z} \ge 0$, por teorema 2 sabemos que es $C(6, 2)$

- $|A_2|$= La cantidad de soluciones de la ecuación con $b \gt 5$, podemos reescribir la restricción de la siguiente manera:
$$b \ge 6$$
Definimos la siguiente variable:
$$
b^{'} = b - 6
$$

Reescribimos la ecuación:

$$  
\begin{aligned}
a + (b^{'} + 6) + c &= 9\\
a + b^{'} + c &= 9 - 6\\
a + b^{'} + c &= 3\\
\end{aligned}
$$

Luego el cardinal de $A_2$ es la cantidad de soluciones de esa ecuación en $\mathbb{Z} \ge 0$, lo cual es igual a $C(5, 2)$

- $|A_3|$ = Resulta el mismo que el cardinal de $A_2$ puesto que tiene la misma condición solo que en otra variable
- $|A_1 \cap A_2|$ = La cantidad de soluciones de la ecuación con $a \gt 4$ y $b \gt 5$, podemos reescribir las restricciones de la siguiente manera:
$$  
\begin{aligned}
a \ge 5 \\
b \ge 6 \\
\end{aligned}
$$

Notar que bajo esas restricciones, si la variable $a$ es como mínimo 5, y la variable $b$ como mínimo 6, la variable $c$ debería tener un valor negativo, y como estamos tratando de encontrar las soluciones dentro en $\mathbb{Z} \ge 0$ eso es absurdo, por lo que $A_1 \cap A_2 = \emptyset$.

Este misma característica se cumple al querer calcular los restantes cardinales.

Ahora remplazamos los cardinales que pudimos obtener.

$$
C(11,2) - C(6,2) - 2 \cdot C(5,2)
$$

Esto equivale a la cantidad de formas de ordenar las bolas en las tres cajas teniendo en cuenta las restricciones del enunciado.
