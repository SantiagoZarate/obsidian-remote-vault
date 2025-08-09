Amadeo tiene un metegol con un equipo verde y el otro granate. Los jugadores de cada equipo están numerados y distribuidos en 4 lineas de la siguiente forma:

- Un arquero con el número 1.
- Dos defensores con los números 2 y 3.
- Cinco mediocampistas con los números 4, 5, 6, 7 y 8.
- Tres delanteros con los números 9, 10 y 11.

Para personalizarlo, tiene pelo, barba y bigotes, de dos colores distintos, y quiere ponerle a cada jugador al menos uno de estos accesorios.

(a) ¿De cuántas formas Amadeo puede personalizar su metegol?

(b) ¿De cuántas formas Amadeo puede personalizar su metegol con la condición de que al menos un mediocampista granate sea pelado y al menos uno de los seis delanteros no tenga bigote?

**Respuestas:**

## A

Sea el $A$ el conjunto cuyos elementos son las formas de personalizar el metegol tal que sus elementos usen solo uno de los cosméticos disponibles

para cada uno de los 22 jugadores tenemos $\begin{pmatrix} 3 \\ 1 \end{pmatrix}$ formas de seleccionar cosméticos, y por el cosmético elegido tenemos 2 colores, por lo que la personalización del primer equipo es independiente de la del segundo, por lo que por principio multiplicativo tenemos que:

$$ 22 \cdot \begin{pmatrix} 3 \\ 1 \end{pmatrix} \cdot 2 $$

Sea el conjunto $B$ cuyos elementos

definamos los conjuntos $A_i$ con $1 \le i \le 3$ donde los elementos de $A_i$ tienen $i$ cosméticos.

lo pedido en el enunciado se resuelve calculando $|A_1| + |A_2| + |A_3|$, pasemos a calcular el cardinal de cada conjunto.

- $|A_1|$ = para cada uno de los 22 jugadores tenemos $\begin{pmatrix} 3 \\ 1 \end{pmatrix}$ formas de seleccionar cosméticos (pelo, barba o bigote), y por el cosmético elegido tenemos 2 colores, por lo que la personalización del primer equipo es independiente de la del segundo, por lo que por principio multiplicativo tenemos que:

$$ 22 \cdot \begin{pmatrix} 3 \\ 1 \end{pmatrix} \cdot 2 $$

- $|A_2|$ = para cada uno de los 22 jugadores tenemos $\begin{pmatrix} 3 \\ 2 \end{pmatrix}$ formas de seleccionar cosméticos, y por los cosmético elegido tenemos 2 colores por cosmetico elegido, por lo tanto la siguiente expresion equivale a la cantidad de formas de personalizar el metegol donde cada jugador tenga 2 cosméticos

$$ 22 \cdot \begin{pmatrix} 3 \\ 2 \end{pmatrix} \cdot 2 \cdot 2 $$

- $|A_3|$ = para cada uno de los 22 jugadores tenemos $\begin{pmatrix} 3 \\ 3 \end{pmatrix}$ formas de seleccionar cosméticos, y por los cosmético elegido tenemos 2 colores por cosmetico elegido, por lo tanto la siguiente expresion equivale a la cantidad de formas de personalizar el metegol donde cada jugador tengan los 3 cosméticos

$$ 22 \cdot \begin{pmatrix} 3 \\ 3 \end{pmatrix} \cdot 2 \cdot 2 \cdot 2 $$

Luego la cantidad de formas de personalizar el metegol es:

$$
 22 \cdot \begin{pmatrix} 3 \\ 1 \end{pmatrix} \cdot 2
+
 22 \cdot \begin{pmatrix} 3 \\ 2 \end{pmatrix} \cdot 2 \cdot
+
 22 \cdot \begin{pmatrix} 3 \\ 3 \end{pmatrix} \cdot 2 \cdot 2 \cdot 2
$$

Igual me estoy dando cuenta que esta forma de contar no cubre los casos en donde por ejemplo 21 jugadores tengan 2 cosmeticos y el restante solo esté usando un cosmético.
