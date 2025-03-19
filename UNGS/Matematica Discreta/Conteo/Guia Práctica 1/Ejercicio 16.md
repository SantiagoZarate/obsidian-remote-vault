## En Una Empresa Trabajan 8 Hombres Y 12 Mujeres

**a)** ¿De cuántas formas se puede elegir una delegación de cinco empleados?
**b)** ¿De cuántas formas si debe estar formada por dos hombres y tres mujeres?

**a)**

Sea el conjunto $S$ cuyos elementos son las formas de armar una delegación de cinco empleados con los trabajadores mencionados en el enunciados.

Lo pedido en el ejercicio se resuelve obteniendo $|S|$, para ello necesitamos seleccionar de formas distintas 5 empleados de los 20 disponibles, lo que es igual a $C(20,5)$

**b)**

En esta ocasión necesitamos que la cantidad de empleados por género sean constantes en todas las delegaciones posibles, sea $M$ el conjunto cuyos elementos satisfacen lo pedido en el enunciado.

Para los hombres necesitamos seleccionar 2 de los 8 disponibles, lo que es igual a $C(8,2)$

Para las mujeres necesitamos seleccionar 3 de las 12 disponibles, lo que es igual a $C(12,3)$

Notar que para cada una de las secciones de hombres vamos a contar con todas las selecciones de mujeres, por lo que por principio multiplicativo tenemos que:

$$
|M| = C(8,2) \cdot C(12,3)
$$
