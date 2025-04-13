---
tags:
  - Permutación-Repetidos
  - Multiplicidad
status: Done
---

## En la Grilla De la Figura Es Posible Siempre Moverse O Bien Una Casilla Hacia la Derecha O Bien Una Casilla Hacia Arriba

**a)** ¿De cuántas maneras podemos ir de la casilla A a la casilla B?

**b)** ¿De cuántas maneras podemos ir de la casilla A a la casilla B pasando por X?

**Respuesta**

### **a)**

Observemos que para ir desde la casilla A a la B tenemos que hacer 4 movimientos hacia arriba y 6 hacia la derecha, pero también hay que tener en cuenta las combinaciones que podemos hacer entre estos movimientos.

Representemos a los movimientos de la siguiente manera:

$$  
\begin{aligned}
X &= \text{Movimiento hacia la derecha}\\
Y &= \text{Movimiento hacia arriba}\\
\end{aligned}
$$

Entonces con esta representación, la siguiente palabra representaría una de las formas de satisfacer lo pedido en el enunciado.

$$
\underline{XXXXXX}\,\underline{YYYY}
$$

Definamos el siguiente multiconjunto:

$$
\{ 6 \cdot X, 4 \cdot Y \}
$$

Ahora la cantidad de permutaciones de 10 elementos con 6 repeticiones para el tipo de elemento X y 4 repeticiones para el tipo de elemento Y es igual a:

$$
\frac{10!}{6!\cdot4!}
$$

Esto equivale a la cantidad de formas de ir desde la celda A, hasta la celda B.

### **b)**

Podemos dividir el problema en dos, la primer parte vamos a calcular la cantidad de formas de ir desde la casilla A hasta la casilla X, y luego calcular la cantidad de formas de ir desde X hasta B. Para cada una de las formas de ir de A hacia X, vamos a contar con todas las formas de ir de X hacia B, por lo que por principio multiplicativo el resultado final tiene esta expresión:

$$
\text{Formas de ir de A hacia X} \cdot \text{Formas de ir de X hacia B}
$$

Para la primer parte, sabemos que tenemos X esta a 2 casillas arriba y 2 casillas a la derecha de A, representamos los movimientos de la siguiente manera.

$$  
\begin{aligned}
x_1 &= \text{Movimiento hacia la derecha}\\
y_1 &= \text{Movimiento hacia arriba}\\
\end{aligned}
$$

la siguiente palabra representaría una forma de ir desde A hacia X:

$$
\underline{x_1x_1}\,\underline{y_1y_1}
$$

definamos el siguiente multiconjunto:

$$
\{ 2 \cdot x_1, 2 \cdot y_1  \}
$$

la cantidad de permutaciones de ese multiconjunto con 4 elementos, donde cada tipo de elemento se repite dos veces es:

$$
\frac{4!}{2!\cdot2!}
$$

Ahora para calcular la segunda parte, sabemos que B esta a 4 movimientos a la derecha y 2 hacia arriba de X, representemos los movimientos de la siguiente manera:

$$  
\begin{aligned}
x_2 &= \text{movimiento hacia la derecha}\\
y_2 &= \text{movimiento hacia arriba}\\
\end{aligned}
$$

Definamos el siguiente multiconjunto:

$$
\{ 4 \cdot x_2, 2 \cdot y_2\}
$$

la cantidad de permutaciones de ese multiconjunto con 6 elementos donde el tipo de elemento $x_2$ tiene 4 repeticiones y el tipo de elemento $y_2$ tiene 2 repeticiones es:

$$
\frac{6!}{4!\cdot2!}
$$

Luego reemplazando los valores en la expresión propuesta al inicio de la resolución tenemos que:

$$
\frac{4!}{2!\cdot2!} \cdot \frac{6!}{4!\cdot2!}
$$

Esto equivale a la cantidad de formas de ir de A hacia B pasando por X
