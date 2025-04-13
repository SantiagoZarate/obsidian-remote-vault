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
