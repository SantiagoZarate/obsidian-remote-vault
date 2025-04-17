## Encontrar la Cantidad De Soluciones En Los Números Naturales De

$$x_1 + x_2 + x_3 = 12$$

que satisfacen las siguientes condiciones

$$  
\begin{aligned}
1 \le &x_1 \le 3\\
1 \le &x_2 \le 8\\
3 \le &x_3 \le 6.
\end{aligned}
$$ 
**Respuesta**

Hacemos una corrección a $x_3$ para que su limite inferior coincida con el primer valor apto pertenecientes a los naturales.

$$ 1 \le x_3 - 2 \le 4$$

Declaramos las siguientes variables:

$$  
\begin{aligned}
a &= x_1\\ 
b &= x_2\\
c &= x_3 - 2\\
\end{aligned}
$$

Reescribimos la ecuación:

$$  
\begin{aligned}
a + b + c &= x_1 + x_2 + (x_3 - 2)\\
a + b + c &= \underline{x_1 + x_2 + x_3} - 2\\
a + b + c &= 12 - 2\\
a + b + c &= 10\\
\end{aligned}
$$

Ahora nuestro problema se resume obtener la cantidad de soluciones en los naturales para esa ecuación.

Sea $S$ el conjunto cuyos elementos son las soluciones en los naturales de la ecuación:

$$ a + b + c = 10$$

Definimos las propiedades:

$$  
\begin{aligned}
P_1 &= a \ge 4\\
P_2 &= b \ge 9\\
P_3 &= c \ge 5\\
\end{aligned}
$$

y los subconjuntos $A_i$ de $S$ tal que $1 \le i \le 3$ de modo que los elementos de $A_i$ satisfacen la propiedad $P_i$, para resolver el problema debemos calcular el cardinal de $\overline{A_1} \cap \overline{A_2} \cap \overline{A_3}$ para ello usaremos el principio I-E para tres propiedades.

$$  
\begin{aligned}
|\overline{A_1} \cap \overline{A_2} \cap \overline{A_3}| =\\
|S| - |A_1| - |A_2| - |A_3| +
|A_1 \cap A_2| + |A_1 \cap A_3| + |A_2 \cap A_3| -
|A_1 \cap A_2 \cap A_3|
\end{aligned}
$$

Antes de calcular los cardinales, declaremos las siguientes variables que nos van a ser útiles para agilizar el calculo de cada cardinal.

$$  
\begin{aligned}
a^{'} &= a - 3 \Rightarrow a^{'} \ge 1\\
b^{'} &= b - 8 \Rightarrow b^{'} \ge 1\\
c^{'} &= c - 4 \Rightarrow c^{'} \ge 1\\
\end{aligned}
$$

Ahora si calculemos los cardinales.

- $|S|$ = La cantidad de soluciones a la ecuación, por teorema es $\begin{pmatrix} 9 \\ 2 \end{pmatrix}$
- $|A_1|$ = La cantidad de soluciones con $a \ge 4$, para eso reescribimos la ecuación usando $a^{'}$:
  $$  

\begin{aligned}

(a^{'} + 3) + b + c &= 10\\

a^{'} + b + c &= 10 - 3\\

a^{'} + b + c &= 7\\

\end{aligned}

$$
Luego la cantidad de soluciones es $\begin{pmatrix} 6 \\ 2 \end{pmatrix}$
- $|A_2|$ = La cantidad de soluciones con $b \ge 9$, para eso reescribimos la ecuación usando $b^{'}$
  $$  

\begin{aligned}

a + (b^{'} + 8) + c &= 10\\

a + b^{'}+ c &= 10 - 8\\

a + b^{'}+ c &= 2\\

\end{aligned}

$$
Veamos que no hay soluciones para esa ecuación en los naturales.
- $|A_3|$ =  La cantidad de soluciones con $c \ge 5$, reescribimos la ecuación usando $c^{'}$:
  $$  

\begin{aligned}

a + b + (c^{'} + 4) &= 10\\

a + b + c^{'} &= 10 - 4\\

a + b + c^{'} &= 6\\

\end{aligned}

$$ 
Luego la cantidad de soluciones es $\begin{pmatrix} 5 \\ 2 \end{pmatrix}$
- $|A_1 \cap A_2|$ = La cantidad de soluciones con $a \ge 4$ y $b \ge 9$, observemos que cuando quisimos calcular $|A_2|$ obtuvimos ninguna soluciones debido a la restricción que tiene la variable $b$, por lo tanto ese caso se repite en este calculo.
- $|A_1 \cap A_3|$ = La cantidad de soluciones con $a \ge 4$ y $c \ge 5$, reescribimos la ecuación usando $a^{'}$ y $c^{'}$:
  $$  

\begin{aligned}

(a^{'} + 3) + b + (c^{'} + 4) &= 10\\

a^{'}+ b + c^{'} &= 10 - 7\\

a^{'}+ b + c^{'} &= 3\\

\end{aligned}

$$
Luego la cantidad de soluciones es $\begin{pmatrix} 2 \\ 2 \end{pmatrix}$
- $|A_2 \cap A_3|$ = Sucede lo mismo que en el calculo de $|A_2|$, por lo tanto la soluciones son nulas
- $|A_1 \cap A_2 \cap A_3|$ = La cantidad de soluciones con $a \ge 4$, $b \ge 9$ y $c \ge 5$, aca ocurre lo mismo que en el cálculo de $|A_2|$, por lo que el conjunto de soluciones es vacío.

Ahora remplazamos los cardinales:

$$\begin{pmatrix} 9 \\ 2 \end{pmatrix}
- \begin{pmatrix} 6 \\ 2 \end{pmatrix}
- \begin{pmatrix} 5 \\ 2 \end{pmatrix}
+ \begin{pmatrix} 2 \\ 2 \end{pmatrix}
$$

Esto equivale a la cantidad de soluciones a la ecuación del enunciado con sus respectivas restricciones.
