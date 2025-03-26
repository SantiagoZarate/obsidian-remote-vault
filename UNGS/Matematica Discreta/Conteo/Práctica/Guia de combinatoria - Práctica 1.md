## 1 - Una Tienda Vende 2 Marcas Distintas De Pasta Dentífrica. Cada Una De Estas Marcas Se Vende En Dos Tamaños Distintos De Tubos Y a Su Vez, Cada Uno De Ellos, Con O Sin Flúor. ¿Cuántos Tipos Diferentes De Tubos Se Venden En la Tienda?

- 2 marcas
- 2 Tamaños distintos
- Con o sin flúor
$$2 . 2 . 2 = 2³ = 8$$

La tienda vende 8 tipos diferentes de tubos

---
  
## 2 - Un Negocio De Cubiertas Tiene Cinco Marcas Distintas. Por Cada Marca Ofrece Ocho Tamaños Distintos Y Por Cada Tamaño Distinto Se Puede Elegir Que la Cubierta Sea Diagonal O Radial, a Su Vez Cada Uno De Esos Tipos Se Ofrece Con Cámara O Sin Cámara. ¿Cuántas Cubiertas Diferentes Se Ofrecen En El Negocio?

- 5 Marcas distintas
- 8 Tamaños distintos
- Diagonal o radial
- Con cámara o sin cámara

$$ 5.8.2.2 = 160 $$
Ofrecen 160 cubiertas diferentes

---

## 3 - Se Construyen Señales Izando 5 Banderas En Un Mástil ¿Cuántas Señales Pueden Construirse Si Se Dispone De Una Cantidad Ilimitada De Banderas En 7 Colores Distintos? ¿Qué Implicancia Tiene En la Forma De Contar Que Se Disponga De Una Cantidad Ilimitada De Banderas De Cada Color? ¿Si De Un Determinado Color Solo Hubiesen 5 Banderas Se Podría Contar De Igual Forma? Reflexione Sobre Qué Aspecto Tendría Que Tener En Cuenta

La primer posición en el mástil puede ser tomada por 7 banderas de distinto color, la segunda posición lo mismo, así hasta la quinta posición, por lo que tenemos

$$7⁵ = 16807$$
cantidad de señales que se pueden construir, permitiendo la repetición de colores entre banderas.

El hecho de que tengamos banderas ilimitadas significa que podemos repetir el color de las banderas que se usan para construir la señal.

Si de un determinado color tenemos solo 5 unidades, el conteo permanece igual porque en ningun escenario se necesitan mas de 5 banderas del mismo color.

---

4

---

## 5 - Las Patentes De Los Automóviles En Nuestro País Se Escriben Mediante Tres Letras Seguidas De Tres Números, Como Por Ejemplo SFX 984 - EEY 233. La Letra Ñ no Se Admite En Las Patentes Y Tanto Las Letras Como Los Números Pueden Repetirse. ¿Cuántas Patentes Diferentes Son Posibles?

**Respuesta:**

Sea S el conjunto de patentes posibles, definimos el subconjunto $S_1$ de $S$ cuyos elementos son las primeras 3 letras de la patente, y el subconjunto $S_2$ de S cuyos elementos son los 3 siguientes dígitos.

podemos ver que $S_1$ y $S_2$ es una partición de $S$, por lo que podemos calcular $|S|$ de la siguiente manera:
$$|S| = |S_1| + |S_2|$$
Para calcular los cardinales de $S_1$ tenemos que para la primer posición contamos con 26 posibles candidatos, y que por cada uno de las opciones que escojamos tendremos 26 posibles posibilidades para la segunda y tercera posición, esto es debido a que se permiten tener letras repetidas entre las patentes.

entonces tenemos que:
$$|S_1| = 26³$$
Para calcular el $|S_2|$ podemos hacer un análisis de manera análoga al conjunto anterior, solo que en este caso contamos con 10 posibilidades por posición, esto es así porque tenemos dígitos del 0 al 9, por lo que tenemos que:
$$|S_2| = 10³$$
Ahora que calculamos los cardinales de $|S_1|$ y $|S_2|$ y que para cada una de las tres primeras letras contamos con la posibilidad de asignar cualquier combinación de los siguientes tres números, por el principio de multiplicidad tenemos que:
$$
\begin{aligned}
|S| &= |S_1| \cdot |S_2|\\
|S| &= 26³ \cdot 10³\\
\end{aligned}
$$
---
## 6 - Para Cada Uno De Los Siguientes Items Responda la Pregunta Del Ejercicio Anterior Teniendo En Cuenta la Restricción Dada.

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
$$  
\begin{aligned}
|S_1| &= P(26,3)\\
|S_2| &= P(10,3)\\
|S| &= P(26,3) \cdot P(10,3)
\end{aligned}
$$
---
## 7 - En Una Habitación Hay 7 Puertas. ¿De Cuántas Formas Se Puede Entrar Por Una Puerta Y Salir Por Otra Distinta?

