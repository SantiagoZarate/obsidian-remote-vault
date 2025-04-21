## Se Denomina Ω El Conjunto De Las Permutaciones De Todas Las Letras De la Palabra MARIPOSARIO

**a)** ¿Cuántos elementos de Ω tienen a las consonantes ordenadas alfabéticamente en el orden en que se lee una palabra?

**b)** ¿Cuántos elementos de Ω tienen letras iguales consecutivas? A modo de ejemplo un elemento de Ω que debemos contar es MAARRIIPOOS.

**c)** ¿Cuántas palabras de 10 letras se pueden formar utilizando las letras de la palabra dada?

**Respuesta**

### **a)**

Observar que a partir de las letras de la palabra dada podemos armar el siguiente multiconjunto.

$$ \{ 1 \cdot M, 2 \cdot A, 2 \cdot R, 2 \cdot I, 1 \cdot P, 2 \cdot O, 1 \cdot S \}$$

Definimos el subconjunto $S$ de $Ω$ tal que sus elementos tengan las consonantes ordenadas alfabéticamente, notar que contamos con 11 posibles posiciones para ubicar cada una de las consonantes, seleccionar 5 de esos 11 espacios es $C(11,5)$ y por cada uno de estos seleccionamientos tenemos que contar las permutaciones de las vocales, notar que podemos armar el siguiente multiconjunto con las vocales:

$$ \{ 2\cdot A, 2 \cdot I, 2 \cdot O \} $$

La cantidad de permutaciones de este multiconjunto es

$$ \frac{6!}{2! \cdot 2! \cdot 2!} $$

Luego por principio multiplicativo tenemos que

$$ C(11,5) \cdot  \frac{6!}{2! \cdot 2! \cdot 2!}$$

equivale a la cantidad de palabras que se pueden armar a partir de las letras de la palabra dada con las consonantes ordenadas alfabéticamente.

### **b)**

Observemos que las letras que se repiten son la $A,R,I$ y $O$, por lo que declaramos las siguientes variables $A^{'}, R^{'}, I^{'}, O^{'}$ tal que tienen las letras repetidas juntas, por lo que redefinimos el conjunto de letras disponibles = ${A^{'}, R^{'}, I^{'}, O^{'}, M, S, P}$ y necesitamos contar las formas de permutar estas letras para formar palabras, eso es igual a 7!
