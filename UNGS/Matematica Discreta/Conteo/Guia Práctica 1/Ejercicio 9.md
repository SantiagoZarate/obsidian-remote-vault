## Los Números En Nuestro Sistema De Numeración Se Construyen Con Los Dígitos 0, 1, . . . , 8 O 9. Considere Aquellos Números Entre 1 Y 10.000 Ambos Inclusive Que Se Forman Utilizando Únicamente Los Dígitos 1, 2 O 3 (no Utilizan Los Dígitos 0, 4, 5, 6, 7, 8, 9). #Multiplicidad #aditivo

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