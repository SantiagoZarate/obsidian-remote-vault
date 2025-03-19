## Con Los Números 4, 3, 5, 6, 7, 9 Y Suponiendo Que Los Dígitos Se Pueden Repetir

**a)** ¿Cuántos números de tres cifras son capicúas?

**b)** ¿Cuántos números de tres cifras hay tales que son mayores a 486 y sus dígitos son distintos de 6, 3 y 5?

**Respuesta**

### **a)**

Sea el conjunto $S$ cuyos elementos son números de 3 cifras y capicúas con los números 4,3,5,6,7 y 9. Lo pedido en el enunciado se resuelve calculando $|S|$, para ello contamos con el siguiente análisis.

- Para la primer posición tenemos 6 posibles valores que escoger.
- Para la segunda posición, debido a que se pueden repetir los números vamos a tener 6 posibles candidatos también.
- La ultima posición va a estar ocupada por el mismo dígito usado en la primer posición, por lo que no tenemos opción de elegir otro dígito

Notar que para cada uno de los dígitos elegidos para la primer posición tenemos la posibilidad de escoger cualquier número para la segunda posición, entonces por principio multiplicativo tenemos que:

$$
|S| = 6 \cdot 6
$$
### **b)**

Sea el conjunto $M$ cuyos elementos sean números formados con los números 4, 3, 5, 6, 7 y 9 mayores a 486.

Definimos el subconjunto $D$ de $M$ cuyos elementos dígitos solo estén formados por 6, 3 y 5 sin repetirse, por definición de complemento tenemos $\overline{D}$ el conjunto cuyos elementos son mayores a 486 y están formados por dígitos distintos de 6, 3 y 5. Lo pedido en el enunciado se resuelve obteniendo $|\overline{D}|$ y por principio de sustracción es:

$$
|\overline{D}| = |M| - |D|
$$

Primero calculamos $|M|$, para ello definimos los siguientes subconjunto de $M$:

$$  
\begin{aligned}
M_1 &= \text{Elementos con la posición de la centena ocupada por el 4}\\
M_2 &= \text{Elementos mayores a 499}
\end{aligned}
$$

Notemos que $M = M_1 \cup M_2$ y que $M_1 \cap M_2 = \emptyset$, por lo tanto $M_1$ y $M_2$ es una partición de $M$, por lo que $|M| = |M_1| + |M_2|$, tenemos que calcular el cardinal de $M_1$ y $M_2$

$M_1$ esta formado por = {493, 496, 494, 495, 496, 497, 499}, así que $|M_1| = 7$

para calcular $|M_2|$ hagamos el siguiente análisis:

- Para la primer posición que representan las centenas tenemos 4 posibles candidatos, el número 4 y 3 quedan descartados porque harían que el elemento no cumpla el requisito de ser mayor a 499
- Para la segunda y tercera posición tenemos todos los números disponibles.

entonces por principio multiplicativo tenemos que:

$$  
\begin{aligned}
M_2 &= 4 \cdot 6 \cdot 6\\
M_2 &= 144
\end{aligned}
$$ 

Una vez calculamos el cardinal de $M_1$ y $M_2$ podemos calcular $|M|$:

$$  
\begin{aligned}
|M| &= |M_1| + |M_2|\\
|M| &= 7 + 144\\
|M| &= 151
\end{aligned}
$$

Ahora nos queda por calcular $|D|$, que sería la cantidad de números mayores a 486 formados por 6, 3 y 5.

- La primer posición, que representa las centenas, va a poder ser ocupada por dos números, el 6 y 5.
- La posición de las decenas originalmente podría haber sido ocupada por los 3 números pero hay que descartar el número que fue elegido en la primer posición, por lo que nos queda 2 candidatos.
- La ultima posición va a poder ser ocupada por el dígito restante, el que no fue elegido ni en la primer ni segunda posición.

entonces por principio multiplicativo tenemos que:

$$

|D| = 2 \cdot 2 \cdot 1

$$

Ahora que ya tenemos el cardinal de $M$ y $D$, podemos seguir en nuestra búsqueda de $|\overline{D}|$, que por principio de sustracción es:

$$  

\begin{aligned}

|\overline{D}| &= |M| - |D|\\

|\overline{D}| &= 151 - 4\\

|\overline{D}| &= 147

\end{aligned}

$$

Entonces la cantidad de números de tres cifras que sean mayores a 486 y que sus dígitos no sean 6, 3 y 5 es 147.
