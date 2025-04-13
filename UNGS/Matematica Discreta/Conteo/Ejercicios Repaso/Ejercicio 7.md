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
