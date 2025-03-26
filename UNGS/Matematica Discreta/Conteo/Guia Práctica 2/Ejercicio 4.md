---
tags:
  - Permutación-Repetidos
  - Multiplicidad
status: Done
---

## Considere El Conjunto Formado Por Las Permutaciones De Todas Las Letras De la Palabra CAMPAMENTO

**a)** ¿Cuántas de estas permutaciones terminan con una A?

**b)** ¿Cuántas de estas permutaciones tienen a todas las consonantes juntas?

**c)** ¿Cuántas de estas permutaciones comienzan y terminan en la misma letra?

**Respuesta**

### **a)**

Sea $S$ el conjunto del que se habla en el enunciado, definimos $M\subset S$ cuyos elementos terminan con una A, lo pedido en el ejercicio se resuelve obteniendo $|M|$.

Si sabemos que los elementos de $M$ terminan con una A, descartamos una de las A porque va a estar fijada en la última posición, definimos siguiente multiconjunto $N$:

$$
\{ \underline{1\cdot C} , \underline{1 \cdot A},\underline{2 \cdot M}, \underline{1\cdot P}, \underline{1 \cdot E},\underline{1\cdot N}, \underline{1\cdot T},\underline{1\cdot O}  \}
$$

Ahora necesitamos contar los ordenamientos del multiconjunto $N$ teniendo en cuenta que tiene 8 clase de elementos, el número de permutaciones de sus 9 elementos es:

$$
|M| = \frac{9!}{2!} = \frac{362880}{2} = 181440
$$

Esto equivale a la cantidad de permutaciones que terminan con la letra A.

### **b)**

Para saber cuantas de estar permutaciones tienen las consonantes conjuntas definimos:

$$
X = \{ \underline{1\cdot C}, \underline{2\cdot M}, \underline{1\cdot N}, \underline{1\cdot T}  \}
$$

Notemos que nos quedan todas las vocales que forman el multiconjunto $J$:

$$
\{ \underline{2\cdot A}, \underline{1\cdot E}, \underline{1\cdot O}  \}
$$

Necesitamos calcular las permutaciones de $X$, notar que tiene 4 tipos de elementos, el número de permutaciones de 5 elementos de $X$ es:

$$
\frac{5!}{2!} = 60
$$

Por cada una estos ordenamientos el multiconjunto $J$ puede ordenarse de ciertas formas, teniendo en cuenta que tiene 3 tipos de elementos, las permutaciones de 4 elementos es:

$$
\frac{4!}{2!} = 12
$$

Notar que entre las 4 vocales, tenemos 5 espacios. por cada espacio podemos poner todas los elementos de $X$ así están todos juntos.

$$
60 \cdot 12 \cdot 5 = 3600
$$

Esto equivale a las permutaciones del conjunto del enunciado que tienen todas las consonantes juntas

### **c)**

Notar que la palabra CAMPAMENTO tiene 2 letras que se repiten más de una vez, en concreto la M y la A, podemos elegir una de las letras y fijar la primera al inicio de la palabra y la otra al final, por lo que nos quedaría por calcular los ordenamientos de las letras intermedias.

Sea cual sea la letra que elegimos poner al inicio y al final, el multiconjunto del que habría que calcular sus ordenamientos tendrá 7 tipos de elementos, donde uno de esos tipos tiene 2 repeticiones, entonces calcular el número de permutaciones de los 8 elementos es:

$$
\frac{8!}{2!}
$$

Notar que para cada letra que estaban repetidas, la M y la A, tenemos esa cantidad de ordenamientos de letras intermedias, por lo que por principio multiplicativo tenemos:

$$
2 \cdot \frac{8!}{2!}
$$

Esto equivale a la cantidad de permutaciones del conjunto del enunciado cuyas palabras empiezan y terminan con la misma letra.