**Respuesta:**

Sea S el conjunto cuyos elementos son las combinaciones de puertas para entrar por una puerta y salir por otra distinta, sea el conjunto P = {$P_1, P_2,... , P_7$} donde cada elemento representa a cada una de las puertas del enunciado, ejemplos de elementos del conjunto S son:
$$
\{P_1, P_2\}, \{P_7, P_2\},\{P_4,P_5\}
$$
Un elemento invalido sería:
$$
\{P_2,P_2\}
$$
Ya que no se puede repetir la misma puerta para entrar y para salir.

Para calcular el ordenamiento en hilera de puertas hago uso de la formula de permutación.
$$P(7,2) 
= \frac{7!}{(7-2)!} 
= \frac{7!}{5!} 
= \frac{7\cdot6\cdot5!}{5!}
= 7\cdot6
$$
Entonces para calcular $|S|$ solo queda por resolver la cuenta $7\cdot6$

---
## 8. ¿Cuántos Números Enteros Entre 10.000 Y 100.000 Existen Tal Que Cada Uno De Sus Dígitos Es Un 6, Un 7 O Un 8? ¿Cuántos Entre 10.000 Y 100.000 Son Tales Que Cada Uno De Sus Dígitos Es Un 6, Un 7, Un 8 O Un 0?

**Respuesta:**

Sea el conjunto S cuyos elementos son los números enteros entre 10.000 y 100.000 y que sus dígitos sean 6, 7 u 8, lo pedido en el ejercicio se obtiene calculando $|S|$, y para ello vamos a hacer el siguiente análisis.

Contamos con 5 posiciones para colocar los números, a pesar de el limite sea 100.000, no nos interesa la sexta posición ya que el menor de los números válidos, en este caso el 6, se excede si lo usamos en la posición de la centena de miles, por lo que queda descartado.

En cada posición tenemos 3 posibles candidatos, 6, 7 u 8, y para cada uno de los números elegidos para esta posición, contamos con la misma cantidad de posibilidades para las posteriores posiciones.

Así que por principio de multiplicidad tenemos que:
$$  
\begin{aligned}
|S| &= 3 \cdot 3 \cdot 3 \cdot 3\\
|S| &= 3⁴
\end{aligned}
$$
Para resolver lo pedido en la siguiente pregunta del enunciado el análisis es bastante parecido al anterior, definimos el conjunto S de la misma manera, solo que ahora los números están formados enteramente por 6, 7, 8 u 0. 

Contamos con las mismas 5 posiciones, pero en este caso la primer posición puede ser ocupada por 3 números, 6,7 u 8, el 0 se descarta porque el limite inferior empieza a partir de 10.000. Las demás posiciones tienen 4 posibles valores.

Sin importar que numero se elige para cada posición esto no condiciona las posibilidades de elección para las siguientes posiciones.

Así que por principio de multiplicidad tenemos que:
$$  
\begin{aligned}
|S| &= 3 \cdot 4 \cdot 4 \cdot 4\\
|S| &= 3 \cdot 4³
\end{aligned}
$$
---
## 9. Los Números En Nuestro Sistema De Numeración Se Construyen Con Los Dígitos 0, 1, . . . , 8 O 9. Considere Aquellos Números Entre 1 Y 10.000 Ambos Inclusive Que Se Forman Utilizando Únicamente Los Dígitos 1, 2 O 3 (no Utilizan Los Dígitos 0, 4, 5, 6, 7, 8, 9). #Multiplicidad #aditivo

- ¿Cuántos de dichos números hay?
- ¿Cuántos de dichos números son impares?
- ¿Cuántos de dichos números son impares y tienen al menos una vez al dígito 2?

> [!NOTE] 
> Este es parecido al anterior pero notar que ahora los numeros pueden tener
> distinta cantidad de digitos.

