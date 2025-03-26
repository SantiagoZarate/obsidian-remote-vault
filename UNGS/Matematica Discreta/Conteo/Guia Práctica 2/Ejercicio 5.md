---
status: TODO
---

## Considere El Conjunto Formado Por Las Permutaciones De Todas Las Letras De la Palabra MANTENIMIENTO

**a)** ¿Cuántas de estas permutaciones no comienzan con vocal y terminan con una consonante?

**b)** ¿Cuántas de estas permutaciones tienen la secuencia de letras MIENTO? por ejemplo la palabra ANMIENTOTENIM es una posibilidad.

**c)** ¿Cuántas de estas permutaciones no tienen dos o más vocales juntas?

**Respuesta**

### **a)**

Sea $S$ el multiconjunto:

$$
\{
\underline{2 \cdot M },\underline{1 \cdot A },\underline{3 \cdot N},\underline{2 \cdot T},\underline{2 \cdot E },\underline{2 \cdot I },\underline{1 \cdot O }, 
\}$$
Se nos pide calcular la cantidad de permutaciones de la palabra del enunciado que empieze y termine con una consonante.

Sea $S$ el conjunto que se considera en el enunciado, definimos $M \subset S$ el conjunto cuyos elementos son palabras que empiezan y terminan con la misma consonante.

Notar que todas las consonantes que aparecen en la palabra se repiten exactamente 2 veces. Originalmente la palabra contiene 13 letras, pero al final la primera y ultima posición con la misma letra, las letras intermedias se reducen a 11.

Sea cual sea la consonante que elijamos para fijar, el multiconjunto del que habría que calcular sus permutaciones tendrá 6 tipos de elementos, con 4 tipos de elementos que se repiten 2 veces, 


%% Hacer el calculo %%

Notar que solo calculamos los ordenamientos de las palabras que empiezan y terminan con la misma consonante, así que definimos $T \subset S$ el conjunto cuyos elementos son palabras que empiezan con una consonante y terminan con otra consonante distinta a la primera:

Definimos el multiconjunto $G = \{ 2 \cdot M, 2 \cdot N, 2 \cdot T  \}$

Si fijamos una letra al principio del tipo de elemento que tenemos en $G$, tenemos dos letras que podemos elegir para fijar en la última posición, por ejemplo:
$$  

\begin{aligned}

&M ... N\\

&M ... T\\

&M ... M \leftarrow \text{No se considera porque tiene la misma consonante}

\end{aligned}

$$
Por principio multiplicativo tenemos que $2³$ es la cantidad de elegir 2 consonantes distintas.

Ahora necesitamos calcular las permutaciones de las letras intermedias, sea cual sea las consonantes que elegimos para la primer y última posición, contamos con un multiconjunto compuesto por todas las vocales, 1 consonante con 2 repeticiones y 2 consonantes que se repiten 1 vez.

Así que tenemos un multiconjunto con 7 tipos de elementos, donde 3 clases de elementos tienen 2 repeticiones, el número de permutaciones de 11 elementos es:
$$

\frac{11!}{2!\cdot2!\cdot2!}

$$

> [!NOTE] TODO
> Hice mal el conteo de letras de la palabra al principio, y puse que solo había 2 N, lo que me cambia la forma de calcular.
