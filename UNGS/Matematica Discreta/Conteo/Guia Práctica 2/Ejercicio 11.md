## Un Joyero Fábrica Anillos En Cuya Cara Exterior Tienen Grabados 10 Símbolos, Cinco De Ellos Son Elegidos Entre Las 24 Letras Del Alfabeto Griego Y Los Otros Cinco Entre Los Enteros Del 1 Al 100

**a)** Suponiendo que las letras y los números no se pueden repetir, ¿cuántos anillos distintos se pueden producir?

**b)** Suponiendo que las letras no se pueden repetir, ¿cuántos anillos distintos se pueden producir?

**c)** Suponiendo que las letras no se pueden repetir, ¿cuántos anillos distintos se pueden producir con los impares juntos y los pares juntos?

### **a)**

Sea $S$ el conjunto cuyos elementos son las formas de producir anillos, lo pedido en el enunciado se resuelve obteniendo $|S|$, para ello notemos que para cada una de las formas de elegir los primeros 5 símbolos, tenemos todas las formas de elegir los restantes 5 símbolos, por principio multiplicativo tenemos que:

$$
|S| = \text{Formas de elegir los primeros 5 símbolos} \cdot  \text{Formas de elegir los restantes símbolos} 
$$

Para los primeros 5 símbolos, tenemos que seleccionar 5 letras de un total de 24 letras disponibles, lo que equivale a $C(24,5)$, para los restantes 5 símbolos tenemos que elegir 5 enteros entre el 1 al 100, lo que es igual a $C(100,5)$.

Entonces calculamos el cardinal de $S$:

$$  
\begin{aligned}
|S| = C(24,5) \cdot C(100,5)
\end{aligned}
$$
### **b)**

Con esta nueva suposición, la cantidad de formas de elegir las 5 letras de un grupo de 24 permanece como $C(24,5)$, pero la forma de elegir los 5 números de un grupo de 100 es igual a $100^5$, por principio multiplicativo tenemos que

$$
C(24,5) \cdot 100^5
$$

equivale a la cantidad de formas de producir anillos con letras sin repetirse

### **c)**

==TODO==
