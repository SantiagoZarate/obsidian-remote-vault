## Por El Fallecimiento De Akira Toriyama, la Empresa Bandai Decide Producir Una Edición Limitada De Figuras De Dragon Ball. Las Figuras Disponibles Serán Goku, Vegeta, Piccolo, Bills, Freezer Y Cell. Suponiendo Que Se Fabricarán 1000 Figuras, Donde Habrá

al menos 50 de cada tipo, no más de 100 de Goku, como mucho 100 de Vegeta y a lo sumo 100 de Cell.

¿Cuántas formas distintas de fabricar las 1000 figuras hay?

**Respuesta**

Declaremos las siguientes variables:

$$  
\begin{aligned}
x_1 &= \text{Cantidad de figuras de Goku}\\
x_2 &= \text{Cantidad de figuras de Vegetta}\\
x_3 &= \text{Cantidad de figuras de Piccolo}\\
x_4 &= \text{Cantidad de figuras de Bills}\\
x_5 &= \text{Cantidad de figuras de Freezer}\\
x_6 &= \text{Cantidad de figuras de Cell}\\
\end{aligned}
$$

El problema presentando se resume a encontrar la cantidad de soluciones a la siguiente ecuación:

$$ x_1 + x_2 + x_3 + x_4 + x_5 + x_6 = 1000 $$

con las siguientes restricciones:

$$  
\begin{aligned}
50 \le &x_1 \le 100\\
50 \le &x_2 \le 100\\
50 \le &x_3 \\
50 \le &x_4 \\
50 \le &x_5 \\
50 \le &x_6 \le 100\\
\end{aligned}
$$

Hagamos la siguiente corrección para que el limite inferior sea 0 y posteriormente usar el teorema 2 de ecuaciones lineales con coeficientes unitarios.

$$  
\begin{aligned}
0 \le &x_1 - 50 \le 50\\
0 \le &x_2 - 50 \le 50\\
0 \le &x_3 - 50\\
0 \le &x_4 - 50\\
0 \le &x_5 - 50\\
0 \le &x_6 - 50\le 50\\
\end{aligned}
$$

reasignemos las variables:

 $$  
\begin{aligned}
a &= x_1 - 50\\
b &= x_2 - 50\\
c &= x_3 - 50\\
d &= x_4 - 50\\
e &= x_5 - 50\\
f &= x_6 - 50\\
\end{aligned}
$$reformulemos la ecuación inicial:

$$  

\begin{aligned}

a + b + c + d + e + f \\&= (x_1 - 50) + (x_2 - 50) + (x_3 - 50) + (x_4 - 50) + (x_5 - 50) + (x_6 - 50)

\\&=x_1 + x_2 + x_3 + x_4 + x_5 + x_6 - (50 \cdot 6)

\\&= 1000 - 300

\\&= 700

\end{aligned}

$$
Entonces el problema se resuelve encontrando las soluciones en $\mathbb{Z} \ge 0$ a esta nueva ecuación con las siguientes restricciones:
$$  

\begin{aligned}

a \le 50\\

b \le 50\\

f \le 50

\end{aligned}

$$ 
Sea $S$ el conjunto cuyos elementos son las soluciones en $\mathbb{Z} \ge 0$ a la ecuación previamente planteada, definimos las siguientes propiedades:

$$  

\begin{aligned}

P_1 &= a \ge 51\\

P_2 &= b \ge 51\\

P_3 &= f \ge 51\\

\end{aligned}

$$
y los subconjuntos $A_i$ de $S$ con $1 \le i \le 3$ tal que los elementos de $A_i$ satisfacen la propiedad $P_i$, bajo estas condiciones el problema se resuelve calculando el cardinal de $\overline{A_1} \cap \overline{A_2} \cap \overline{A_3}$, para ello usaremos el principio I-E para tres propiedades

$$\begin{aligned}
|\overline{A_1} \cap \overline{A_2} \cap \overline{A_3}| = \\
|S| - |A_1| - |A_2| - |A_3|
+ |A_1\cap A_2| + |A_1 \cap A_3| + |A_2 \cap A_3|
- |A_1 \cap A_2 \cap A_3|
\end{aligned}
$$

Antes de calcular los cardinales definamos las siguientes variables:

$$  
\begin{aligned}
a^{'} &= a - 51\\
b^{'} &= b - 51\\
f^{'} &= f - 51\\
\end{aligned}
$$

Ahora pasemos a calcular los cardinales.

- $|S|$ = $\begin{pmatrix} 705 \\ 5 \end{pmatrix}$ (Usando el teorema 2)
- $|A_1|$ = La cantidad de soluciones con $a \ge 51$, usamos la variable $a^{'}$ para reescribir la ecuación.
  $$  

\begin{aligned}

(a^{'} + 51) + b + c + d +e +f &= 700 \\

a^{'} + b + c + d +e +f &= 700 - 51 \\

a^{'} + b + c + d +e +f &= 649 \\

\end{aligned}

$$
Luego la cantidad de soluciones en $\mathbb{Z} \ge 0$ es $\begin{pmatrix} 654 \\ 5 \end{pmatrix}$
- $|A_2|$ y $|A_3|$ = Resulta lo mismo que el calculo del cardinal de  $A_1$ ya que tienen la misma restricción solo que en otras variables
- $|A_1 \cap A_2|$ = La cantidad de soluciones con $a \ge 51$ y $b \ge 51$, reescribimos la ecuación original usando $a^{'}$ y $b^{'}$.
  $$\begin{aligned}
(a^{'} + 51) + (b^{'} + 51) + c + d + e + f &= 700\\
a^{'}  + b^{'}  + c + d + e + f &= 700 - 102\\
a^{'}  + b^{'}  + c + d + e + f &= 598\\
\end{aligned}
$$ 

Luego la cantidad de soluciones es $\begin{pmatrix} 603 \\ 5 \end{pmatrix}$

- $|A_1 \cap A_3|$ y $|A_2 \cap A_3|$ = Resulta lo mismo que el cálculo del cardinal de $|A_1 \cap A_2|$
- $|A_1 \cap A_2 \cap A_3|$ = La cantidad de soluciones con $a \ge 51$, $b \ge 51$ y $f \ge 51$, reescribimos la ecuación usando $a^{'}$, $b^{'}$ y $f^{`}$.
  $$\begin{aligned}

(a^{'} + 51) + (b^{'} + 51) + c + d + e + (f^{'} + 51) &= 700\\

a^{'} + b^{'} + c + d + e + f^{'} &= 700 - 153\\

a^{'} + b^{'} + c + d + e + f^{'} &= 547\\

\end{aligned}

$$
Luego la cantidad de soluciones es $\begin{pmatrix} 552 \\ 5 \end{pmatrix}$

Ahora reemplazamos los cardinales calculados en la expresión del principio I-E para tres propiedades. Notar que tenemos resultados simétricos

$$

\begin{pmatrix} 705 \\ 5 \end{pmatrix}

- \begin{pmatrix} 3 \\ 1 \end{pmatrix} \cdot \begin{pmatrix} 654 \\ 5\end{pmatrix}
+ \begin{pmatrix} 3 \\ 2 \end{pmatrix} \cdot \begin{pmatrix} 603 \\ 5\end{pmatrix}
- \begin{pmatrix} 3 \\ 3 \end{pmatrix} \cdot \begin{pmatrix} 552 \\ 5\end{pmatrix}
$$

Esto equivale a la cantidad de formas distintas de fabricar las 1000 figuras con las restricciones que impone el enunciado.
