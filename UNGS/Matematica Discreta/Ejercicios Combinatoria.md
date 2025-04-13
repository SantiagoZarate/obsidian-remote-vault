## Entregable 5

## **a)** ¿De Cuántas Formas Se Puede Dar Una Mano De Poker (una Mano Consta De 5 cartas) De Modo Que Contenga Al Menos Una Carta De Cada Palo?

Aclaración: Para Que Haya Al Menos Una Carta De Cada Palo, Por Ejemplo, Lo Que no Puede Ocurrir Es Que En Una Mano no Haya Ninguna Carta De Trébol

## **b)** Si Consideramos 685465 Manos De Poker De Modo Que Contengan Al Menos Una Carta De Cada Palo. ¿Pueden Ser Las 685465 Todas Distintas?

**Respuesta**

## **a)**

Observar que un mazo de cartas estándar de poker tiene 52 cartas, distribuidas en 4 palos (trébol, corazón, diamante y picas ) con 13 cartas por palo

Para contar la cantidad de manos que se pueden formar teniendo en cuenta que haya al menos una carta de palo propongamos el siguiente escenario:

Si agarramos una carta de cada palo nos faltaría escoger una carta más para completar la mano, en este caso vamos a tomar dos del palo trébol, entonces la cantidad de formas de seleccionar 2 cartas del palo trébol entre 13 posibles es $C(13,2)$, por cada uno de estos seleccionamientos tenemos que seleccionar una carta entre trece posible para los demás palos, por principio de multiplicidad tenemos que:

$$
\begin{pmatrix} 13 \\ 2 \end{pmatrix} \cdot
\begin{pmatrix} 13 \\ 1 \end{pmatrix} \cdot
\begin{pmatrix} 13 \\ 1 \end{pmatrix} \cdot
\begin{pmatrix} 13 \\ 1 \end{pmatrix} = 171366
$$

Esto equivale a la cantidad de formas de armar una mano donde tenemos dos cartas del palo trébol.

Aún nos falta calcular la cantidad de formas de armar una mano donde tengo 2 cartas de los palos restantes, el análisis es el mismo que usamos recién, este proceso se repite un total de 4 veces (una por cada palo) por lo que la cantidad de manos que se pueden armar es:

$$
171366 \cdot 4 = 685464
$$
## **b)**

En términos del principio de palomar relacionamos la cantidad de formas de dar una mano de poker tal que al menos haya una carta de cada palo con la cantidad de palomares, esa cantidad gracias a la resolución del punto anterior sabemos que es 6856464. La cantidad de palomas la relacionamos con la cantidad de manos que nos da el enunciado del punto **b)**

Por definición del principio del palomar, si tenemos $\text{cantidad palomas} \gt \text{cantidad palomares}$ nos aseguramos que al menos un palomar tienen al menos dos palomas, en el contexto de nuestro problema eso significa que al menos dos manos van a ser iguales, por lo tanto y respondiendo a la pregunta, no, las 685465 no van a ser todas distintas.

---

## Enunciado De Clase 52

## Se Tienen 5 Esferas De Color Verde, 5 De Color Rojo Y 5 De Color Azul, Y Se Quieren Distribuir En Tres Tubos Verticales Distintos Con Las Siguientes Condiciones

 - El tubo 1 debe tener al menos una esfera.
 - El tubo 2 debe tener al menos una esfera.
 - Las 5 esferas verdes no deben estar todas juntas.

¿Cuántas distribuciones se pueden hacer?

Nota 1: Dos esferas del mismo color son indistinguibles.

Nota 2: Todas las esferas y los tubos tienen el mismo diámetro.

Nota 3: Todos los tubos tienen capacidad para todas las esferas.

**Respuesta**

Sea $S$ el conjunto cuyos elementos son las formas de distribuir las esferas del enunciado en 3 tubos distintos, definimos las siguientes propiedades:

$$  
\begin{aligned}
P_1 &= \text{El primer tubo no tiene esferas}\\
P_2 &= \text{El segundo tubo no tiene esferas}\\
P_3 &= \text{Las esferas verdes estan juntas}
\end{aligned}
$$

También los subconjuntos $A_i$ de $S$ con $1 \le i \le 3$ tal que los elementos de $A_i$ satisfacen la propiedad $P_i$, Bajo estas condiciones lo pedido en el enunciado se resuelve calculando el cardinal de $\overline{A_1} \cap \overline{A_2} \cap \overline{A_3}$ para ello usaremos el principio I-E para 3 propiedades.

$$  
\begin{aligned}
|\overline{A_1} \cap \overline{A_2} \cap \overline{A_3}| =
|S| - |A_1| - |A_2| - |A_3| +
|A_1 \cap A_2| + |A_1 \cap A_3| + |A_2 \cap A_3| -\\
|A_1 \cap A_2 \cap A_3|
\end{aligned}
$$

Calculemos los cardinales:

- $|S|$ : Para cada color contamos con 5 esferas, que pueden ser ubicadas en 3 tubos distintos, al tener una cantidad ilimitada de espacio por tubo podemos usar el teorema de combinatoria con elementos repetidos, lo que nos ayuda a calcular la cantidad de formas de seleccionar a que tubo van a ser asignadas las esferas, eso es igual a $\begin{pmatrix} 7 \\ 2 \end{pmatrix}$, esto es así para cada uno de los colores, entonces por principio multiplicativo tenemos que:
  $$\begin{pmatrix} 7 \\ 2 \end{pmatrix} \cdot \begin{pmatrix} 7 \\ 2 \end{pmatrix} \cdot \begin{pmatrix} 7 \\ 2 \end{pmatrix} = 9261 $$
  esto equivale a la cantidad de formas de distribuir las esferas en los tres tubos sin restricciones.
- $|A_1|$ = Distribuciones donde el tubo 1 no tenga esferas, en este caso seguimos una lógica similar al calculo del conjunto anterior, pero con un ajuste, en este caso solo contamos con 2 tubos, por lo tanto por cada color necesitamos contar la cantidad de formas de seleccionar entre los dos tubos que se le asignaran a las esferas, por principio multiplicativo eso es:
  $$\begin{pmatrix} 6 \\ 1 \end{pmatrix} \cdot \begin{pmatrix} 6 \\ 1 \end{pmatrix} \cdot \begin{pmatrix} 6 \\ 1 \end{pmatrix} = 216$$
- $|A_2|$ = Resulta lo mismo que el calculo del cardinal de $A_1$ solo que en vez de ser el primer tubo el que tiene la restricción es el segundo, pero la cantidad de distribuciones permanece la misma. 216
- $|A_3|$ = Las distribuciones donde las esferas verdes estén juntas, para ello tenemos 3 casos. definamos los siguientes subconjuntos de $A_3$
  - X : Todas las esferas están en el 1er tubo
  - Y : Todas las esferas están en el 2do tubo
  - Z : Todas las esferas están en el 3er tubo

Por principio aditivo tenemos que:

$$
|A_3| = |X| + |Y| + |Z|
$$

Calculemos los cardinales de los subconjuntos:

- $|X|$ = Ubicamos todas las esferas en el primer tubo, ahora para cada color restante contamos con 5 esferas que pueden ser ubicadas en 3 tubos distintos, debido a que tenemos una cantidad de espacio ilimitada en todos los tubos usamos el teorema de combinatoria con elementos repetidos para contar la cantidad de seleccionamientos de tubos para que sean asignados como el lugar donde se asigna cada esfera, eso es igual a $C(7, 2)$, esto se cumple para cada uno de los colores restantes, el azul y rojo, entonces por principio multiplicativo tenemos que:
  $$\begin{pmatrix} 7 \\ 2 \end{pmatrix} \cdot \begin{pmatrix} 7 \\ 2 \end{pmatrix} = 441$$
- $|Y|$ y $|Z|$ = Resulta lo mismo que el calculo del cardinal de $X$
Ahora podemos seguir en nuestro calculo para obtener $|A_3|$

$$  
\begin{aligned}
|A_3| &= |X| + |Y| + |Z|\\
|A_3| &= 441 + 441 + 441\\
|A_3| &= 1323\\
\end{aligned}
$$
- $|A_1 \cap A_2|$= La cantidad de distribuciones sin esferas en el primer y segundo tubo, por lo que solo hay una forma de colocar las esferas, todas en el tercer tubo, por lo que el cardinal de $A_1 \cap A_2 = 1$
- $|A_1 \cap A_3|$= La cantidad de distribuciones sin esferas en el primer tubo, y las esferas verdes juntas, hacemos un análisis análogo al calculo que hicimos para obtener el cardinal de $A_3$ pero solo con dos tubos (Ya que el primero debe estar vacío)
  Tenemos dos casos, uno donde todas las esferas verdes están en el segundo tubo y el otro donde todas las esferas verdes están en el tercer tubo, para cada uno de estos casos, las esferas de los colores restantes tienen $C(6,1)$ formas de ser distribuidas entre los dos tubos restantes, así que principio multiplicativo tenemos que:
  $$ 2 \cdot  \begin{pmatrix} 6 \\ 1 \end{pmatrix} \cdot \begin{pmatrix} 6 \\ 1 \end{pmatrix}   = 72$$
  Esto equivale al cardinal de $A_1 \cap A_3$
- $|A_2 \cap A_3|$ = Resulta el mismo resultado del calculo del cardinal de $A_1 \cap A_3$
- $|A_1 \cap A_2 \cap A_3|$ = La cantidad de distribuciones sin esferas en el primer y segundo tubo y las esferas verdes todas en el mismo tubo, por lo que nos queda somo una forma de distribuir las esferas, todas en el tercer tubo.

Reemplazamos los cardinales en la expresión del principio I-E para tres propiedades:

$$9261 - 2 \cdot 216  - 1323 + 1 + 2 \cdot 72 - 1 = 7650$$

