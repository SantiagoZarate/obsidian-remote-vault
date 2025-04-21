## Dada la Palabra EQUILIBRIO Se Desea Saber

**a)** ¿cuántas palabras distintas se pueden formar usando todas las letras de la palabra dada?

**b)** ¿cuántas palabras distintas se pueden formar usando todas las letras de la palabra dada tal que no comiencen con E y no terminen con I?

**c)** ¿cuántas palabras distintas se pueden formar usando todas las letras de la palabra dada tal que comiencen con I o terminen con E, y contengan el anagrama QUE?

**Respuesta**

### **a)**

Observemos que con las letras de la palabra dada podemos armar el siguiente multiconjunto:

$$ \{ 1 \cdot E, 1 \cdot Q , 1 \cdot U, 3 \cdot I, 1 \cdot L, 1 \cdot B, 1 \cdot R, 1 \cdot O \} $$

Contar la cantidad de permutaciones de ese multiconjunto teniendo en cuenta que tiene tres repeticiones de la clase de elemento $I$ y un total de 10 elementos es:

$$ \frac{10!}{3!} = 604800$$

Esto equivale a la cantidad de palabras que se pueden formar a partir de las letras de la palabra del enunciado.

### **b)**

Sea $S$ el conjunto cuyos elementos son las palabras que se pueden formar a partir de las letras de la palabra EQUILIBRIO, definimos el subconjunto $A$ de $S$ cuyos elementos son palabras que empiecen con E y terminen con I, por definición de complemento tenemos $\overline{A}$ tal que sus elementos son palabras que no empiezan con E y no terminan con I, el problema se resuelve calculando el cardinal de $\overline{A}$, por principio de sustracción es igual a:

$$|\overline{A}| = |S| - |A|$$

Calculemos los cardinales.

- $|S|$ = $604800$, lo calculamos en el punto **a)**
- $|A|$ = Fijamos la letra $E$ a la primer posición y una de las $I$ a la última, por lo que nos queda por contar los ordenamientos de las 8 restantes letras teniendo en cuenta que el tipo de elemento $I$ tiene 2 repeticiones, eso es igual a
  $$ \frac{8!}{2!} = 20160 $$
Ahora podemos seguir con el cálculo del cardinal de $\overline{A}$:
$$  \begin{aligned}
|\overline{A}| &= |S| - |A|\\
|\overline{A}| &= 604800 - 20160\\
\end{aligned}
$$Esto equivale a la cantidad de palabras que se pueden formar a partir de la palabra dada con las restricciones propuestas por el enunciado.

### **c)**

Observemos que tenemos dos casos, el primero donde debemos contar las palabras que comiencen con I y contengan el anagrama QUE, y el segundo caso donde terminen con la E y tengan el anagrama QUE.

El problema se resuelve haciendo la sumatoria de la cantidad de palabras que se pueden armar en cada caso.

Para el primer caso, fijamos la I a la primer posición, y declaramos la variable $X$ como el anagrama QUE, por lo que podemos declarar el siguiente multiconjunto:

$$ \{ 2 \cdot I, 1 \cdot L, 1 \cdot B , 1 \cdot R, 1 \cdot O, 1 \cdot X \} $$

la cantidad de permutaciones de 7 elementos con dos repeticiones de la clase de elemento $I$ es igual a:
$$ \frac{7!}{2!} $$
