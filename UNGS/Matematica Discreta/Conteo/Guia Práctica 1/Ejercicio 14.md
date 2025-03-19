---
tags:
  - Adición
  - Combinación
---

## Se Tienen Siete Puntos Distintos Sobre Una Recta Y Otros Seis Puntos Sobre Una Recta Paralela a la Anterior. ¿Cuántos Triángulos Distintos Se Pueden Formar?

> [!Análisis]
>
> Como mínimo tengo que tomar 1 por recta y como máximo 2, puedo tomar dos puntos consecutivos o dos puntos totalmente alejados eso no importa, Al momento de formar un triangulo los puntos que tomo de una recta no pueden ser los mismo.
>
> Si tomo dos puntos de la recta A puedo tomar cualquiera de la otra, eso me marca la dependencia entre ellas, seguro use el principio multiplicativo
>
> Tomo el punto 1 y 2 de la recta A, puedo agarrar cualquiera de B, tomo el punto 1 y 3, puedo agarrar cualquier de B, lo mismo funciona desde B hacia A
>
> Notar que si formo un triangulo con los puntos A1, A2 y B1 es el mismo triangulo que se forma si elijo los puntos B1, A2, A1

Se define el conjunto $A$ = {$A_1$, $A_2$, ..., $A_7$} y $B$ = {$B_1$, $B_2$, ..., $B_6$} cuyos elementos representan puntos en una recta.

Sea el conjunto S cuyos elementos son elementos de $A$ y $B$ tomados de a grupos de a 3 donde no pueden haber mas de 2 elementos de un mismo conjunto por grupo.

ejemplos de elementos de $S$:

- {$A_1$, $A_2$, $B_1$}
- {$A_1$, $A_2$, $B_2$}

Lo pedido en el enunciado se resuelve calculando $|S|$.

Definamos los siguientes subconjunto de $S$

$$  
\begin{aligned}
S_1 = \text{Elementos con 2 elementos de A}\\
S_2 = \text{Elementos con 2 elementos de B}\\
\end{aligned}
$$

Notemos que $S = S_1 \cup S_2$ y que $S_1 \cap S_2 = \emptyset$, por lo tanto $S_1$ y $S_2$ es una partición de $S$, por lo que $|S| = |S_1| + |S_2|$

Para calcular el cardinal de $S_1$ hay que contar las combinaciones $A$ tomando 2 elementos, es decir $C(7,2)$, para cada una de las combinaciones vamos a contar con todos los elementos de $B$, entonces:

$$
|S_1| = C(7,2) \cdot 6
$$

Para calcular el cardinal de $|S_2|$ seguimos un análisis análogo al subconjunto anterior, solo que en este caso varía los elementos disponibles que podemos combinar que es $C(6,2)$, para cada una de las combinaciones vamos a contar con todos los elementos de A, entonces:

$$
|S_2| = C(6,2) \cdot 7
$$

Una vez calculamos el cardinal de ambos subconjuntos, por principio aditivo calculamos $|S|$:

$$|S| = C(7,2) \cdot 6 + C(6,2) \cdot 7$$
