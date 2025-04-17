## Calcular El Número De Soluciones En Los Naturales De la Ecuación

$$x + y + z = 29$$

que satisfacen las siguientes condiciones $x ≤ 7, y ≤ 7$ y $z ≤ 16$

**Respuesta**

Sea $S$ el conjunto cuyos elementos son las soluciones en $\mathbb{N}$ de la ecuación planteada en el enunciado, definimos las siguientes propiedades:

$$  
\begin{aligned}
P_1 &= x \gt 7\\
P_2 &= y \gt 7\\
P_3 &= z \gt 16\\
\end{aligned}
$$

y los subconjunto $A_i$ con $1 \le i \le 3$ tal que los elementos de $A_i$ satisfacen la propiedad $P_i$, lo pedido en el enunciado se resuelve calculando el cardinal de $\overline{A_1} \cap \overline{A_2} \cap \overline{A_3}$ para ello usaremos el principio I-E para tres propiedades.

$$  
\begin{aligned}
|\overline{A_1} \cap \overline{A_2} \cap \overline{A_3}| =\\
|S| - |A_1| - |A_2| - |A_3| +
|A_1 \cap A_2| + |A_1 \cap A_3| + |A_2 \cap A_3| -
|A_1 \cap A_2 \cap A_3|
\end{aligned}
$$

Antes de calcular los cardinales, reescribamos las restricciones de las propiedades de la siguiente manera:

$$  
\begin{aligned}
P_1 = x \ge 8\\
P_2 = y \ge 8\\
P_3 = z \ge 17\\
\end{aligned}
$$

y declaramos las siguientes variables que vamos a usar luego para calcular los cardinales:

$$  
\begin{aligned}
x^{'} &= x - 7 \Rightarrow x^{'} \ge 1\\
y^{'} &= y - 7 \Rightarrow y^{'} \ge 1\\
z^{'} &= z - 16 \Rightarrow z^{'} \ge 1\\
\end{aligned}
$$ 

Calculemos los cardinales:

- $|S|$ = La cantidad de soluciones, por teorema 2 de ecuaciones lineares con coeficientes naturales eso es igual a $C(31, 2)$
- $|A_1|$ = La cantidad de soluciones con $x \gt 7$, reescribimos la ecuación usando $x^{'}$:
  $$  

\begin{aligned}

 (x^{'} + 7) + y + z &= 29 \\

 x^{'} + y + z &= 29 - 7 \\

 x^{'} + y + z &= 22 \\

\end{aligned}

$$
Ahora la cantidad de soluciones es $C(21,2)$ 
- $|A_2|$ = Resulta lo mismo que el calculo de $|A_1|$ ya que es la misma restricción pero en otra variable.
- $|A_3|$ = La cantidad de soluciones con $z \lt 16$, reescribimos la ecuación usando $z^{'}$:
  $$  

\begin{aligned}

x + y + (z^{'} + 16) &= 29\\

x + y + z^{'} &= 29 - 16\\

x + y + z^{'} &= 13\\

\end{aligned}

$$ Luego la cantidad de soluciones es $\begin{pmatrix} 12 \\ 2 \end{pmatrix}$

- $|A_1 \cap A_2|$ = La cantidad de soluciones con $x \gt 7$ y $y \gt 7$, reescribimos la ecuación usando $x^{'}$ y $y^{'}$:
  $$  

\begin{aligned}

(x^{'} + 7) + (y^{'} + 7) + z &= 29\\

x^{'} + y^{'} + z &= 29 - 14\\

x^{'} + y^{'} + z &= 15\\

\end{aligned}

$$
Entonces la cantidad de soluciones es $\begin{pmatrix} 14 \\ 2 \end{pmatrix}$
- $|A_1 \cap A_3|$ = La cantidad de soluciones con $x \lt 7$ y $z \lt 16$, reescribimos la ecuación usando $x^{'}$ y $z^{'}$:
  $$  

\begin{aligned}

(x^{'} + 7) + y + (z^{'} + 16) &= 29\\

x^{'} + y + z^{'} &= 29 - 23\\

x^{'} + y + z^{'} &= 6\\

\end{aligned}

$$
Luego la cantidad de soluciones es $\begin{pmatrix} 5 \\ 2 \end{pmatrix}$
- $|A_2 \cap A_3|$ = Resulta lo mismo que el calculo de $|A_1 \cap A_3|$ ya que tenemos las mismas restricciones en distintas variables
- $|A_1 \cap A_2 \cap A_3|$ = La cantidad de soluciones con $x \lt 7$, $y \lt 7$ y $z \lt 16$, reescribimos la ecuación usando las nuevas variables:
  $$  

\begin{aligned}

(x^{'} + 7) + (y^{'} + 7) + (z^{'} + 16) = 29\\

x^{'} + y^{'} + z^{'} = 29 - 30\\

x^{'} + y^{'} + z^{'} = -1\\

\end{aligned}

$$
Veamos que no existen soluciones para esa ecuación en $\mathbb{N}$

Ahora reemplazamos los cardinales en la expresión del principio I-E para tres propiedades:
$$

\begin{pmatrix} 31 \\ 2 \end{pmatrix} -

2 \cdot\begin{pmatrix} 21 \\ 2 \end{pmatrix} -

\begin{pmatrix} 12 \\ 2 \end{pmatrix}

+ 2 \cdot \begin{pmatrix} 14 \\ 2 \end{pmatrix}

+ \begin{pmatrix} 5 \\ 2 \end{pmatrix}

$$
