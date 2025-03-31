**a)** ¿Cuántas permutaciones hay de todas las letras de la palabra ESTRIDENTE?

**b)** ¿Cuántas permutaciones hay de todas las letras de la palabra ESTRIDENTE que comienzan y terminan con la letra E?

**c)** ¿Cuántas permutaciones hay de todas las letras de la palabra ESTRIDENTE que no comienzan con la letra D?

**d)** ¿Cuántas permutaciones hay de todas las letras de la palabra ESTRIDENTE que tengan todas las consonantes juntas?

**Respuesta**

## **A)**

Observar que la palabra dada tiene algunas letras repetidas, y que si definimos el multiconjunto con las letras de esa palabra nos queda lo siguiente:

$$
\{ 3 \cdot E, 1 \cdot S, 2 \cdot T, 1 \cdot R, 1 \cdot I, 1 \cdot D, 1 \cdot N \}
$$

La cantidad de permutaciones 10 elementos de ese conjunto, con el tipo de elemento E con 3 repeticiones, y el tipo de elemento T con 2 repeticiones es:

$$
\frac{10!}{3! \cdot 2!} = \frac{3628800}{12} = 302400
$$

Eso equivale a las permutaciones de las letras de la palabra dada.

## **B)**

Si tenemos la restricción que la palabra empieze y termine con la E, podemos definir el siguiente multiconjunto:

$$
\{ 1 \cdot E, 1 \cdot S, 2 \cdot T, 1 \cdot R, 1 \cdot I, 1 \cdot D, 1 \cdot N \}
$$

La cantidad de permutaciones 8 elementos de ese conjunto, con el tipo de elemento T con 2 repeticiones es:

$$
\frac{8!}{2!}
$$

Eso equivale a las permutaciones de las letras de la palabra dada con las restricciones del enunciado.

## **C)**

Definimos el conjunto $P$ cuyos elementos son las permutaciones de las letras de la palabra ESTRIDENTE, definimos $S \subset P$ el conjunto cuyos elementos empiezan con la letra D, por definición de conjunto tenemos $\overline{S}$ cuyos elementos no empiezan con la letra D, lo pedido en el enunciado se resuelve obteniendo $|\overline{S}|$, por principio de sustracción sabemos que es:

$$
|\overline{S}| = |P| - |S|
$$

Ahora calculemos los cardinales de $P$ y $S$

- $|P|$:
Esto ya lo obtuvimos cuando resolvimos el punto **a)**, que es 302400

- $|S|$
Ahora debemos contar la cantidad de ordenamientos de la palabra donde empieze con la letra D, para eso fijamos la letra D en la primera de las 10 posiciones y definimos el siguiente multiconjunto:

$$
\{ 3 \cdot E, 1 \cdot S, 2 \cdot T, 1 \cdot R, 1 \cdot I, 1 \cdot N \}
$$

La cantidad de permutaciones 9 elementos de ese conjunto, con el tipo de elemento E con 3 repeticiones, y el tipo de elemento T con 2 repeticiones es:

$$
\frac{9!}{3!\cdot2!} = \frac{362880}{12} = 30240
$$

Esas son la cantidad de palabras que empiezan con la letra D

Ahora podemos seguir en la búsqueda de $|\overline{S}|$

$$  
\begin{aligned}
|\overline{S}| &= |P| - |S|\\
|\overline{S}| &= 302400 - 30240\\
|\overline{S}| &= 272160\\
\end{aligned}
$$

Esto equivale a la cantidad de permutaciones donde la palabra no empieza con la letra D

### **D)**

==TODO==
