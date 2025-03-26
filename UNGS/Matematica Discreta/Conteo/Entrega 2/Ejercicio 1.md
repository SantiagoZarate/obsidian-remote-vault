## Se Tiene la Palabra PARALELEPIPEDO

**a)** ¿Cuántas palabras distintas se pueden formar, con todas las letras de la palabra dada, si las consonantes deben estar juntas?

**b)** ¿Cuántas palabras distintas se pueden formar, con todas las letras de la palabra dada, si la cadena de caracteres PARALELO debe figurar textualmente en la palabra?

**c)** ¿Cuántas palabras distintas se pueden formar, con todas las letras de la palabra dada, si las vocales deben aparecen en la palabra ordenadas alfabéticamente? Por ejemplo la palabra PARALELEPEPIDO es un caso a contar, al igual que la palabra AAEPPRLEDELIOP. Por otro lado la palabra PARALELEPIPEDO no es un caso a contar.

**d)** ¿Cuántas palabras distintas se pueden formar, con todas las letras de la palabra dada, si la misma debe tener al menos dos vocales consecutivas?

**e)** ¿Cuántas palabras distintas se pueden formar con diez letras tomadas de la palabra dada si la misma no debe tener tres letras iguales?

**f)** ¿De cuántas formas distintas se pueden acomodar en ronda todas las letras de la palabra dada ?

**Respuesta**

### **a)** *¿Cuántas Palabras Distintas Se Pueden Formar, Con Todas Las Letras De la Palabra Dada, Si Las Consonantes Deben Estar Juntas?*

Observemos que la palabra del enunciado tiene las siguientes letras:

$$
\{P,A,R,L,E,I,D,O \}
$$

Sea $S$ el siguiente multiconjunto cuyos elementos son las consonantes de la palabra:

$$
\{ \underline{3\cdot P},\underline{1\cdot R}, \underline{2 \cdot L}, \underline{1\cdot D}\}
$$

Calcular la cantidad de ordenamientos de $S$ teniendo en cuenta que tiene 5 tipos de elementos, con 3 repeticiones del tipo P y 2 repeticiones de L. Contar las permutaciones de 7 elementos de $S$ es:

$$
\frac{7!}{3!\cdot2!}
$$

Definimos el multiconjunto $V$ cuyos elementos son las vocales de la palabra:

$$
\{ \underline{2 \cdot A}, \underline{3 \cdot E}, \underline{1 \cdot I}, \underline{1\cdot0} \}
$$

Contar los ordenamientos de $V$ teniendo en cuenta que tiene 4 tipos de elementos, con 2 repeticiones del tipo A y 3 repeticiones del tipo E, contar las permutaciones de 7 elementos de $V$ es:

$$
\frac{7!}{3!,2!}
$$

Para cada uno de los elementos de $S$ tenemos $|V|$ ordenamientos de las vocales, entre las 7 vocales tenemos 8 espacios donde ubicar todas las consonantes juntas, por lo que por principio multiplicativo tenemos que:

$$
\frac{7!}{3!,2!} \cdot \frac{7!}{3!,2!} \cdot 8
$$

Esto equivale a la cantidad de palabras que tengan todas las consonantes juntas según la palabra del enunciado.

### **b)** *¿Cuántas Palabras Distintas Se Pueden Formar, Con Todas Las Letras De la Palabra Dada, Si la Cadena De Caracteres PARALELO Debe Figurar Textualmente En la Palabra?*

Teniendo en cuenta que la palabra PARALELO debe figurar textualmente dentro de las palabra que se formar, descartamos las letras de PARALELO para definir el siguiente multiconjunto $M$:

$$
\{ \underline{2\cdot P}, \underline{2 \cdot E}, \underline{1 \cdot I},\underline{1\cdot D}  \}
$$

Calculamos los ordenamientos de $M$ teniendo en cuenta que tiene 4 tipos de elementos, con 2 repeticiones de P y E. El número de permutaciones de 6 elementos de $M$ es:

$$
\frac{6!}{2!\cdot2!}
$$

Por cada uno de los ordenamientos de $M$ tenemos 7 espacios donde ubicar la palabra PARALELO, por lo que por principio multiplicativo tenemos que:

$$
\frac{6!}{2!\cdot2!} \cdot 7
$$

