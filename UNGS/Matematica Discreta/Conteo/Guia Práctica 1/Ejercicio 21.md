## Se Quiere Diseñar Una Bandera Compuesta Por Al Menos Dos Y a Lo Sumo Cinco Rayas Verticales. Si Cada Raya Tiene Que Ser De Distinto Color Y Se Dispone De Ocho Colores Distintos Para Diseñarla. ¿De Cuántas Formas Distintas Se Puede Diseñar la Bandera?

**Respuesta**

Observemos que el orden de aparición de los colores importa, supongamos tenemos una bandera compuesta por dos rayas verticales, si la formamos de color ROJO y AZUL, va a ser una bandera diferente a la que se forma con el AZUL y ROJO.

Sea $S$ el conjunto cuyos elementos son las formas de armar la bandera con lo pedido en el enunciado, definimos los siguientes subconjuntos de $S$

$$  
\begin{aligned}
S_1 &= \text{Banderas con 2 rayas vericales}\\
S_2 &= \text{Banderas con 3 rayas vericales}\\
S_3 &= \text{Banderas con 4 rayas vericales}\\
S_4 &= \text{Banderas con 5 rayas vericales}\\
\end{aligned}
$$

Notemos que $S = S_1 \cup S_2 \cup S_3 \cup S_4$ y que $S_i \cap S_j = \emptyset$ siempre que $i \neq j$, por lo tanto los subconjuntos definidos es una partición de $S$, por lo que por principio aditivo tenemos que

$$|S| = |S_1| + |S_2| + |S_3| + |S_4|$$

Nos interesa Calcular $|S|$, primero necesitamos calcular el cardinal de cada subconjunto

Para calcular el cardinal de $S_1$ tenemos que contar los ordenamientos de 2 colores de los 8 disponibles, lo que es $P(8,2)$, este mismo análisis se usa con los demás subconjuntos. entonces nos queda que:

$$  
\begin{aligned}
S_1 &= P(8,2)\\
S_2 &= P(8,3)\\
S_3 &= P(8,4)\\
S_4 &= P(8,5)\\
\end{aligned}
$$

Ahora podemos obtener el resultado de $|S|$:

$$  
\begin{aligned}
|S| = P(8,2) + P(8,3) + P(8,4) + P(8,5)
\end{aligned}
$$

Esa sería la cantidad de banderas distintas que se pueden formar con las restricciones del enunciado
