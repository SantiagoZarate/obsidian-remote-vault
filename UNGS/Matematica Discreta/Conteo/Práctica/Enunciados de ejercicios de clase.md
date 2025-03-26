**Ejercicio 1.**
Una zapatería vende distintos tipos de zapatos. Vende con tacón y sin tacón. Aquellos zapatos que tienen tacón pueden ser de taco alto y de taco bajo y aquellos que no lo poseen pueden venir con o sin hebilla.

**¿Cuántos tipos distintos de zapatos ofrece la zapatería?**

![[Diagramas de venn|page=page;pos=-187,191;size=846,401]]


***Respuesta:***

Sea el conjunto Zapatos, cuyos elementos son los zapatos ofrecidos por la zapateria, quiero calcular |Zapatos|.

*Voy a usar el principio aditivos, donde |S1| + |S2| + ... + |Sn|  = |S|*

Podemos particionar el conjunto en distintos subconjuntos según sus propiedades, para empezar dividimos el conjunto entre los zapatos con tacón y por otro lado los que no tienen tacón. A su vez el primer grupo puede ser divido entre zapatos de taco alto o bajo, el grupo de zapatos sin tacón de divide a su vez entre los que tienen hebilla y los que no.

En total nos queda el conjunto dividido en cuatro subconjuntos formado con elementos con propiedades claramente distintas. Usando el principio aditivo, donde la intersección entre subconjuntos significa un conjunto vacío, para obtener el cardinal del conjunto Zapato, y teniendo en cuanta que cada subconjunto tiene un solo elemento podemos hacer la siguiente cuenta:

1 + 1+ 1 + 1 = 4

Entonces, la zapateria ofrece 4 zapatos distintos.


---

**Ejercicio 2.**
Una peluquería para mascotas ofrece cortes para gatos y perros. Para perros ofrece tres opciones distintas para la cola, tres para las patas, dos para la cabeza y dos para el resto del cuerpo. Para gatos ofrece dos opciones para la cola, dos para la cabeza y una  única opción para el resto del cuerpo.

**¿Cuántos tipos de corte ofrece la peluquería en total?**

![[Diagramas de venn|page=page;pos=-144,690;size=671,347]]

**Respuesta:**

Sea S el conjunto de los cortes que ofrece la peluquería en total.
Para contar los elementos del conjunto S definamos los siguientes conjuntos:

$$
\begin{aligned}
S_1 &= \{\text{Cortes para perros}\} \\
S_2 &= \{\text{Cortes para gatos}\} \\
\end{aligned}
$$
Observemos que $S = S_1 \cup S_2$ y que $S_1 \cap S_2 = \emptyset$ Es decir, los subconjuntos S1 y S2 son una partición del conjunto S, por lo tanto $|S| = |S_1| + |S_2|$ Para contar el cardinal de cada subconjunto definamos los siguientes conjuntos.

El conjunto S1 se divide de la siguiente manera:

$$
\begin{aligned}
S_1a &= \{\text{Cortes para perros para la cola}\} \\
S_1b &= \{\text{Cortes para perros para las patas}\} \\
S_1c &= \{\text{Cortes para perros para la cabeza}\} \\
S_1d &= \{\text{Cortes para perros para el cuerpo}\} \\
\end{aligned}
$$

El conjunto S2 se divide de la siguiente manera:

$$
\begin{aligned}
S_2a &= \{\text{Cortes para gatos para la cola}\} \\
S_2b &= \{\text{Cortes para gatos para la cabeza}\} \\
S_2c &= \{\text{Cortes para gatos para el cuerpo}\} \\
\end{aligned}
$$

Contemos el cardinal de cada subconjunto:
$$
\begin{aligned}
|S_1a| = 3 \\
|S_1b| = 3 \\
|S_1c| = 2\\
|S_1d| = 2\\
\\
|S_2a| = 2\\
|S_2b| = 2\\
|S_2c| = 1\\
\end{aligned}
$$
Utilizando el principio aditivo tenemos que:
$$
|S_1| = |S_1a| + |S_1b| + |S_1c| + |S_1d|
$$
$$
|S_2| = |S_2a| + |S_2b| + |S_2c|
$$
Entonces:
$$
\begin{aligned}
|S_1| &= 10 \\
|S_2| &= 5
\end{aligned}
$$
Utilizando el principio aditivo nuevamente tenemos que:
$$
|S| = |S_1| + |S_1| + |S_2|
$$
**Rta: $|S| = 15$

