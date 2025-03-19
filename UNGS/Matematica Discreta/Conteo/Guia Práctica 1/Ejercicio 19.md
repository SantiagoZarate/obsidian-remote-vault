## Imaginemos Un Tablero De Ajedrez De 8 × 8 Casillas. En El Juego De Ajedrez, Dos Torres Se Amenazan Si Se Encuentran En la Misma Fila O En la Misma Columna

**a)** ¿De cuántas formas distintas pueden ubicarse 8 torres iguales que no se amenacen entre sí?

**b)** ¿De cuántas formas distintas pueden ubicarse 8 torres de ocho colores distintos que no se amenacen entre sí?

**Respuesta**

### **a)**

Observemos que inicialmente contamos con 8 posibles columnas donde ubicar una torre, y que si colocamos una torre en la columna 1 , y fila 1, no podemos colocar ninguna torre en la misma fila o columna, Para la siguiente torre no vamos a poder contar con la columna ni la fila que seleccionamos para la primer torre, es decir voy reduciendo la cantidad de torres y columna a medida que agrego torres.

En este ejemplo, vamos a ubicar las torres de la columna 1 a la 8 consecutivamente, la primer torre puede escoger cualquiera de las 8 columnas, la segunda torre, en cambio va a contar con 7 columnas a elegir, obviamente ocupando otra fila. Es decir que para la n-torre voy a tener 8-n columnas a elegir.

Entonces por principio principio multiplicativos tenemos que :

$$
8 \cdot 7 \cdot 6 \cdot 5 \cdot 4 \cdot 3 \cdot 2 \cdot 1 = 40320
$$

40320 serian las formas de ubicar las torres sin que se amenacen

### **b)**

Ahora que se nos pide tener en cuenta el color de las torres, sabemos que 40320 es la cantidad de formas que podemos ubicar las torres sin que se amenacen entre si, ahora habría que calcular los ordenamientos que se pueden formar intercambiando las torres de posición entre ellas, notar que están ordenadas en hilera pero a distinta altura debido a que ocupan distintas filas.

Entonces por teorema de permutación tenemos que las 8 permutaciones de las 8 torres de color es $8!$

Notar que para cada uno de estos ordenamientos seguimos contando con todas las distribuciones de torres para que no se amenacen entre sí, entonces el resultado de lo pedido en el enunciado es $40320 \cdot 8!$
