---
tags:
  - Adición
  - Multiplicidad
status: Done
---

## ¿Cuántos Números Enteros Mayores Que 99 Y Menores Que 1000 Se Escriben Utilizando Dígitos Distintos? ¿Cuántos De Estos Números Son Impares? #aditivo #Multiplicidad

**Respuesta:**

Sea $S$ el conjunto cuyos elementos sean números enteros mayores a 99 y menores a 1000 que contienen dígitos distintos, lo pedido por el enunciado se resuelve calculando $|S|$, para ello planteamos lo siguiente.

Contamos con 3 posiciones para asignar números, la primer posición cuenta con 9 posibles candidatos (1,2, ... , 9), la segunda posición contaría con 10 dígitos pero como no se permiten dígitos repetidos, el dígito elegido para la primer posición es descartado para la segunda, por lo que nos quedan 9 posibilidades, para la ultima posición y con un razonamiento análogo a los candidatos de la segunda posición, nos queda con 8 posibles candidatos.

Tener en cuenta que para cada uno de los dígitos elegidos por posición vamos a tener la misma cantidad de candidatos para la siguiente posición

**Entonces por principio multiplicativo tenemos lo siguiente:**

$$
|S| = 9 \cdot 9 \cdot 8
$$

Ahora para calcular cuantos de estos números son impares vamos a hacer un análisis parecido an anterior, definamos al conjunto $M$ cuyos elementos son los números impares.

- Para la primer posición contamos con 9 posibilidades, del 1 al 9
- Para la segunda posición contamos originalmente con 10 posibilidades, del 0 al 9, pero como se admiten repetidos contamos con 9, porque se descarta la opción elegida en la primer posición.
- Para la tercer opción originalmente contaríamos con 5 posibilidades, el 1, 3, 5, 7 o 9, ya que son los números impares, pero hay que tener en cuenta que al no admitir repetidos nos quedan 3 posibilidades, debido a que descartamos los números de la primer y segunda posición

entonces por principio de multiplicidad tenemos que:

$$
|M| = 9 \cdot 9 \cdot 3
$$
*Usando otro acercamiento.*
Sea el subconjunto $M$ de $S$ el conjunto cuyos elementos son impares, definamos los siguiente conjuntos:
$$  
\begin{aligned}
M_1 &= \text{Números que terminan con el dígito 1}\\
M_2 &= \text{Números que terminan con el dígito 3}\\
M_3 &= \text{Números que terminan con el dígito 5}\\
M_4 &= \text{Números que terminan con el dígito 7}\\
M_5 &= \text{Números que terminan con el dígito 9}\\
\end{aligned}
$$

Observemos que $M = M_1 \cup M_2 \cup M_3 \cup M_4 \cup M_5$ y que $M_i \cap M_j = \emptyset$ para todo $i \neq j$, por lo que $M_1$,$M_2$,$M_3$,$M_4$ y $M_5$ es una partición de $M$ y que por principio aditivo tenemos

$$
|M| = |M_1| + |M_2| + |M_3| + |M_4| + |M_5|
$$

para calcular $|M_1|$ hacemos el siguiente análisis.

- La ultima posición va a estar siempre ocupada por el dígito 1, esto hay que tenerlo en cuenta porque este número no se va a poder repetir en las demás posiciones
- La primer posición originalmente tendría 9 posibles candidatos, del 1 al 9, pero el número 1 queda descartado, así que contamos con 8 posibilidades.
- La segunda posición originalmente tendría 10 posibles candidatos, del 0 al 9, pero descartamos el número 1 de la ultima posición y también descartamos el número de la segunda posición, por los que nos quedan 8 posibles candidatos.

Entonces por principio multiplicativo tenemos el siguiente calculo.

$$
|M_1| = 8 \cdot 8 \cdot 1
$$

La cuenta es la misma para todos los subconjuntos de $M$ ya definidos, por lo que el calculo de $|M|$ nos queda de la siguiente manera:

$$
|M| = 8\cdot8 \cdot 5
$$

Entonces la respuesta al cual es la cantidad de números impares del conjunto $S$ es $8\cdot8\cdot5$
