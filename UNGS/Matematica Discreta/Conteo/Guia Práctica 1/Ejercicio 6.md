## Para Cada Uno De Los Siguientes Items Responda la Pregunta Del Ejercicio Anterior Teniendo En Cuenta la Restricción Dada.

a) Las letras no pueden repetirse.
b) Los números no pueden repetirse.
c) Las letras y los números no pueden repetirse.
d) La última de las letras es una Q.
e) La primera de las letras es una A.
f ) La última de las letras es una vocal.
g) La primera de las letras es una vocal.

Respuesta:

**a)** - Teniendo en cuenta que las letras no puede repetirse, el calculo para obtener $|S_1|$ va a ser diferente, para la primer posición voy a seguir contando con 26 posibilidades, pero para la siguiente voy a contar con 25, debido a que no se admiten valores repetidos, y 24 para la tercera posición.

entonces la cuenta que nos queda es la siguiente:

$$|S_1| = 26 \cdot 25 \cdot 24$$
Una vez sabemos el valor del cardinal de $S_1$, el conjunto $S_2$ permanece intacto, por principio multiplicativo tenemos que:
$$
\begin{aligned}
|S| &= |S_1| \cdot |S_2|\\
|S| &= 26 \cdot 25 \cdot 24 \cdot 10³\\
\end{aligned}
$$
**b)** - En esta oportunidad cambia la manera de calcular $|S_2|$, con la nueva restricción que nos impide tener números repetidos para la primer posición de los números tenemos 10 posibilidades, 9 para la segunda y 8 para la tercera, nos queda la siguiente cuenta:
$$|S_2| = 10 \cdot 9 \cdot 8$$
Una vez tenemos el cardinal de $|S_2|$ resta hacer el calculo para obtener $|S|$, que es el siguiente:
$$
\begin{aligned}
|S| &= |S_1| \cdot |S_2|\\
|S| &= 26³ \cdot 10 \cdot 9 \cdot 8\\
\end{aligned}
$$
Usando permutaciones, podemos calcular la cantidad de ordenamientos en hilera de elementos únicos.

Recordar la formula de $P(n,r)$:
$$  
\begin{aligned}
P(n,r) = \frac{n!}{(n-r)!}
\end{aligned}
$$
En nuestro caso quedaría de la siguiente manera:

$$
\begin{aligned}
&P(10,3)
= \frac{10!}{(10-3)!}
= \frac{10!}{7!}
= \frac{10\cdot9\cdot8\cdot7!}{7!}
= 10 \cdot 9 \cdot 8
\end{aligned}
$$

**C)** Teniendo en cuenta que los números y letras no puede repetirse podemos usar los cálculos de puntos anteriores, y al calcular el cardinal de $S$ usando la multiplicidad, ya que sin importar que ordenamiento obtengamos de las letras vamos a tener la oportunidad de usar cualquier ordenamiento de números.

***Nota para mi***
**Aclarar el uso de la función de permutaciones.**