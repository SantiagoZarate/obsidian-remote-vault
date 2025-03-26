---
tags:
  - Permutación-Repetidos
status: Done
---

## ¿De Cuántas Formas Se Pueden Ordenar 4 Letras X, 5 Letras Y, 6 Letras Z Y 2 Letras W?

**Respuesta**

Observemos que podemos ordenar las letras formando una palabra, es decir un ordenamiento en hilera:

$$
\underline{XXXX}\,\underline{YYYYY}\,\underline{ZZZZZZ}\,\underline{WW}
$$

Definimos el siguiente multiconjunto $S$ a partir de esa palabra:

$$
\{ 4 \cdot X, 5 \cdot Y, 6 \cdot Z, 2 \cdot W \}
$$

Ahora que tenemos el multiconjunto $S$ con 4 tipos distintos de elementos, el número de permutaciones de los 17 elementos de $S$ es:

$$
\frac{17!}{4!\cdot5!\cdot6!\cdot2!}
$$

Entonces esa es la cantidad de formas que se pueden ordenar las letras del enunciado.
