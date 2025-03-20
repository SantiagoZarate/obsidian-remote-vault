---
tags:
  - Permutación-Circular
  - Multiplicidad
status: Done
---

## ¿De Cuántas Maneras Se Pueden Sentar Cuatro Mujeres Y Cuatro Varones En Una Mesa Redonda De Forma Tal Que Dos Hombres no Se Sienten En Sillas Adyacentes?

**Respuesta**

*Sin usar principio de sustracción, usando un segundo enfoque aprendido en clase*

Supongamos que de los dos hombres, dejamos a uno de ellos afuera de la consideración por el momento, llamemos $X$ al hombre que quedo en consideración e $Y$ al que quedo fuera.

Necesitamos contar el ordenamiento circular de 7 personas de un grupo de 7, por lo que por teorema 2 es igual $6!$, notemos que en cualquier ordenamiento circular de estos contamos con 7 espacios entre los integrantes de la mesa, ahora necesitamos incluir a $Y$, los espacios a la izquierda y derecha de $X$ no van a poder ser usados, por lo que nos quedan 5 espacios disponibles.

Entonces, independientemente de los ordenamientos que tengamos del grupo de 7 personas, vamos a tener 5 lugares donde ubicar a $Y$, por lo que las maneras de sentar al grupo de personas según lo pedido en el enunciado es:

$$
6! \cdot 5
$$
