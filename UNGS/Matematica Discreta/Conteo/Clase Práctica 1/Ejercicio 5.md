El club de matemáticos de Los Polvorines tiene 27 miembros en total. Son 16 mujeres y 11 varones. Quieren formar una comisión de 8 miembros que los represente en las olimpiadas.

**a)** ¿ De cuántas maneras posibles puede conformarse esa comisión?

**b)** ¿ De cuántas maneras posibles puede conformarse esa comisión si se quisiera que esté formada por 4 mujeres y 4 hombres?

**c)** ¿ De cu´antas maneras posibles puede conformarse la comisión si se quisiera que est´e formada por al menos 5 mujeres?

**Respuesta**

## **a)**

Sea el conjunto $S$ cuyos elementos son las formas en que se pueden formar el grupo de 8 miembros a partir de los 27 miembros, lo pedido en el enunciado se resuelve calculando $|S|$.

Para ello necesitamos contar la cantidad de ordenamientos que pueden tener los miembros de la comisión, tomados del grupo de 27 personas, eso es igual a $P(27,8)$

Entonces tenemos el cardinal de $S$

$$
|S| = P(27,8)
$$

La cantidad de formas distintas de armar el grupo de 8 personas es $P(27,8)$

**b)**

Sea el conjunto $M$ cuyos elementos son las formas de armar un grupo de 8 personas a partir de un conjunto inicial de 27 personas, en donde el grupo este formado por 4 mujeres y 4 hombres.

Lo pedido en el enunciado se resuelve calculando $|M|$, para ello definamos los siguientes conjuntos

$$  
\begin{aligned}
Mj &= {Mj_1, Mj_2, ..., Mj_{16}}\\
Vr &= {Vr_1, Vr_2, ..., Vr_{11}}
\end{aligned}
$$

Ahora calculemos cardinal de $M$, sabemos que solo podemos tomar 4 personas de cada género, es decir, tenemos que contar la cantidad de ordenamientos de mujeres tomadas de a 4, lo mismo para los hombres.

Teniendo en cuenta los cardinales de $Mj$ y $Vr$ tenemos lo siguiente

$$  
\begin{aligned}
|Mj| &= P(16, 4)\\
|Vr| &= P(11, 4)\\
\end{aligned}
$$

Notar que para cada una de los ordenamientos de Mujeres contamos con $P(11,4)$ ordenamientos de hombres, así que por principio multiplicativo tenemos que:

$$
|M| = P(16,4) \cdot P(11,4)
$$

Entonces la cantidad de formas de armar la comisión con 4 personas de cada género es de $P(16,4) \cdot P(11,4)$

**c)**

Sea $D$ el conjunto cuyos elementos sean las formas de armar la comisión por al menos 5 mujeres, lo pedido en el enunciado se resuelve obteniendo $|D|$.

Para ello notemos que podemos calcular la cantidad de formas en que se puede armar el grupo con un máximo de 3 varones, de esta forma estamos calculando $|D|$

Definamos los siguiente subconjuntos de D

$$  
\begin{aligned}
D_1 &= \text{Comisiones teniendo 3 varones}\\
D_2 &= \text{Comisiones teniendo 2 varones}\\
D_3 &= \text{Comisiones teniendo 1 varon}\\
\end{aligned}
$$

Notemos que $D = D_1 \cup D_2 \cup D_3$ y que $D_i \cap D_j = \emptyset$ siempre que $i \neq j$, así que $D_1$, $D_2$ y $D_3$ es una partición de D, por lo tanto por principio aditivo tenemos que:

$$
|D| = |D_1| + |D_2| +|D_3|
$$

Para calcular el cardinal de $D_1$ tenemos que calcular la cantidad de ordenamientos del $Vr$ tomados de tres, es decir $P(11, 3)$, y por cada uno de estos ordenamientos contamos con P(16, 5) ordenamientos de mujeres, escogemos 5 mujeres por ordenamientos por que son la cantidad de espacios restantes para armar la comisión luego de elegir los tres hombres.

Entonces tenemos que:

$$  
\begin{aligned}
|D_1| &= P(11,3) \cdot P(16,5)\\
\end{aligned}
$$

Siguiendo un razonamiento análogo al calculo para obtener $|D_1|$ podemos calcular el cardinal de $D_2$ y $D_3$

$$  
\begin{aligned}
|D_2| &= P(11,2) \cdot P(16,6)\\
|D_3| &= P(11,1) \cdot P(16,7)\\
\end{aligned}
$$

Ahora podemos obtener $|D|$:

$$  
\begin{aligned}
|D| &= |D_1| + |D_2| +|D_3|\\
|D| &= P(11,3) \cdot P(16,5) + P(11,2) \cdot P(16,6)+ P(11,1) \cdot P(16,7)
\end{aligned}
$$

Esa seria la cantidad de formas de armar la comisión teniendo 5 mujeres como mínimo en el grupo