**Respuesta:**

Sea $S$ el conjunto cuyos elementos son números formados únicamente por los dígitos 1, 2 o 3 entre el rango 1 - 10.000 ambos inclusive, definimos los siguientes subconjuntos de $S$
$$  
\begin{aligned}
S_1 &= \text{Elementos con numeros de 4 digitos} \\
S_2 &= \text{Elementos con numeros de 3 digitos} \\
S_3 &= \text{Elementos con numeros de 2 digitos} \\
S_4 &= \text{Elementos con numeros de 1 digitos} \\
\end{aligned}
$$
Observemos que $S = S_1 \cup S_2 \cup S_3 \cup S_4$ y que $S_i \cap S_j = \emptyset$ con $i \neq j$  Es decir, los subconjuntos $S_1,S_2,S_3$ y  $S_4$ son una partición del conjunto S, por lo tanto $|S| = |S_1| + |S_2| + |S_3| + |S_4|$.

Para contar el cardinal $S_1$ analizamos el numero de 4 dígitos que podemos formar, por cada posición tenemos 3 números candidatos y para cada uno de los números que elijamos las posibilidades a escoger en la siguiente posición es la misma, entonces por principio de multiplicidad se cumple
$$|S| = p . q$$
en este caso $p$ seria la cantidad de elementos candidatos a elegir, y $q$ también, en este caso contamos por 4 espacios disponibles, por los que nos quedaría:
$$|S_1| = 3⁴$$
para hacer el calculo de $|S_2|$, $|S_3|$ y $|S_4|$ podemos usar un razonamiento análogo al conjunto anterior, pero variando los espacios disponibles para poner los números.

el cálculo para cada subconjunto queda de la siguiente manera:
$$  
\begin{aligned}
|S_2| &= 3³\\
|S_3| &= 3²\\
|S_4| &= 3
\end{aligned}
$$
Una vez tenemos el calculo de cada uno de los cardinales de los subconjuntos de $S$ por principio aditivo podemos calcular $|S|$:
$$
|S| = 3⁴ + 3³ + 3² + 3
$$
**Entonces lo pedido en la primer pregunta del enunciado es lo propuesto anteriormente.**

Siguiendo con el enunciado es hora de calcular la cantidad de números pertenecientes al $S$ cuyos elementos sean impares.

Definimos al subconjunto $P$ de $S$ cuyos elementos sean pares, es decir que el dígito que representa las unidades este ocupado por un 2.

Por definición de complemento, definimos $\overline{P}$ como un subconjunto de $S$ cuyos elementos son números impares.

Lo pedido en el enunciado se obtiene calculando el cardinal de $\overline{P}$ y para ello usaremos el principio de sustracción.
$$|\overline{P}| = |S| - |P|$$
El cardinal de $S$ ya lo calculamos en el punto anterior, por lo que queda por calcular $|P|$, sabemos que la ultima posición va a estar siempre ocupada por un 2, y como máximo tendremos números de 4 dígitos ya que el limite es 10.000 pero la posibilidad de tener 5 dígitos queda descartada por que el valor mínimo que cumpla con el requisito para ser parte de $S$ sería 11.111 pero se excede del límite.

Definimos los siguiente subconjuntos de $P$:
$$  
\begin{aligned}
P_1 &= \text{Números de 4 digitos}\\
P_2 &= \text{Números de 3 digitos}\\
P_3 &= \text{Números de 2 digitos}\\
\end{aligned}
$$
No hace falta definir el subconjunto con un solo dígito ya que solo existe un elemento, en este caso el 2 que es par.

Notemos que $P = P_1 \cup P_2 \cup P_3$ y que $P_i \cap P_j = \emptyset$ siempre que $i \neq j$ es decir los subconjuntos $P_1$, $P_2$ y $P_3$ es una partición de $P$, por lo tanto $|P| = |P_1| + |P_2| + |P_3|$

