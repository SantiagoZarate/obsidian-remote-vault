## 2. Sea X El Conjunto Formado Por Las Permutaciones De Todas Las Letras De la Palabra TABLOIDES

**a)** ¿Cuántos elementos de X comienzan con vocal y no terminan en consonante?
**b)** ¿Cuántos elementos de X no tienen dos vocales consecutivas?
**c)** ¿Cuántos elementos de X tienen a las letras A y B juntas, pero no tienen juntas a las letras D y E ?

**Respuesta**

### **a)**

Sea S el subconjunto de X cuyos elementos comienzan con vocal y no terminan consonante, lo pedido en el enunciado se resuelve calculando $|S|$, para ello hagamos el siguiente análisis.

- Para la primer posición tenemos 4 posibles candidatos A, O, I y E
- Para la ultima posición tenemos 3 posibles candidatos, se descarta la seleccionada en la primer posición.
- Para las letras del medio tenemos 5 consonantes, y 2 vocales restantes, es decir 7 letras

Para obtener las permutaciones de las letras del medio necesitamos calcular el ordenamiento en hilera de 7 letras, eso es igual a $P(7,7)$

Ahora para cada una de las letras seleccionadas en la primer posición contamos con $P(7,7)$ letras intermedias y 3 variantes de vocales para la ultima posición, así que por principio multiplicativo calculamos $|S|$:

$$
|S| = 4 \cdot P(7,7) \cdot 3
$$
### **b)**

Sea el subconjunto $V$ de $S$ cuyos elementos tienen dos vocales consecutivas. Por definición de conjunto tenemos que $\overline{V}$ es conjunto cuyos elementos satisfacen que no tienen dos vocales consecutivas. Lo pedido en el enunciado se resuelve calculando $|\overline{V}|$ y para ello, por principio de sustracción es:

$$
|\overline{V}| = |X| - |V|
$$

Para obtener el cardinal de $X$ tenemos que calcular los ordenamientos de todas las letras que forman la palabra TABLOIDES, es decir P(9,9).

Ahora pasemos a calcular $|V|$.

Sabiendo que los elementos de $A$ satisfacen la condición de tener dos vocales consecutivas definimos las posibilidades que tiene cada letra de ocupar un espacio.

Notemos que la palabra TABLOIDES tiene 9 letras sin repetirse entre ellas, de las cuales 4 son vocales y 5 consonantes.

Damos un ejemplo de como pueden posicionarse las letras:

- Las primeras dos posiciones van a estar ocupadas por 2 vocales, tenemos que contar los ordenamientos de 4 vocales tomadas de a 2, es decir P(4,2)
- Las restantes letras, las 5 consonantes y las dos vocales que no fueron seleccionadas para las primeras posiciones, pueden ser ordenadas de P(7,7) formas.

Notar que en el ejemplo dado estamos ubicando las dos vocales consecutivas en la primer posición, pero podrían haber sido ubicadas al final, o en cualquier parte de la palabra, entre las letras restantes, que son 7, tenemos 8 espacios posibles para ubicar las dos consonantes consecutivas, un espacio a la izquierda de cada letras y un espacio a la derecha del todo.

Entonces, para cada una de las combinaciones de las dos letras vocales consecutivas, es decir $P(4,2)$, vamos a tener $P(7, 7)$ ordenamientos de las restantes letras y podemos ubicar las vocales consecutivas en 8 espacios diferentes, entonces por principio de multiplicidad tenemos que:

$$
|V| = P(4,2) \cdot P(7,7) \cdot 8
$$

Ahora que ya tenemos el resultado de $|V|$, podemos obtener $|\overline{V}|$

$$  
\begin{aligned}
|\overline{V}| &= |U| - |V|\\
|\overline{V}| &= P(9,9) - (P(4,2) \cdot P(7,7) \cdot 8)
\end{aligned}
$$

Entonces esa es la cantidad de elementos de $X$ que satisfacen la condición de no tener dos vocales consecutivas.

### **c)**

Definimos a $H$ el subconjunto de $X$ cuyas palabras tienen las letras A y B juntas.

También definimos el subconjunto $L$ de $H$ cuyos elementos satisfacen que las letras D y E están juntas, por definición de complemento tenemos que $\overline{L}$ es el conjunto cuyos elementos tienen palabras con las letras D y E separadas, lo pedido en el enunciado se resuelve obteniendo $|\overline{L}|$ que por principio de sustracción es

$$
|\overline{L}| = |H| - |L|
$$

Empecemos calculando $|H|$. Notemos que lo pedido es algo parecido a la que analizamos en el punto **B)**, así que podemos tomar el mismo razonamiento pero esta vez en de tener en cuenta los ordenamientos de 4 vocales tomados de a 2, necesitamos contar los ordenamientos de 2 letras, A y B, es decir $P(2,2)$

Entonces, el calculo de $|H|$ con la nueva restricción queda de la siguiente manera

$$
|H| = P(2,2) \cdot P(7,7) \cdot 8
$$

Nos queda por calcular $|L|$ que es la cantidad de ordenamientos de las palabras con A y B juntas a la misma vez que tienen D y E juntas.

Lo que estamos buscando es parecido a lo que planteamos para hallar $|H|$, tenemos que contar los ordenamientos de D y E, luego los ordenamientos de las letras restantes y por ultimo saber en cuantos espacios podemos ubicar el par D y E juntos.

- Los ordenamientos para D y E es $P(2,2)$
- Las letras restantes originalmente serían 7, pero en esta ocasión sabemos que tenemos las letras A y B juntas, por lo que no las podemos contar por separadas, así que tenemos 6 elementos para ordenar, eso es igual a $P(6,6)$
- Los espacios disponibles son 7, los espacios a la izquierda de cada uno de los 6 elementos más el espacio a la derecha al final del todo.

Entonces el calculo para obtener $|L|$ es:

$$
|L| = P(2,2) \cdot P(6,6) \cdot 7
$$

Ahora podemos continuar en la búsqueda de $|\overline{L}|$ que por principio de sustracción es:

$$  
\begin{aligned}
|\overline{L}| &= |H| - |L|\\
|\overline{L}| &= (P(2,2) \cdot P(7,7) \cdot 8) - (P(2,2) \cdot P(6,6) \cdot 7)\\
|\overline{L}| &= (2! \cdot 7! \cdot 8) - (2! \cdot 6! \cdot 7)\\
|\overline{L}| &= 70560
\end{aligned}
$$

Entonces 70560 es la cantidad de elementos de $X$ que satisfacen que A y B están juntas mientras que D y E están separadas al mismo tiempo.
