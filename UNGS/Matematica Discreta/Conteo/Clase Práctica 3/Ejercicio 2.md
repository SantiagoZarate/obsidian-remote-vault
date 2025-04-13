---
tags:
  - Sustacción
  - Permutación-Repetidos
status: Done
---

## ¿Cuántos n´umeros Distintos De Ocho Cifras Y Mayores a 20000000 Se Pueden Formar Con Los Dígitos 12277788?

**Respuesta**

Sea $S$ el conjunto cuyos elementos son los números formados por las dígitos 12277788, definamos $A \subset S$ cuyos elementos son menores a 20000000, por definición de complemento tenemos $\overline{A}$ cuyos elementos son mayores a 20000000, lo pedido en el enunciado se resuelve obteniendo $\overline{A}$, por principio de sustracción eso es igual a

$$
\overline{A} = |S| - |A|
$$

calculemos los cardinales.

- $|S|$ = Definamos el siguiente multiconjunto a partir de los dígitos del enunciado:
  $$ \{ un \cdot 1, dos \cdot 2, tres \cdot 7, dos \cdot 8 \} $$
  La cantidad de permutaciones de 8 elementos, con el tipo de elemento 2 y 8 con dos repeticiones, y el tipo de elemento 7 con tres elementos es igual a $\frac{8!}{2!\cdot2!\cdot3!}$

  Esto equivale al cardinal de $S$

- $|A|$ = Observemos que para que se cumpla la restricción de que el número sea menor a 20000000, con los dígitos que tenemos disponibles del enunciado necesitamos que empieze con el dígito 1, de esta manera nos quedan 7 números con los que podemos formar el siguiente multiconjunto:
  $$\{ dos \cdot 2, tres \cdot 7, dos \cdot 8 \}$$
  La cantidad de ordenamientos de 7 elementos con el tipo de elemento 2 y 8 con dos repeticiones, y el tipo de elemento 7 con tres repeticiones es $\frac{7!}{2!\cdot2!\cdot3!}$

Ahora podemos continuar y calcular $\overline{A}$

$$  
\begin{aligned}
\overline{A} &= |S| - |A|\\
\overline{A} &= \frac{8!}{2!\cdot2!\cdot3!} - \frac{7!}{2!\cdot2!\cdot3!}\\
\end{aligned}
$$ Esto equivale a la cantidad de números que se pueden formar con los dígitos del enunciado tal que cumplan la respectiva restricción.
