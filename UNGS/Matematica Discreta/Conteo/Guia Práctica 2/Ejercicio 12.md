---
status: TODO
---

Se tiene una ruleta de diez lugares, donde en cada lugar hay un premio. Los premios de la ruleta son elegidos de la siguiente forma:

- 5 son distintos y elegidos del conjunto {1, 2, 3, 4, 5, 6, 7}, donde cada número representa millones de pesos.
- 5 son elegidos del conjunto {Parlante, Auriculares, Teclado, Mouse}

**a)** ¿Cuántas configuraciones distintas de la ruleta se pueden hacer?

**b)** ¿Cuántas configuraciones distintas de la ruleta se pueden hacer con la condición de que los 5 premios en dinero estén todos separados y ordenados de menor a mayor en sentido horario?

**Respuesta**

## **a)**

Sea $S$ el conjunto cuyos elementos son las configuraciones de la ruleta teniendo en cuenta las restricciones del enunciado, resolver el ejercicio se resume a calcular $|S|$.

Para ello veamos que para 5 de los 10 espacios, necesitamos escoger 5 números distintos del conjunto {1, 2, 3, 4, 5, 6, 7}, lo que es igual a C(7,5).

Para los restantes 5 espacios necesitamos seleccionar 5 elementos del conjunto {Parlante, Auriculares, Teclado, Mouse}, esto se puede traducir a cantar la cantidad de soluciones en $\mathbb{Z} \ge 0$ de la ecuación linear con coeficientes unitarios.

$$
X_1 + X_2 + X_3 + X_4 = 5
$$

Donde definimos las siguientes variables

$$  
\begin{aligned}
X_1 &= \text{Cantidad de Parlante}\\
X_2 &= \text{Cantidad de Auriculares}\\
X_3 &= \text{Cantidad de Teclado}\\
X_4 &= \text{Cantidad de Mouse}\\
\end{aligned}
$$

Por *teorema 2* sabemos que la cantidad de soluciones para esta ecuación es:

$$
\frac{5 + 4 - 1}{ 4 -1} = \frac{8}{3}
$$

Ahora que ya seleccionamos los 10 elementos que van a ocupar los 10 espacios de la ruleta hay que contar las permutaciones circulares, fijamos uno de los números que elegimos al principio ya que son todos distintos, por lo que nos quedan 9 espacios, por permutación sabemos que es 9!

Finalmente tenemos que por cada una de las selecciones de los 5 números, tenemos $\frac{8}{3}$ selecciones de premios tecnológicos, que pueden ser permutados 9! veces, por principio multiplicativo tenemos que:

$$
|S| = C(7,5) \cdot \frac{8}{3} \cdot 9!
$$

==TODO: REVISAR LA ULTIMA PARTE==
