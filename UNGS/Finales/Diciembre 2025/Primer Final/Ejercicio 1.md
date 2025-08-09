Una fábrica tiene tres lineas de empaquetado de productos. Las dos primeras usan cajas de dos colores posibles, rojo y azul, y la última usa de 3 colores posibles, rojo, azul y verde.

Además, en ocasiones se le agrega a la caja un cupón de descuento. Todos las cajas tienen la posibilidad de tener el cupón de descuento independientemente de las otras. Suponiendo que por hora se empaquetan 36 productos, 12 productos por linea.

(a) ¿Cuántas combinaciones posibles hay para los colores de las 36 cajas que se empaquetaron en una hora con la condición de que en cada linea al menos una caja tenga un cupón?

(b) ¿Cuántas horas deben transcurrir como mínimo para garantizar que al menos cuatro veces se obtenga la misma distribución?

**Respuestas**

## A-

Comencemos calculando la cantidad de posibles combinaciones de empaquetar los productos por linea.

En la primer linea, cada producto tiene 4 posibles formas de estar empaquetado.

- Color rojo con cupón de descuento
- Color rojo sin cupón de descuento
- Color azul con cupón de descuento
- Color azul sin cupón de descuento

por principio multiplicativo, tenemos que hay $4^{12}$ formas de empaquetar los productos de la linea 1, para la linea 2 es la misma cantidad ya que tienen las mismas restricciones.

Para la linea 3, siguiendo un razonamiento análogo al de la linea 1, cada producto tiene 6 posibles formas de ser empaquetado, luego por principio multiplicativo tenemos que $6^{12}$ son las formas de empaquetar los productos de la linea 3.

Luego las formas de empaquetar por linea es independiente una de otra, por lo tanto mediante principio multiplicativo tenemos que la cantidad de formas de empaquetar los 36 productos es igual a:

$$ 4^{12} \cdot 4^{12} \cdot 6^{12} $$

me estoy dando cuenta que esto no response lo preguntado en el enunciado.

pensándolo mejor, me sirve, porque ya calcule todas las formas de combinar los empaquetados, ahora puedo calcular los casos en donde NO HAYA NINGÚN cupón, y después usando el principio de sustracción puedo obtener las combinaciones en donde haya al menos un cupón por linea.

podría resolverlo usando el principio I-E

---

Sea $S$ el conjunto cuyos elementos son las formas de empaquetar los 36 productos teniendo en cuenta las restricciones del enunciado, definimos las siguientes propiedades.

$$  
\begin{aligned}
P_1 = \text{La linea 1 no tiene cupones de descuento}\\
P_2 = \text{La linea 2 no tiene cupones de descuento}\\
P_3 = \text{La linea 3 no tiene cupones de descuento}\\
\end{aligned}
$$

Definimos los subconjuntos $A_i$ de $S$ tal que los elementos de $A_i$ con $i \le i \le 3$ satisfacen la propiedad $P_i$, resolver lo pedido en el enunciado se resume a calcular el cardinal del conjunto $\overline{A_1} \cap \overline{A_2} \cap \overline{A_3}$, para ello vamos a usar el principio I-E para tres propiedades.

$$\begin{aligned}
|\overline{A_1} \cap \overline{A_2} \cap \overline{A_3}| = |S|
- |A_1| - |A_2| - |A_3|
+ |A_1 \cap A_2| + |A_1 \cap A_3| + |A_2 \cap A_3|
\\- |A_1 \cap A_2 \cap A_3|

\end{aligned}
$$ 

Pasemos a calcular los cardinales de cada conjunto.

- $|S|$ = $4^{12} \cdot 4^{12} \cdot 6^{12}$ , ya lo calculé al principio
- $|A_1|$ = Necesitamos calcular la cantidad de combinaciones de empaquetados tal que los productos de la linea 1 no pueden tener cupones de descuento, entonces, cada uno de los 12 productos tiene 2 posibles formas de empaquetarse, independientemente de como se empaqueten, para la linea 2 tenemos $4^{12}$ maneras de empaquetar los productos, y para la linea 3 tenemos $6^{12}$ maneras, por pcio. multiplicativo tenemos que la cantidad de formas de empaquetar los 36 productos de manera tal que la linea 1 no tenga cupones es:
  $$ 2^{12} \cdot 4^{12} \cdot 6^{12}$$
- $|A_2| =  2^{12} \cdot 4^{12} \cdot 6^{12}$, se cumplen las mismas condiciones que en el calculo de $|A_1|$
- $|A_3|$ = De manera análoga al razonamiento anterior, cada uno de los productos de la linea 3 tiene 3 posibles formas de empaquetarse (rojo, verde y azul), por principio multiplicativo tenemos $3^{12}$ formas de empaquetar los 12 productos de la linea 3, luego para las lineas 1 y 2 tenemos $4^{12}$ formas de empaquetar los productos, por principio multiplicativo tenemos que la cantidad de formas de empaquetar los 36 productos sin tener cupones en la linea 3 es igual a:
  $$ 4^{12} \cdot 4^{12} \cdot 3^{12}$$
- $|A_1 \cap A_2|$ = Tenemos que contar la cantidad de formas de empaquetar los 36 productos de forma tal que en la linea 1 y 2 no hayan cupones, siguiendo el razonamiento de puntos anteriores tenemos que esa cantidad es igual a:

  $$ 2^{12} \cdot 2^{12} \cdot 6^{12}$$

- $|A_1 \cap A_3| y |A_2 \cap A_3|$ = $2^{12} \cdot 4^{12} \cdot 3^{12}$
- $|A_1 \cap A_2 \cap A_3|$ = $2^{12} \cdot 2^{12} \cdot 3^{12}$

Ahora tenemos que reemplazar los cardinales en la expresioón del principio I-E para tres propiedades.
