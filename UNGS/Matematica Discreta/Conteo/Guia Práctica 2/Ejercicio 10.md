---
status: Incomplete
---

## Considere El Conjunto S Formado Por Los Ordenamientos En Circulo De Todas Las Letras De la Palabra MANTENIMIENTO

**a)** ¿Cuántos elementos tiene S?

**b)** ¿Cuántos de estos ordenamientos tienen la secuencia de letras MIENTO?.

**c)** ¿Cuántos de estos ordenamientos no tienen dos o más vocales juntas?

**Respuesta**

### **a)**

Notar que con las letras de la palabra dada podemos definir el multinconjunto $G$ =

$$
\{ 2 \cdot M, 1 \cdot A, 3 \cdot N, 2 \cdot T, 2 \cdot E , 2 \cdot I, 1 \cdot O \}
$$

Entonces para poder contar los elementos de $S$, que sería contar los ordenamientos en ronda con elementos repetidos, podemos tomar al tipo de elemento "A" y ubicar a las demás letras en posiciones relativas a "A", por ej: la primer letra a la izquierda de "A".

Contar las permutaciones de $G$, teniendo en cuenta que tiene 7 tipos de elementos, con el tipo de elemento "N" con 3 repeticiones, y los tipos M, T, E e I con 2 repeticiones, las permutaciones de 13 elementos de $G$ es:

$$
\frac{13!}{3!\cdot2!\cdot2!\cdot2!\cdot2!}
$$

Eso equivale a la cantidad de ordenamientos en hilera de $G$, pero en el enunciado se nos pide que estén en ronda, por lo que por cada 13 ordenamientos en hilera, tenemos un ordenamiento circular único, entonces la cantidad de elementos de $S$ es:

$$
\frac{1}{13} \cdot
\frac{12!}{3!\cdot2!\cdot2!\cdot2!\cdot2!}
$$
### **b)**

En este caso se nos pide contar la cantidad de elementos de $S$ que tengan la secuencia de letras MIENTO, por lo que de nuestro multiconjunto de letras $G$ del punto anterior podemos restarles esta secuencia y añadirla como un nuevo tipo de elemento, por lo que definimos el multiconjunto $P$:

$$
\{ 1 \cdot M, 1 \cdot A, 2 \cdot N, 1 \cdot T, 1 \cdot E, 1 \cdot I, 1 \cdot MIENTO \}
$$

Ahora, la cantidad de permutaciones de 8 elementos de $P$, teniendo en cuenta que quiero contar los ordenamientos en circulo con elementos repetidos y fijando al elemento MIENTO es:

$$
\frac{7!}{2!}
$$

Esto equivale a la cantidad de elementos de $S$ con la secuencia MIENTO.

Por cada uno de estos ordenamientos podemos armar una ronda con estas 7 letras, notemos que entre cada letra nos quedan 7 espacios, que van a ser donde se puede ubicar la secuencia MIENTO.

### **c)**

 - Buscar la que no tienen vocales juntas

Definimos $K \subset S$ cuyos elementos tienen dos o más vocales juntas, por definición de complemento tenemos $\overline{K}$ cuyos elementos no tienen vocales juntas, lo pedido en el enunciado se resuelve obteniendo $|\overline{K}|$ que por principio de sustracción es:

$$
|\overline{K}| = |S| - |K|
$$

Ya tenemos el cardinal de $S$ por resolución de puntos anteriores, así que calculemos $|K|$, lo que seria igual a contar los ordenamientos en donde no tengamos vocales juntas.

Notar que la palabra está constituida por 7 consonantes y 6 vocales

definimos el siguiente multiconjunto con las consonantes:

$$
\{ 2 \cdot M, 3 \cdot N, 2 \cdot T \}
$$

definimos el siguiente multiconjunto con las vocales:

$$
\{ 1 \cdot A, 2 \cdot E, 2 \cdot I  ,1 \cdot O \}
$$

Para contar las permutaciones, fijamos la letra A en el primer lugar y contamos los ordenamientos de 5 elementos, con E e I con 2 repeticiones, lo que es igual a :

$$
\frac{5!}{2!\cdot2!}
$$

Esa es la cantidad de ordenamientos circulares de las 6 vocales, notar que tenemos

==TODO==