---

**Ejercicio 4.**
En las heladerías Grido de Bella Vista y San Miguel se venden distintos gustos de helado. En
cada heladería se ofrece servir los helados en un cucurucho o en tasitas de pasta de oblea. El cliente puede comprar el helado conteniendo una , dos o tres bochas que se ubican una arriba de la otra.

En cada una de las heladerías se tienen los siguientes gustos:

**Heladería de Bella Vista:**
- Dulce de leche
- Flan
- Chocolate
- Americana
- Menta granizada

**Heladería de San Miguel:**
- Granizado
- Tramontana
- Vainilla
- Frutilla

**¿Cuántas tipos de helados distintos se pueden ofrecer entre ambas heladerías?**

Observación: Se considera que un helado es distinto a otro, si tiene distinto tipo de recipiente que lo contiene, distintos sabores, o distinto orden en la confección del helado si tuviera dos o tres bochas.

![[Diagramas de venn|page=page;pos=-124,1072;size=728,351]]

**Respuesta**

Sea S el conjunto de los distintos tipos de helados que se ofrecen entre ambas heladerías.
Definimos los siguientes conjuntos:

$$
\begin{aligned}
S_1 &= \{\text{Elementos de S provenientes de San Miguel}\} \\
S_2 &= \{\text{Elementos de S provenientes de Bella Vista}\} \\
\end{aligned}
$$

***Explayar mas usando la teoría del principio aditivo***  Entonces $|S| = |S_1| + |S_2|$

(Justificación de independencia entre P . Q)

Para calcular el cardinal de $|S_1|$ cada subconjunto pueden ser particionados entre 2 teniendo en cuenta el recipiente, ya sea de cucurucho o pasta de oblea, la cantidad de gustos de helados a elegir no cambia.

Entonces para calcular $|S_1|$ y aplicando el principio multiplicativo tenemos que
$$|S_1| = p . q$$
En este caso P seria la cantidad de recipientes, es decir 2, mientras que Q es la cantidad de combinaciones distintas de helados que ofrece la heladería.

Ahora para calcular la cantidad de combinaciones que ofrece la heladería, hay que tener en cuenta que la cantidad de bochas de helado a elegir puede ser entre 1 a 3. Para el conjunto $S_1$, y recordando que ofrece 5 sabores distintos, tenemos que:

- La primer bocha puede ser ocupada por 5 posibles sabores.
- La segunda bocha puede ser ocupada por 4 posibles sabores mas la opción de no querer un segundo gusto.
- La tercer bocha puede ser ocupada por 3 posibles sabores mas la opción de no querer un tercer gusto.

Entonces para calcular la cantidad de combinaciones que ofrece la heladería tenemos que:
$$5.5.4 = 100$$
Ahora si podemos avanzar y descubrir que 
$$
\begin{aligned}
|S_1| &= 2 \cdot 100 \\
|S_1| &= 200
\end{aligned}
$$
Queda por calcular $|S_2|$ y siguiendo un razonamiento análogo al descubrimiento del conjunto anterior, solo que en este caso la heladería de Bella Vista ofrece 4 gustos distintos, tenemos que:

- La primer bocha puede ser ocupada por 4 posibles sabores.
- La segunda bocha puede ser ocupada por 3 posibles sabores mas la opción de no querer un segundo gusto.
- La tercer bocha puede ser ocupada por 2 posibles sabores mas la opción de no querer un tercer gusto.

Entonces para calcular la cantidad de combinaciones que ofrece la heladería tenemos que:
$$4.4.3 = 48$$Ahora si podemos avanzar y descubrir que
$$
\begin{aligned}
|S_2| &= 2 \cdot 48 \\
|S_2| &= 96 \\
\end{aligned}
$$
Finalmente utilizando el principio aditivo tenemos que:
$$
\begin{aligned}
|S| &= |S_1| + |S_2| \\
|S| &= 200 + 96\\
|S| &= 296
\end{aligned}
$$
**Rta:** $|S|=296$

---
