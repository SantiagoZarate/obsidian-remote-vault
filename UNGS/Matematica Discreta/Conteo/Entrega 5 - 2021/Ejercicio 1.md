## Sea El Conjunto A = {0, 1, 2, 3, 4, 6, 8, 9}. ¿Cuántos Números De Ocho Cifras Se Pueden Formar, Tomando Todos Los Elementos De A, De Forma Tal Que Los Dígitos Pares no Estén Ordenados En Forma Creciente Y Que El Número no Tenga a Los Dígitos 8 Y 9 Juntos En Cualquier Orden?

**Respuesta**

Definamos el conjunto $S$ cuyos elementos son los números de ocho cifras que se forman con los elementos de $A$, definamos las siguientes propiedades:

$$  
\begin{aligned}
P_1 &= \text{Los dígitos pares están ordenados en forma decreciente}\\
P_2 &= \text{Los dígitos 8 y 9 están en posiciones contiguas}\\
\end{aligned}
$$

También los subconjuntos $A_i$ de $S$ con $i = 1, 2$ tal que los elementos de $A_i$ satisfacen la propiedad $P_i$. Bajo estas condiciones el problema se resuelve calculando el cardinal de $\overline{A_1} \cap \overline{A_2}$ para ello usaremos el principio I-E para dos propiedades:

$$
|\overline{A_1} \cap \overline{A_2}| = |S| - |A_1| - |A_2| + |A_1 \cap A_2|
$$

Calculemos los cardinales:

- $|S|$= $7 \cdot 7!$ (El cero no puede ir al inicio, por lo que se descuenta la primer posición)
- $|A_1|$= La cantidad de números donde los pares estén ordenados en forma decreciente. Contamos con 5 números pares, el hecho de que los números pares estén ordenados en forma creciente nos impone que tengan este ordenamiento:

$$
86420
$$

Tenemos 6 espacios entre esos dígitos, donde podemos ubicar los tres dígitos restantes, entonces la cantidad de formas de seleccionar los espacios que serán asignados a los dígitos impares es $C(6,3)$, y por cada uno de estos seleccionamientos tenemos que contar las permutaciones entre ello, lo que por principio multiplicativo tenemos que es igual a :

$$
C(6,3) \cdot 3!
$$

Esto equivale al cardinal de $|A_1|$

- $|A_2|$ = La cantidad de números donde los dígitos 8 y 9 estén juntos, asignamos a la variable $X$ esos dos números. Para el número 0 tenemos que descartar la primera posición, por lo que tienen 7 posibles posicionamientos, luego nos quedan los 5 dígitos restantes, mas los 2 que están en $X$, tenemos que contar los ordenamientos en secuencia de 6 elementos, eso equivale a 6! y por cada uno de estos ordenamientos tenemos que tener en cuenta las permutaciones de $X$, que sería $2!$

  Luego tenemos que:

  $$7 \cdot 6! \cdot 2!$$

  equivale al cardinal de $|A_2|$

- $|A_1 \cap A_2|$ = La cantidad de números donde los dígitos pares están en forma decreciente y los números 8 y 9 están juntos, sabemos que tenemos un único ordenamiento para los pares en forma decreciente, a partir de este orden tenemos 6 espacios que pueden ser usados por los restantes números. Notar que en este caso necesitamos al 8 y al 9 juntos, por lo que asignamos a la variable $Y$ , entonces tenemos el siguiente ordenamiento:
  $$Y6420$$
Contamos nuevamente con 6 espacios, de los cuales debemos seleccionar 2 para que se les asignen a los números impares, eso es igual a $C(6, 2)$, por cada uno de estos seleccionamientos tenemos que tener en cuenta las permutaciones de $Y$, que sería $2!$, entonces por principio multiplicativo tenemos que:
$$
C(6, 2) \cdot 2!
$$

Esto equivale a $|A_1 \cap A_2|$

> [!faq] Duda
> Creo que ni hacía falta usar el principio I-E

> [!cite] Chatgpt
> En realidad **sí hacía falta** si querés contar exactamente cuántos números cumplen **ambas condiciones negativas** (ni pares ordenados crecientes, ni 8 y 9 juntos). Usar I-E evita contar doble las intersecciones o subcontar.
>
> Podrías haberlo hecho también **de forma directa**, pero sería más propenso a errores y más largo. Así que tu elección fue adecuada y elegante ✨
