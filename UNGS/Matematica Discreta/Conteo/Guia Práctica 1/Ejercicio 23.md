---
tags:
  - Permutación-Circular
  - Multiplicidad
---

## ¿De Cuántas Maneras Se Pueden Sentar Ocho Personas Alrededor De Una Mesa Redonda? ¿Y Si Hubiera Dos De Ellas Que Tienen Que Sentarse Juntas Necesariamente?

**Respuesta**

Observar que podríamos ordenar las sillas en forma de hilera una después de la otra, por lo que necesitamos contar los ordenamientos de 8 personas, es decir $P(8,8)$, ahora como lo pedido establece la condición de que las sillas están ordenadas en una mesa redonda, y estas son 8, significa que cada 8 ordenamientos en hilera tenemos 1 ordenamiento circular único.

por lo que la cantidad de maneras de contar los ordenamientos de los pedido en el enunciado es:

$$
\frac{1}{8}\cdot P(8,8) 
$$

En este caso en particular, donde se nos pide las n-permutaciones circulares podemos concluir el problema diciendo que las formas en ordenar las 8 personas en una mesa redonda es $7!$

---

En el caso de que dos personas se sienten juntas necesariamente, definamos el conjunto $P$ = {$P_1$, $P_2$, ..., $P_8$} cuyos elementos representan a las personas. $P_1$ y $P_2$ tienen que estar juntos obligatoriamente, así que definamoslo como $X$ = {$P_1$, $P_2$}

Ahora definamos el conjunto $M$ = {$X$, $P_3$, ..., $P_8$} cuyos elementos son las personas restantes y el par de personas que se sientan juntas.

Debemos calcular el número de 7-permutaciones de un conjunto de 7 elementos, lo que es igual a $6!$ notar que nos faltan contar los ordenamientos de las dos personas que debe ir juntas, es decir, contar las 2 permutaciones del conjunto X, que tiene dos elementos, lo que es igual a $2!$

Para cada uno de los $2!$ ordenamientos de las personas juntas, tengo $6!$ ordenamientos circulares, así que principio multiplicativo tengo que las formas de sentar a las personas teniendo en cuenta en lo pedido en la segunda parte del enunciado es:

$$
2! \cdot 6!
$$
