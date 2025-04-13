Una compañía almacena productos y la numeración de las cajas en el almacén viene especificado por el número de pasillo, seguido de la localización en el pasillo y finalmente el numero de la estantería. Hay un total de 50 pasillos, 85 armarios en cada pasillo y 5 estanterías en cada armario. Demostrar que si la compañía tiene 63760 productos habrá al menos 4 productos con una misma identificación

**Respuesta**

Primero calculemos la cantidad de lugares para almacenar productos tenemos, eso es igual a

$$
50 \cdot 85 \cdot 5  = 21250
$$

Entonces contamos con 21250 cajas o espacios donde ubicar los productos

- Cantidad de espacios: **Palomares**
- Cantidad de productos: **Palomas**

Entonces usando la fórmula del teorema podemos saber la cantidad de palomas necesarias para que se cumpla la condición en la que al menos un palomar tiene al menos 4 palomas.

$$
n(r - 1) + 1
$$
$$  
\begin{aligned}
21250\cdot(r - 1) + 1 &= 63751\\
\end{aligned}
$$

Luego sabemos que la cantidad mínima de palomas que necesitamos para que se cumpla le condición es 63751 y $63751 \ge 63760$, por lo lo tanto queda justificado que van a haber al menos 4 productos con la misma identificación
