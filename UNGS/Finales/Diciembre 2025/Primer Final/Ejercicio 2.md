---
tags:
  - Ecuación-Linear
---

Cierta caja musical tiene una pieza circular con 20 espacios a lo largo de su borde donde se pueden colgar campanitas elegidas entre 4 tipos distintos. Suponiendo que al menos un espacio no debe quedar vacío, que hay suficientes campanitas para que las 20 sean del mismo tipo y que las campanitas del mismo tipo son indistinguibles.

(a) ¿De cuántas formas distintas se pueden elegir las campanitas sin considerar como se ubicarán en la pieza circular?

(b) En una elección al azar se tomaron 3 campanitas del tipo uno, 3 del tipo dos, 5 del tipo tres y 4 del tipo cuatro. ¿De cuántas formas distintas se pueden ubicar estas campanitas en el borde de la pieza circular con la condición de que las campanitas del tipo 1 estén todas juntas, las del tipo 2 estén todas juntas y no haya dos espacios vacíos consecutivos?

**Respuestas**

## A -

Se puede resolver contando las posibles formas de resolver una ecuación linear con coeficientes unitarios, o sinó usando el teorema de combinaciones con elementos repetidos.

Definamos las siguientes propiedades:

$$\begin{aligned}
x_1 = \text{Campanitas de tipo 1}\\
x_2 = \text{Campanitas de tipo 2}\\
x_3 = \text{Campanitas de tipo 3}\\
x_4 = \text{Campanitas de tipo 4}\\
\end{aligned}
$$ 

Observemos que el problema se resuelve a obtener la cantidad de soluciones a la siguiente ecuación en $\mathbb{Z} \ge 0$:

$$x_1 + x_2 + x_3 + x_4 = 20$$

Luego la cantidad de formas de solucionar esa ecuación en $\mathbb{Z} \ge 0$, usando el teorema de ecuaciones lineares con coeficientes unitarios es igual a $\begin{pmatrix}23 \\ 3 \end{pmatrix}$, esto equivale a la cantidad de formas de seleccionar las 20 piezas sin tener en cuenta como serán ubicadas en la pieza

---
## B -

Problema de permutaciones circulares con elementos repetidos, creo que para contar los ordenamientos necesitamos un elemento que sea único, que va a actuar como punto de referencia, en este caso no tenemos un elemento que sea de una clase única, tenemos 15 campanitas y 5 espacios.

Debido a que necesitamos que las campanas del tipo estén todas juntas, vamos a asignar las 3 campanas a la variable $X$, y las 3 campanas del tipo dos a la variable $Y$, luego tenemos que calcular las formas de distribuir circularmente los elementos del siguiente multi conjunto:

$$ \{ 1 \cdot X, 1 \cdot Y, 5 \cdot \text{tipo tres}, 4 \cdot \text{tipo cuatro} \} $$

tenemos que distribuir 11 elementos en 16 espacios disponibles (originalmente eran 20, pero $X$ e $Y$ usan 3 espacios cada uno, ya que se le asignaron 3 campanas a cada variable)