Esto equivale a la cantidad de palabras que se pueden formar según lo pedido en **b)**

### **c)** *¿Cuántas Palabras Distintas Se Pueden Formar, Con Todas Las Letras De la Palabra Dada, Si Las Vocales Deben Aparecen En la Palabra Ordenadas Alfabéticamente? Por Ejemplo la Palabra PARALELEPEPIDO Es Un Caso a Contar, Al Igual Que la Palabra AAEPPRLEDELIOP. Por Otro Lado la Palabra PARALELEPIPEDO no Es Un Caso a contar.*

Observemos que solo existe un orden alfabético para las letras, en este caso se nos piden las palabras con las vocales ordenadas alfabéticamente, es decir que aparezcan en el siguiente orden:

$$
AAEEEIO
$$

Ahora hace falta ver los ordenamientos y colocamientos de las consonantes, notemos que la palabra dada tiene 14 letras, así vamos a seleccionar 7 espacios que van a ser ocupados por las consonantes, los restantes 7 espacios van a ser ocupados por las vocales ordenadas alfabéticamente. Nuestra selección equivale a $C(14,7)$

Por cada uno de las selecciones contamos con la cantidad de ordenamientos de los elementos del siguiente multiconjunto:

$$
\{ \underline{3 \cdot P}, \underline{1 \cdot R}, \underline{2 \cdot L}, \underline{1 \cdot D} \}
$$

El multiconjunto definido tiene 4 tipos de elementos, el tipo P con 3 repeticiones, el tipo L con 2 repeticiones, el número de permutaciones de los 7 elementos del multiconjunto es:

$$
\frac{7!}{3!\cdot2!}
$$

Entonces la cantidad de palabras que respeten lo pedido en el punto **c)** es:

$$
C(14,7) \cdot \frac{7!}{3!\cdot2!}
$$
### **d)** *¿Cuántas Palabras Distintas Se Pueden Formar, Con Todas Las Letras De la Palabra Dada, Si la Misma Debe Tener Al Menos Dos Vocales consecutivas?*

Sea $S$ el conjunto cuyas elementos son las palabras que se pueden formar con las letras de la palabra dada, definimos $M \subset S$ el conjunto cuyos elementos tienen las vocales separadas, por definición de complemento tenemos $\overline{M}$ como el conjunto cuyas palabras tiene al menos dos vocales contiguas, nos interesa calcular $|\overline{M}|$, por principio de sustracción tenemos que:

$$
|\overline{M}| = |S| - |M|
$$

Calculemos entonces cada cardinal:

- $|S| = ?$

Definimos el siguiente multiconjunto=

$$
\{\underline{3 \cdot P}, \underline{2 \cdot A},\underline{1 \cdot R},
\underline{2 \cdot L},\underline{3 \cdot E}, \underline{1 \cdot I},
\underline{1 \cdot D},\underline{1\cdot0} \}
$$

Contar los ordenamientos de $S$, teniendo en cuenta que tiene 8 tipos de elementos, con 3 repeticiones de la letra P, 3 de la E, 2 de la A y 2 de la L, por teorema sabemos que la cantidad de permutaciones de 14 elementos de $S$ es:

$$
\frac{14!}{3!\cdot3!\cdot2!\cdot2!}
$$

Eso equivale a la cantidad de elementos de $S$

- $|M| = ?$

Ahora tenemos que calcular la cantidad de elementos de $S$ que tengan las vocales separadas. Para ello, del total de 14 letras de la palabra restamos las 7 vocales y nos quedamos con las 7 consonantes, notar que tenemos 8 espacios entre estas 7 consonantes, por lo que necesitamos seleccionar 7 de los 8 espacios disponibles para poder asignarlo a una vocal, lo que es igual a:

$$
C(8,7)
$$

Ahora, tenemos que tener en cuenta que por cada una de esas selecciones tenemos que ordenar las consonantes que ya estaban fijas, teniendo en cuenta el multiconjunto con las consonantes:

$$
\{ \underline{3 \cdot P}, \underline{1 \cdot R}, \underline{2 \cdot L}, \underline{1 \cdot D} \}
$$

La cantidad de permutaciones de 7 elementos con 3 repeticiones de P y 2 de L es:

$$
\frac{7!}{3!\cdot2!}
$$

