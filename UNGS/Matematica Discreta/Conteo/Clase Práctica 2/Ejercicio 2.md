## En Un Casamiento, 5 Hombres Y 4 Mujeres Se est´an Por Sacar Una Foto

**a)** Si se los ordena en fila, ¿cuántas fotos pueden sacarse si las mujeres tienen que estar juntas y los hombres también tienen que estar juntos?

**b)** Si se los ordena en fila, ¿cuántas fotos pueden sacarse si no puede haber dos o más mujeres juntas?

**c)** Ahora, ¿cuántas fotos pueden sacarse si las mujeres tienen que estar juntas y los hombres pueden o no estar juntos?

**Respuesta**

### **a)**

Definamos los siguientes conjuntos:

$$  
\begin{aligned}
A &= \text{Las cuatro mujeres}\\
B &= \text{Los cinco hombres}\\
\end{aligned}
$$

Las cantidad de permutaciones de $A$ es igual a $4!$, y por cada una de estas permutaciones, tenemos $5!$ ordenamientos de $B$, y por cada ordenamiento tenemos que tener en cuenta los ordenamientos del conjunto $\{ A, B \}$, que sería $2!$

Luego la cantidad de formas de ordenar la fila con las mujeres juntas y los hombres juntos es:

$$
2! \cdot 4! \cdot 5!
$$

### **b)**

Saquemos a las mujeres del total del grupo, tenemos 5 hombres, entre los cuales tenemos 6 espacios, uno a la derecha de cada hombre y otro al final,

de esos 6 espacios tengo que elegir 4 para poder asignar una mujer, de esta forma nos aseguramos que las mujeres no estén juntas

La cantidad de formas de seleccionar 4 espacios entre los 6 totales es $C(6, 4)$, y por cada uno de esta selecciones, tengo que contar la cantidad de formas de ordenar a las mujeres, lo que es igual a $4!$

Para cada una de estos ordenamientos también tenemos que tener en cuenta el orden de los 5 hombres, la cantidad de formas de ordenarlos es de $5!$

Luego la cantidad de formas de armar la fila con tal de que las mujeres no estén consecutivas es:

$$
C(6, 4)\cdot 4! \cdot 5!
$$
### **c)**

Definamos la siguiente variable:

$$
M = \text{Las 4 mujeres juntas}
$$

Ahora debemos contar las cantidades de ordenamientos de los 5 hombres y $M$, eso es igual a $6!$, y por cada uno de esos ordenamientos hay que tener en cuenta los ordenamientos de $M$, que es igual a $4!$.

Luego la cantidad de formar de ordenar la fila tal que cumplan con lo pedido en el enunciado es:

$$
6! \cdot 4!
$$
