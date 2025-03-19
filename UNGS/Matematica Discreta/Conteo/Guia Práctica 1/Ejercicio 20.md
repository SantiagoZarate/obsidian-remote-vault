## ¿De Cuántas Formas Pueden Sentarse 10 Personas En Fila Si Hay Dos Personas Determinadas Que no Pueden Sentarse En Asientos Contiguos?

**Respuesta**

Definimos el conjunto $P$ = {$P_1$, $P_2$, ..., $P_{10}$} cuyos elementos representan las personas, sea $S$ el conjunto cuyos elementos son las formas en que se pueden sentar las 10 personas en fila, contar los ordenamientos en fila de las 10 personas es igual $10!$.

Sea el subconjunto $M$ de $S$ cuyos elementos tienen a $P_1$ y $P_2$ sentados en asientos contiguos, por definición de complemento tenemos $\overline{M}$ que serían los elementos con $P_1$ y $P_2$ separados, por definición $M$ y $\overline{M}$ es una partición de $S$.

Lo pedido en el enunciado se resuelve obteniendo $\overline{M}$, por principio de sustracción es:

$$
|\overline{M}| = |S| - |M|
$$

Sabemos que $|S| = 10!$, por lo que nos queda por obtener $|M|$

- Para las primeras dos posiciones tenemos a $P_1$ y $P_2$ y los podemos ordenar de dos maneras, primero $P_1$ y después $P_2$ o viceversa
- Para los restantes asientos tenemos 8 personas, y tenemos que contar la cantidad de ordenamientos entre estas 8 personas, lo que es igual a $8!$

Notar que en el ejemplo ubicamos $P_1$ y $P_2$ en las primeras posiciones, pero contamos con 9 posiciones en donde ubicarlos, las posiciones a la izquierda de cada una de las 8 personas restantes, y la posición a la derecha del todo.

Observar que para cada ordenamiento de las dos personas contiguas tenemos $8!$ ordenamientos de las restantes personas e independientemente de los ordenamientos de cada uno, podemos ubicar a las dos personas en 9 lugares distintos, así que por principio multiplicativo tenemos que:

$$
|M| = 2 \cdot 8! \cdot 9
$$

Ahora podemos seguir en la búsqueda de $|\overline{M}|$, que es el resultado del siguiente cálculo:

$$  
\begin{aligned}
|\overline{M}| &= |S| - |M|\\
|\overline{M}| &= 10! - (2\cdot8!\cdot9)\\
\end{aligned}
$$

Esa seria la cantidad de formas de sentar 10 personas en fila teniendo en cuenta lo pedido en el enunciado.