Para calcular los cardinales de los subconjuntos de $P$ sabemos que para todas las posiciones voy a tener 3 posibilidades y la ultima posición va a estar ocupada siempre por un 2, así que para calcular $|P_1|$ tenemos la siguiente cuenta:
$$
\begin{aligned}
|P_1| &= 3 \cdot 3 \cdot 3 \cdot 1 \\
|P_1| &= 3³ \\
\end{aligned}
$$
De la misma manera lo hacemos con los subconjuntos restantes de $P$:
$$  
\begin{aligned}
|P_2| &= 3² \\
|P_3| &= 3
\end{aligned}
$$ 
siguiendo el principio aditivo calculamos $|P|$ de la siguiente manera:
$$
|P| = 3³ + 3² + 3
$$
Una vez tenemos el calculo del cardinal de $P$ podemos calcular el cardinal de $\overline{P}$ de la siguiente manera:
$$  
\begin{aligned}
|\overline{P}| &= |S| - |P| \\
|\overline{P}| &= (3⁴ + 3³ + 3² + 3)  - (3³ + 3² + 3)\\
|\overline{P}| &= 3⁴
\end{aligned}
$$
**Entonces respondiendo la pregunta a cual es la cantidad de numero de $S$ que sean impares es con el siguiente calculo:**
$$
|\overline{P}| = 3⁴
$$

Ahora es momento de responder a la ultima pregunta:

¿Cuántos de dichos números son impares y tienen al menos una vez al dígito 2?

Sigamos teniendo a $S$ como al conjunto cuyos elementos son números formados por 1, 2 o 3 entre 1 y 10.000, sea el subconjunto $M$ de $S$ cuyos elementos esta formado por los números impares, definidos el subconjunto $N$ de $M$ cuyos elementos solo están formados por los números 1 y 3. 

Por definición de complemento tenemos que $\overline{N}$ es el conjunto cuyos elementos tienen al menos una vez el número 2. Resolver el ejercicio implica obtener  $|\overline{N}|$ y para ello usamos el principio de sustracción, es decir:

$$
|\overline{N}| = |M| - |N|
$$
El valor del cardinal de $M$ ya lo tenemos por resolución de puntos anteriores, por los que los cardinales nos quedarían de la siguiente manera.
$$  
\begin{aligned}
|M| &= 3⁴\\
|N| &= ?\\
|\overline{N}| &= ?
\end{aligned}
$$
Voy a calcular el cardinal de $N$, para ello siguiendo un razonamiento análogo a puntos anteriores se que puedo particionar a $N$ en 4 subconjuntos, cada uno formado por elementos con cierta cantidad de digitos, y que cada elemento de estos subconjuntos en cada posición puede tomar dos opciones, el 1 o el 3, por lo que por principio multiplicativo nos queda:

$$
|N| = 2⁴ + 2³ + 2² + 2
$$

**Ahora que tenemos el cardinal de $N$ podemos continuar y calcular el cardinal de $\overline{N}$ que seria el resultado de la siguiente cuenta:**
$$
\begin{aligned}
|\overline{N}| &= 3⁴ - (2⁴ + 2³ + 2² + 2)\\
|\overline{N}| &= 81 - 46\\
|\overline{N}| &= 35\\
\end{aligned}
$$

## 10 - ¿Cuántos Números Enteros Mayores Que 99 Y Menores Que 1000 Se Escriben Utilizando Dígitos Distintos? ¿Cuántos De Estos Números Son Impares?

Sea S el conjunto cuyos elementos sean números enteros mayores a 99 y menores a 1000 que contienen dígitos distintos, lo pedido por el enunciado se resuelve calculando $|S|$, para ello planteamos lo siguiente.

Contamos con 3 posiciones para asignar números, la primer posición cuenta con 9 posibles candidatos (1,2, ... , 9), la segunda posición contaría con 10 dígitos pero como no se permiten dígitos repetidos, el dígito elegido para la primer posición es descartado para la segunda, por lo que nos quedan 9 posibilidades, para la ultima posición y con un razonamiento análogo a los candidatos de la segunda posición, nos queda con 8 posibles candidatos.

Tener en cuenta que para cada uno de los dígitos elegidos por posición vamos a tener la misma cantidad de candidatos para la siguiente posición

**Entonces por principio multiplicativo tenemos lo siguiente:**

$$
|S| = 9 \cdot 9 \cdot 8
$$
Ahora para calcular cuantos de estos números son impares vamos a hacer un analisis parecido an anterior, definamos al conjunto $M$ cuyos elementos son los números impares.

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
Observemos que $M = M_1 \cup M_2 \cup M_3 \cup M_4 \cup M_5$  y que $M_i \cap M_j = \emptyset$ para todo $i \neq j$, por lo que $M_1$,$M_2$,$M_3$,$M_4$  y $M_5$ es una partición de $M$ y que por principio aditivo tenemos
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