Esto equivale a la cantidad de distribuciones de las esferas teniendo en cuenta las restricciones del enunciado.

---

## Ejercicio De Repaso 7

## Cuatro Amigos Ganan Un Día En Un Parque De Diversiones Para Ellos Solos

**a)** Suponiendo que el primer juego al que van es una montaña rusa con un trencito de 8 asientos individuales, ¿de cuántas maneras se pueden ubicar los 4 amigos de forma que no haya 3 asientos seguidos ocupados?

**b)** Suponiendo que el segundo juego al que van es de las sillas voladoras con un total de 8 sillas, ¿de cuántas maneras se pueden ubicar los 4 amigos de forma que no haya 3 sillas seguidas ocupadas?

**Respuesta**
### **a)**

Observemos que los asientos tienen un orden secuencial, por lo que podemos representar las distribuciones usando una codificación binaria, donde los 1's representan un asiento ocupado, y los 0's asientos vacíos.

Definamos el conjunto $S$ cuyos elementos son las formas de armar una cadena de cuatro 1's y cuatro 0's y al subconjunto $A$ de $S$ cuyos elementos tienen tres unos seguidos. También definamos el subconjunto $B$ de $S$ cuyos elementos tienen los cuatro unos seguidos. El problema se resuelve calculando

$$
|S| - |A| - |B|
$$

Calculemos los cardinales:

- $|S|$= La cantidad de cadenas sin restricciones, para ello de los ocho espacios necesitamos contar la cantidad de formas de seleccionar cuatro espacios, eso es igual a $C(8, 4)$, y por cada uno de esta selecciones tenemos contar las permutaciones de los unos que van a ocupar los espacios previamente seleccionados, entonces por principio multiplicativo tenemos que:
  $$ C(8,4) \cdot 4! = 1680$$
  esto equivale al cardinal de $S$
- $|A|$ = La cantidad de cadenas con tres unos seguidos y el restante aislado, para ello vamos a dejar afuera uno de los unos, por lo que nos quedan 3 unos, vamos a tener dos escenarios:
  - Los empezamos a colocar desde el inicio o el final
  - Los colocamos en cualquier otra parte

En el primer escenario al ubicar los tres unos desde el comienzo nos queda esta distribucion:

$$11100000 $$

Ahora nos queda por seleccionar uno de los 5 espacios ocupados por los ceros para que se le asigne al uno que dejamos afuera, pero notar que no puede estar en el cuarto lugar porque tendriamos 4 lugares ocupados consecutivamente, por eso nuestros posibles espacios se reducen a 4.

Entonces la cantidad de formas de seleccionar 1 espacio entre 4 es $C(4,1)$ y por cada uno de estos seleccionamientos tenemos que contar las permutaciones de los 4 unos, que representarían a las personas, por principio multiplicativo esto es igual a:

$$ C(4,1) \cdot 4! $$

Este mismo calculo se produce si colocamos los tres unos consecutivos al final, por lo tanto la cantidad de formas de distribuir las personas con tal de que haya asientos ocupados consecutivamente al inicio y al final es:

$$ C(4,1) \cdot 4! \cdot 2 = 192$$

Nos queda por contar los casos donde los tres unos consecutivos empiecen a partir de cualquier otro lugar, teniendo la siguiente distribución:

$$ 01110000 $$

Nos quedan 5 posibles lugares en donde el uno que dejamos afuera puede ser ubicado, pero no puede ocupar la posición directamente anterior ni posterior a los tres unos, por lo que los espacios posibles se reducen a 3, por lo tanto contar la cantidad de posibles selecciones de unos de estos tres lugares es $C(3,1)$, y por cada uno de estos seleccionamientos tenemos que contar las permutaciones de los cuatro unos de la cadena, y esto se repite 6 veces, ya que no contamos las posiciones del inicio y del final, entonces por principio multiplicativo tenemos que:

$$ C(3,1) \cdot 4! \cdot 6 = 432$$

equivale a la cantidad de formas de distribuir los tres unos seguidos sin empezando su colocación en cualquier posición a excepción del inicio y el final

Ahora tenemos que sumar las cantidades que surgen de cada escenario:

$$ 192 + 432 = 624$$

Esto equivale al cardenal de $A$

- $|B|$= Si agrupamos los cuatro unos seguidos, de los 8 espacios vamos a contar con 5 espacios posibles, por lo que contar las formas de seleccionar un espacio de cinco posibles es igual a $C(5,1)$, y por cada uno de estos seleccionamientos tenemos que contar las permutaciones de los unos, por principio multiplicativo tenemos que:

$$
C(5,1) \cdot 4! = 120
$$

Esto equivale al cardinal de $B$

Ahora podemos seguir nuestro calculo

$$  
\begin{aligned}
|S| - |A| - |B|\\
1680 - 624 - 120 = 936
\end{aligned}
$$

Esto equivale a la cantidad de formas de distribuir a las cuatro personas en ocho asientos de modo que no haya tres asientos consecutivos ocupados.
