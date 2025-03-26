---
tags:
  - Combinación
  - Permutación-Repetidos
status: Incomplete
---

## Se Tiene Un Tablero De 8 Filas Y 8 Columnas, 6 Fichas De Color Rojo, 5 Fichas De Color Azul, 4 Fichas De Color Verde, 3 De Color Blanco Y 2 De Color Negro. Suponiendo Que Las Fichas Del Mismo Color Son Indistinguibles

**a)** ¿De cuántas formas se pueden ubicar las 20 fichas en el tablero?

**b)** ¿De cuántas formas se pueden ubicar las 20 fichas en el tablero con la condición de que en cada fila haya como mucho 1 ficha roja?

**c)** ¿De cuántas formas se pueden ubicar las 20 fichas en el tablero con la condición de que en el lugar (1,1) y en el lugar (8,8) haya fichas blancas o negras?

**Respuesta**

### **a)**

Observar que podemos pensar a las posiciones del tablero como una fila de 64 espacios vacíos, donde cada 8 espacios representaría una nueva fila. a las fichas las podemos representar por letras, R para las fichas rojas, A para las azules y así con todas.

Podemos pensar un ordenamiento en hilera de estas letras formando una palabra con las cantidades de letras correspondiendo a las cantidad de fichas de cada color según establece el enunciado. Definimos el siguiente multiconjunto $S$:

$$
\{ \underline{6 \cdot R}, \underline{5 \cdot A}, \underline{4 \cdot V}, \underline{3 \cdot B}, \underline{2 \cdot N} \}
$$

Necesitamos contar las permutaciones del $S$, donde tenemos 5 tipos de elementos, cada uno con una cantidad distinta de repeticiones, el número de permutaciones de los 20 elementos de $S$ es:

$$
\frac{20!}{6!\cdot5!\cdot4!\cdot3!\cdot2!}
$$

Para cada uno de los ordenamientos necesitamos seleccionar 20 espacios de los 64 disponibles para que sean asignadas a cada una de las letras, lo que es igual a $C(64, 20)$.

Entonces la cantidad de formas de ubicar las fichas es:

$$
\frac{20!}{6!\cdot5!\cdot4!\cdot3!\cdot2!} \cdot C(64,20)
$$
### **b)**

De las 64 espacios disponibles, vamos a reservar 8, un espacio por fila, vamos a ordenar todas las fichas a excepción de las rojas, entonces nuestro calculo que de la siguiente manera:

$$
\frac{15!}{5!\cdot4!\cdot3!\cdot2!}
$$

Ahora de los 8 espacios por fila reservados, necesitamos contar las formas de seleccionar 6 espacios donde vamos a color una fichas roja, lo que es igual a $C(8,6)$

Entonces la forma de ordenar las fichas con la condición del enunciado es:

$$\frac{14!}{5!\cdot4!\cdot3!\cdot2!} \cdot C(8,6)$$

### **c)**

==TODO==
