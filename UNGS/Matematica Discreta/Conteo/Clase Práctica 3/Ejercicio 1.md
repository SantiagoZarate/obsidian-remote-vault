## De Las 26 Letras Del Alfabeto, ¿cuántos Subconjuntos De Tres Letras Hay Que no Tienen Dos Letras Consecutivas Del Alfabeto?

**Respuesta**

Sea $S$ el conjunto elementos son las letras del alfabeto, la cantidad de subconjuntos de $S$ que tengan tres letras es igual a $\begin{pmatrix} 26 \\ 3 \end{pmatrix}$²

Definamos el conjunto $P$ cuyos elementos son los subconjuntos de $S$ de tres letras, definamos el conjunto $A \subset P$ cuyos elementos tengan dos letras consecutivas en el alfabeto, por definición de complemento tenemos $\overline{A}$ tal que sus elementos no tienen letras seguidas en el alfabeto, lo pedido en el enunciado se resuelve calculando el cardinal de $\overline{A}$ , por principio de sustracción es igual a:

$$
|\overline{A}| = |P| -  |A|
$$

> [!NOTE] Resolucion moodle
> Necesitamos elegir tres letras de las 26 del alfabeto. Vamos a recorrer las 26 letras del alfabeto asignando a cada letra un 0 si no la elegimos o un 1 si la elegimos. Consideramos s´olo una forma de recorrer el alfabeto ya que no nos interesa el orden. Entonces cualquier elecci´on de letras del alfabeto es equivalente a una cadena de 26 bits. En el enunciado se pide elegir tres letras y que entre ellas no haya dos consecutivas, entonces queremos formar cadenas de bits con 3 unos y 23 ceros que no tengan dos unos consecutivos. Para hacer esto vamos a ubicar los 3 unos entre los 23 ceros, es decir, elegimos 3 lugares para los unos de los 24 lugares formados por los 22 lugares entre los ceros y las 2 puntas. Tenemos C(24, 3) = 24! 21!·3! opciones para hacerlo. Como todos los ceros son iguales no es necesario permutarlos entre ellos, lo mismo ocurre con los unos. Por lo tanto, la cantidad de subconjuntos de tres letras hay que no tienen dos letras consecutivas del alfabeto es 24! 21!·3! = 2024.
