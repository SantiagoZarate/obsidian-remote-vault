## Se Tienen 5 Esferas De Color Verde, 5 De Color Rojo Y 5 De Color Azul, Y Se Quieren Distribuir En Tres Tubos Verticales Distintos Con Las Siguientes Condiciones

 - El tubo 1 debe tener al menos una esfera.
 - El tubo 2 debe tener al menos una esfera.
 - Las 5 esferas verdes no deben estar todas juntas.

¿Cuántas distribuciones se pueden hacer?

Nota 1: Dos esferas del mismo color son indistinguibles.

Nota 2: Todas las esferas y los tubos tienen el mismo diámetro.

Nota 3: Todos los tubos tienen capacidad para todas las esferas.

**Respuesta**

Asignamos 1 esfera al primer tubo, 1 esfera al segundo tubo, de esta manera satisfacemos las restricciones mínimas, luego haciendo uso de el teorema de combinaciones con elementos repetidos tenemos que la cantidad de formas de seleccionar 3 tubos para que sea donde cada una de las esferas va a ser distribuida es $C(12, 2)$.

Ahora nos queda contar las formas en que se pueden distribuir tal que las esferas verdes no estén juntas, para eso definimos el conjunto $S$ cuyos elementos son las formas de distribuir las 15 esferas en los 3 tubos con la restriction de que el primer y segundo tubo tengan al menos una esfera, definimos el subconjunto $A$ de $S$ cuyos elementos tienen a las esferas verdes juntas, nos interesa calcular $\overline{A}$, por principio de sustracción sabemos que es igual a:

$$
|\overline{A}|  = |S| - |A|
$$

Sabemos que $|S|$ es $C(12, 2)$, ahora para calcular $|A|$ suponemos que todas las esferas van al primer tubo, entonces del total de 13 esferas nos queda 7, usando el teorema de combinatoria con elementos repetidos tenemos $C(6, 2)$ formas de seleccionar a que tubo va cada esfera, esto se repite poniendo las esferas en el segundo y tercer tubo, entonces por principio multiplicativo tenemos que:

$$
\begin{pmatrix} 6 \\ 2 \end{pmatrix} \cdot \begin{pmatrix} 6 \\ 2 \end{pmatrix} \cdot \begin{pmatrix} 6 \\ 2 \end{pmatrix} 
$$

Eso equivale a $|A|$, ahora podemos seguir con el calculo de $|\overline{A}|$

$$  
\begin{aligned}
|\overline{A}|  = |S| - |A|\\
|\overline{A}|  = C(12,2) - \begin{pmatrix} 6 \\ 2 \end{pmatrix} \cdot3\\
\end{aligned}
$$

Esto equivale a la cantidad de distribuciones que cumplen con lo que pide el enunciado

---

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
