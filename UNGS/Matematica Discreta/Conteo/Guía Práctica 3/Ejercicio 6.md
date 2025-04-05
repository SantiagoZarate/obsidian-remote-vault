---
tags:
  - Ecuación-Linear
  - Inclusión-Exclusión
status: Done
correcto: true
---

## Una Urna Contiene 7 Bolitas Blancas, 8 Bolitas Rojas, 4 Bolitas Amarillas Y 6 Bolitas Negras. Se Extraen, Una a Una, 7 Bolitas De la Urna Sin Reponerlas. ¿Cuántas Combinaciones De Cantidades De Bolitas De Cada Color Pueden Resultar De Dicha Extracción?

**Respuesta**

> [!tip] Unidades limitadas
> No podemos usar el teorema de combinatoria con elementos repetidos porque no tenemos una cantidad ilimitada de las bolitas, fijarse que tenemos que tomar 7 bolitas, pero por ejemplo para las bolitas amarillas tenemos como máximo 4.

Definamos las siguientes variables:

$$  
\begin{aligned}
x_1 &= \text{Cantidad de bolitas blancas}\\
x_2 &= \text{Cantidad de bolitas rojas}\\
x_3 &= \text{Cantidad de bolitas amarillas}\\
x_4 &= \text{Cantidad de bolitas negras}\\
\end{aligned}
$$ 

Observemos que el problema se puede resolver obteniendo la cantidad de soluciones de la siguiente ecuación:

$$
x_1 + x_2 + x_3 + x_4 =7
$$

Con las restricciones:

$$  
\begin{aligned}
0 \le &x_1 \le 7\\
0 \le &x_2 \le 8\\
0 \le &x_3 \le 4\\
0 \le &x_4 \le 6\\
\end{aligned}
$$ 

Notar que la cota superior de $x_1$ y $x_2$ no nos influyen porque según la ecuación planteada, la suma debe ser igual a 7.

Definimos el conjunto $S$ cuyos elementos son las soluciones en $\mathbb{Z} \ge 0$ de la ecuación:

$$
x_1 + x_2 + x_3 + x_4 =7
$$

definimos las siguientes propiedades:

$$  
\begin{aligned}
P_1 &= x_3 > 4\\
P_2 &= x_4 > 6\\
\end{aligned}
$$

y los subconjuntos $A_1$ de $S$ tal que sus elementos satisfacen $P_1$ y $A_2$ de $S$ tal que sus elementos satisfacen la propiedad $P_2$, Bajo estas condiciones el problema se resuelve calculando el cardinal $\overline{A_1} \cap \overline{A_2}$ para ello vamos a usar el principio inclusión-exclusión para 2 propiedades.

$$
|\overline{A_1} \cap \overline{A_2}| =
|S| - |A_1| - |A_2| + 
|A_1 \cap A_2|
$$

Calculemos los cardinales.

- $|S|$ = La cantidad de soluciones a la ecuación planteada en $\mathbb{Z} \ge 0$, por teorema 2 sabemos que es $C(10,3)$
- $|A_1|$ = La cantidad de soluciones a la ecuación pero con $x_3 \gt 4$
Las restricción entonces es:
$$
x_3 \ge 5
$$

Definimos $x_3^{'} = x_3 - 5 \Rightarrow x_3^{'} \ge 0$

Ahora reescribimos la ecuación usando la nueva variable:

$$  
\begin{aligned}
x_1 + x_2 + x_3^{'} + x_4 &= 7\\
x_1 + x_2 + x_3^{'} + x_4 &= 7 - 5\\
x_1 + x_2 + x_3^{'} + x_4 &= 2\\
\end{aligned}
$$

Entonces la cantidad de soluciones para esa ecuación en $\mathbb{Z} \ge 0$ , por teorema 2 es $C(5, 3)$, esto equivale a $|A_1|$

- $|A_2|$ = Seguimos el mismo razonamiento para calcular $|A_1|$, pero con otra restricción para otra variable, en este caso $x_4 \gt 6$, entonces reescribimos esta restricción como
$$
x_4 \ge 7
$$

Declaramos la variable $x_4^{'} = x_4 - 7$

Y reescribimos la ecuación usando la nueva variable:

$$  
\begin{aligned}
x_1 + x_2 + x_3 + x_4^{'} &= 7\\
x_1 + x_2 + x_3 + x_4^{'} &= 7 - 7\\
x_1 + x_2 + x_3 + x_4^{'} &= 0\\
\end{aligned}
$$

Entonces la cantidad de soluciones para esa ecuación en $\mathbb{Z} \ge 0$ es $C(3,3)$, esto seria el cardinal de $A_2$

- $|A_1 \cap A_2|$ = La cantidad de soluciones con $x_3 \gt 4$ y $x_4 \gt 6$, reescribimos las restricciones de la siguiente manera:
$$ x_3 \ge 5; x_4 \ge 7$$
Notar que con esas restricciones, si $x_4$ tiene que ser como mínimo 7, las demás variables deberían ser iguales a 0 para satisfacer la ecuación, pero en este caso deberíamos asignarme un 5 a $x_3$ por lo que resulta absurdo, por lo tanto $A_1 \cap A_2 = \emptyset$

Ahora reemplazamos los cardinales en la expresión del principio inclusión-exclusión.

$$
C(10,3) - C(5,3) - C(3,3)
$$

Esto equivale a la cantidad de combinaciones que se pueden obtener de las extracciones de las bolitas del enunciado
