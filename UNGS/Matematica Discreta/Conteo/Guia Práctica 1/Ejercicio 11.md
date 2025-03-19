---
tags:
  - Multiplicidad
  - Permutación
  - Sustacción
---
## Consideremos Los Reordenamientos De Las Letras De la Palabra ARTÍCULOS.

**a)** ¿Cuántos reordenamientos hay en total?
**b)** ¿Cuántos comienzan con vocal?
**c)** ¿Cuántos no comienzan con vocal?
**d)** ¿Cuántos terminan en vocal?
**e)** ¿Cuántos comienzan con dos vocales y terminan en dos consonantes?

**Respuesta**

Sea el conjunto S cuyos elementos sean todas las palabras con las letras de la palabra ARTÍCULOS, lo pedido por el punto **a)** se resuelve calculando $|S|$, por que tenemos que contar la cantidad de ordenamientos en hilera con las letras de la palabra ARTÍCULOS, notar que no tenemos letras repetidas en la palabra, por lo que podemos usar la función de permutación.
$$
|S| = P(n,r)
$$
En nuestro caso la cantidad de letras es 9, y la cantidad de elementos a ordenar es 9, entonces tenemos lo siguiente:
$$
P(9,9) = \frac{9!}{(9 - 9)!} = 9!
$$
Entonces, la cantidad de reordenamientos en total es de $9!$

Definimos al subconjunto $T$ de $S$ cuyas palabras comienzan con vocal, Para calcular lo pedido en el punto **b)** necesitamos hallar $|T|$, para ello vamos a contar los ordenamientos de las 8 letras después de la primer posición, que queda descartada porque va a estar ocupada por una vocal.

Para cada una de las vocales que ocupen la primer posición contamos con $P(8,8)$ formas de ordenas las siguientes letras.

Finalmente por principio multiplicativo la cantidad de palabras que empiezan con vocal es:
$$
\begin{aligned}
|T| &= \text{cantidad de vocales} \cdot P(8,8) \\
|T| &= 4 \cdot P(8,8) \\
\end{aligned}
$$
Lo que se nos pide en el punto **c)** es $|\overline{T}|$, es decir la cantidad de elementos de $S$ cuyas palabras ==no empiezan con vocal==.

Ya hemos realizado el calculo de $|S|$ y $|T|$ en puntos anteriores, así que por principio de sustracción podemos hacer el siguiente calculo:
$$  
\begin{aligned}
|\overline{T}| &= |S| - |T|\\
|\overline{T}| &= 9! - (4\cdot P(8,8))
\end{aligned}
$$
Calcular lo pedido en la consigna **d)** seria hacer una análisis similar al hecho para resolver el punto **b)**, solo que en este caso la última posición esta ocupada por una vocal,  por lo que podemos definir el subconjunto $U$ de $S$ cuyos elementos terminan con vocal, el calculo permanece igual al propuesto en el punto **b)**

Lo pedido en el enunciado se resuelve calculando $|U|$ es decir la siguiente cuenta:
$$|U| = P(8,8) \cdot 4$$
Sea el subconjunto $V$ de $S$ cuyos elementos empiezan dos vocales y terminan con dos consonantes, resolver el item **e)** sería obtener $|V|$.

sean los conjuntos $Vocal$ = {A, I, U, O} y $Consonante$ = {R, T, C, L, S}

Quiero contar los ordenamientos secuenciales de 2 elementos del $Vocal$, por permutación se define como $P(4,2)$

De la misma manera con $Consonante$, por permutación es igual a $P(5,2)$

De esa manera tenemos las cantidades de ordenamiento para las primeras dos letras vocales y las ultimas dos letras consonantes al final, resta por calcular los ordenamientos que quedan en el medio de la palabra.

Sabemos que de los 4 elementos de $Vocal$ se descartan 2 por que están siendo usados para las primeras dos posiciones, de $Consonante$ nos quedan 3 elementos disponibles, ahora calculamos los ordenamientos secuenciales entre las 2 vocales restantes y las 3 consonantes restantes, por permutación es igual a $P(5,5)$.

Notar que por cada una de los ordenamientos de las primeras dos letras, se corresponden $P(5,5)$ ordenamientos de letras intermedias y a su vez $P(5,2)$ ultimas dos letras consonantes.

Finalmente por principio multiplicativo $|V|$ es:
$$
|V| = P(4,2) \cdot P(5,5) \cdot P(5,2)
$$
