---
tags:
  - Ecuación-Linear
  - Inclusión-Exclusión
status: Done
---

## Quince Personas Quieren Realizar Un Viaje a Salta Y Utilizarán Cuatro Vehículos Distintos Para Dicho Viaje, Tres Autos Y Una Combi. Todas Las Personas Saben Manejar. ¿Cuántas Formas Distintas Hay De Distribuir la Cantidad De Personas En Los Vehículos, Si En El Auto Rojo no Pueden Viajar Más De Tres Personas, En Los Autos Azul Y Gris no Más De Cuatro Personas, Y En la Combi Por Lo Menos Deben Viajar Cuatro Personas Pero no Más De Seis?

**Respuesta**

Representaremos a los autos de la siguiente forma:

$$  
\begin{aligned}
a &= \text{Cantidad de personas que viajan en el auto rojo}\\
b &= \text{Cantidad de personas que viajan en el auto azul}\\
d &= \text{Cantidad de personas que viajan en el auto gris}\\
c &= \text{Cantidad de personas que viajan en la combi}\\
\end{aligned}
$$ 

Lo pedido en el enunciado se obtiene resolviendo la siguiente ecuación:

$$ a + b + c + d = 15 $$

con las siguientes restricciones:

$$  
\begin{aligned}
a \le 3\\
b \le 4\\
c \le 4\\
4 \le d \le 6\\
\end{aligned}
$$

Hacemos una corrección a $d$ para que la cota inferior sea 0.

$$
0 \le d - 4 \le 2
$$

Definimos la siguiente variable:

$$
e = d - 4
$$

reescribimos la ecuación de la siguiente manera:

$$  
\begin{aligned}
a + b + c + e = a + b + c + (d - 4)\\
a + b + c + e = a + b + c + d - 4\\
a + b + c + e = 15 - 4\\
a + b + c + e = 11\\
\end{aligned}
$$ 

Definimos el conjunto $S$ cuyos elementos son las soluciones en $\mathbb{Z} \ge 0$ a la ecuación

$$
a + b + c + e = 11\\
$$

definimos las siguientes propiedades:

$$  
\begin{aligned}
p_1 &= a \gt 3\\
p_2 &= b \gt 4\\
p_3 &= c \gt 4\\
p_4 &= e \gt 2\\
\end{aligned}
$$

Y los subconjuntos $A_i$ de $S$ con $1 \le i \le 4$ donde los elementos de $A_i$ satisfacen la propiedad $p_i$. Bajo estas condiciones lo pedido en el enunciado se resuelve obteniendo el cardinal de $\overline{A_1} \cap \overline{A_2} \cap \overline{A_3} \cap \overline{A_4}$ , para ello usaremos el principio I-E para 4 propiedades.

Reescribamos las restricciones de las propiedades de la siguiente manera:

$$  
\begin{aligned}
p_1 &= a \ge 4\\
p_2 &= b \ge 5\\
p_3 &= c \ge 5\\
p_4 &= e \ge 3\\
\end{aligned}
$$

Y definamos las siguientes variables que nos van a servir para encontrar los cardinales de las uniones de subconjuntos de la expresión del principio I-E

$$  
\begin{aligned}
a^{'} &= a - 4\\
b^{'} &= b - 5\\
c^{'} &= c - 5\\
e^{'} &= e - 3\\
\end{aligned}
$$ 

Ahora calculemos los cardinales:

- $|S|$ = $C(14,3)$
- $|A_1|$ = $C(10, 3)$
$$  
\begin{aligned}
(a^{'} + 4) + b + c + e &= 11\\
a^{'} + b + c + e &= 11 - 4\\
a^{'} + b + c + e &= 7\\
\end{aligned}
$$
- $|A_2|$ =$C(9, 3)$
$$  
\begin{aligned}
a + (b^{'} + 5) + c + e &= 11\\
a + b^{'} + c + e &= 11 - 5\\
a + b^{'} + c + e &= 6\\
\end{aligned}
$$
- $|A_3|$ = Resulta lo mismo que el cardinal de $A_2$ ya que tiene la misma restricción pero en otra variable.
- $|A_4|$ = $C(11,3)$

$$
\begin{aligned}
a + b + c + (e^{'} + 3) &= 11\\
a + b + c + e^{'} &= 11 - 3\\
a + b + c + e^{'} &= 8\\
\end{aligned}
$$
- $|A_1 \cap A_2|$ = $C(5, 3)$

$$
\begin{aligned}
(a^{'} + 4) + (b^{'} + 5) + c + e &= 11\\
a^{'} + b^{'} + c + e &= 11 - 4 - 5\\
a^{'} + b^{'} + c + e &= 2\\
\end{aligned}
$$
- $|A_1 \cap A_3|$ = Resulta lo mismo que el cardinal anterior
- $|A_1 \cap A_4|$ = $C(7, 3)$

$$
\begin{aligned}
(a^{'} + 4) + b + c + (e^{'} + 3) &= 11\\
a^{'} + b + c + e^{'} &= 11 - 4 - 3\\
a^{'} + b + c + e^{'} &= 4\\
\end{aligned}
$$
- $|A_2 \cap A_3|$ = $C(4, 3)$

$$
\begin{aligned}
a + (b^{'} + 5) + (c^{'} + 5) + e &= 11\\
a + b^{'} + c^{'} + e &= 11 - 5 - 5\\
a + b^{'} + c^{'} + e &= 1\\
\end{aligned}
$$
- $|A_2 \cap A_4|$ = $C(6, 3)$

$$
\begin{aligned}
a + (b^{'} + 5) + c + (e^{'} + 3) &= 11\\
a + b^{'} + c + e^{'} &= 11 - 5 - 3\\
a + b^{'} + c + e^{'} &= 3\\
\end{aligned}
$$
- $|A_3 \cap A_4|$ = Resulta lo mismo que el cardinal anterior
- $|A_1 \cap A_2 \cap A_3|$ = $0$

$$
\begin{aligned}
(a^{'} + 4) + (b^{'} + 5) + (c^{'} + 5) + e &= 11\\
a^{'} + b^{'} + c^{'} + e &= 11 - 4 - 5 - 5\\
a^{'} + b^{'} + c^{'} + e &= -3\\
\end{aligned}
$$

Luego la cantidad de soluciones a esa ecuación en $\mathbb{Z} \ge 0$ es 0, lo mismo se cumple en los restantes cardinales.

Ahora reemplazamos los cardinales.

$$  
\begin{aligned}
C(14,3) - C(10, 3) - 2 \cdot C(9, 3) - C(11, 3) \\+ 2 \cdot C(5, 3) + C(7, 3) + C(4, 3) + 2 \cdot C( 6,3)
\end{aligned}
$$ 

Esto equivale a la cantidad de formas distintas de distribuir a las personas en los vehículos presentados en el enunciado con sus restricciones.
