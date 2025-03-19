En un casamiento, 5 hombres y 4 mujeres se están por sacar una foto.

**a)** Si se los ordena en fila, ¿cuántas fotos distintas pueden tomarse?

**b)** El fotógrafo decide ahora que los varones ocupen las posiciones impares, y las mujeres las posiciones pares. ¿Cuántas de estas fotos, distintas entre si pueden sacarse?

**Respuesta**

## **a)**

Sea el conjunto $S$ cuyos elementos sean las formas de tomarse una foto teniendo un grupo de 5 hombres y 4 mujeres, lo pedido en el enunciado se resuelve calculando $|S|$

Teniendo en cuenta que se ponen en forma de fila, podemos contar los ordenamientos de un grupo de 9 personas, que es igual a $P(9,9)$

## **b)**

Ahora que entra en consideración la posición que tienen que tomar las personas según su genero, definimos el conjunto $S$ cuyos elementos son las formas de ordenar las 9 personas para la foto teniendo en cuenta dicha restricción.

Definimos los siguientes conjuntos:

$$  
\begin{aligned}
V &= \text{Conjunto con los 5 hombres}\\
M &= \text{Conjunto con las 4 mujeres}\\
\end{aligned}
$$

Podemos contar los ordenamientos de cada conjunto y tener en cuenta que para cada ordenamiento de elementos, hay que entrelazar los elementos del otro conjunto y empezar colocando a un hombre primero, ya que ocupan los lugares impares.

Entonces para contar los ordenamientos en hilera de $V$, usamos la función de permutación, que es igual a $P(4,4)$, hacemos los mismo con el conjunto $M$, nos queda $P(5,5)$

Notar que para cada uno de los ordenamientos de $V$ tenemos $P(5,5)$ ordenamientos de $M$ en los que se pueden entrelazar, entonces por principio multiplicativo es:

$$  
\begin{aligned}
|S| &= |V| \cdot |M|\\
|S| &= P(4,4) \cdot P(5,5)\\
|S| &= 4! \cdot 5!\\
\end{aligned}
$$

Entonces la cantidad de formas en las que se pueden colocar el grupo de personas teniendo en cuenta las restricciones de las posiciones por género es $4! \cdot 5!$