También por cada uno de estos ordenamientos tenemos que tener en cuenta el orden de las vocales que se entrelazan con las vocales, teniendo en cuenta el multiconjunto vocales:

$$
\{ \underline{2 \cdot A}, \underline{3 \cdot E}, \underline{1 \cdot I}, \underline{1\cdot0} \}
$$

La cantidad de permutaciones de 7 elementos con 3 repeticiones de E y 2 de A es:

$$
\frac{7!}{3!\cdot2!}
$$

Entonces por principio multiplicativo tenemos que:

$$
|M| = C(8,7) \cdot \frac{7!}{3!\cdot2!} \cdot \frac{7!}{3!\cdot2!}
$$

Ahora que ya tenemos los cardinales de $S$ y $M$ podemos obtener $|\overline{M}|$:

$$  
\begin{aligned}
|\overline{M}| &= |S| - |M|\\  
|\overline{M}| &= \frac{14!}{3!\cdot3!\cdot2!\cdot2!} - C(8,7) \cdot \frac{7!}{3!\cdot2!} \cdot \frac{7!}{3!\cdot2!}\\  
\end{aligned}
$$

Eso equivale a la cantidad de palabras que se pueden formar con la palabra dada teniendo en cuenta que tengan al menos 2 vocales juntas.

### **e)** *¿Cuántas Palabras Distintas Se Pueden Formar Con Diez Letras Tomadas De la Palabra Dada Si la Misma no Debe Tener Tres Letras iguales?*

Notemos que la palabra dada tiene 8 tipos de letras distintas y como se necesitan formar palabras de 10 letras algunas de ellas deberán estar repetidas. Queremos calcular el cardinal del conjunto $S$ definido como las palabras de 10 letras usando las letras de la palabra del enunciado.

Observemos que solo hay repetición de las letras P, A, L y E, como máximo podemos tomar 2 de sus repeticiones, por ej. las letras P y E tienen 3 veces, así que solo podemos agarrar 2.

Necesito seleccionar 2 de las 4 letras que repiten, que van a servir para poder llegar a las 10 letras que se requieren para la palabra, lo que es igual a $C(4,2)$.

Por cada uno de estas selecciones, voy a poder armar un multiconjunto donde de las 8 letras distintas que tiene la palabra 2 van a tener 2 repeticiones, las 6 restantes letras solo aparecen 1 vez, por lo que por teorema sabemos las permutaciones de un multiconjunto con 10 elementos es:

$$
\frac{10!}{2!\cdot2!}
$$

Entonces por principio multiplicativo tenemos que:

$$
|S| = C(4,2) \cdot \frac{10!}{2!\cdot2!}
$$

Entonces esto equivale a la cantidad de palabras que se pueden formar de 10 letras teniendo en cuenta lo pedido en el enunciado.

### **f)** *¿De Cuántas Formas Distintas Se Pueden Acomodar En Ronda Todas Las Letras De la Palabra Dada ?*

Ahora se nos piden ordenar las letras de la palabra dada en ronda y contar sus permutaciones, definimos el multiconjunto $S$ que tiene las letras de la palabra dada:

$$
\{\underline{3 \cdot P}, \underline{2 \cdot A},\underline{1 \cdot R},
\underline{2 \cdot L},\underline{3 \cdot E}, \underline{1 \cdot I},
\underline{1 \cdot D},\underline{1\cdot0} \}
$$

Observemos que para contar los ordenamientos en ronda de un conjunto con elementos repetidos necesitamos que haya al menos una clase de elementos que este presente solo 1 vez, en $S$ tenemos 4 clases de elementos que cumplan este requisito, las letras R, I, D y O.

Tomamos como referencia a la letra R como el punto de origen de la ronda, pero podemos pensar a la ronda como una hilera, donde tenemos que colocar las en posiciones relativas a R, por que la contar los ordenamientos del multiconjunto $S$ es:

$$
\frac{14!}{3!\cdot3!\cdot2!\cdot2!}
$$

Como se nos pide ordenarlas en ronda, cada 14 ordenamientos lineales tenemos 1 ordenamiento circular distinto, lo que equivale a:

$$
\frac{1}{14} \cdot \frac{14!}{3!\cdot3!\cdot2!\cdot2!}
$$

Esto seria la cantidad de formar de ordenar las letras de la palabra dada en ronda.
