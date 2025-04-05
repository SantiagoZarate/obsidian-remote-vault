## La Pizzería De Los Hermanos Mario Ofrece Su Pizza Especial Que Es Una Pizza Redonda Dividida En 8 Porciones Iguales, Cada Porción De Un Gusto Diferente (muzzarella, Provolone, Panceta, Morrones, Calabresa, Rúcula, Huevo Duro Y ananá)

**a)** ¿De cuántas maneras diferentes pueden estar ordenadas las 8 porciones en la pizza especial?

**b)** ¿De cuántas maneras diferentes pueden estar ordenadas las 8 porciones en la pizza especial si se quiere que la porción de provolone esté junto a la de ananá y que la porción de huevo duro esté junto a la de panceta?

**Respuesta**

### **a)**

Observar que si ponemos a las pizzas en orden secuencial, la cantidad de formas de ordenar los 8 gustos sería $8!$, pero al tener un orden circular cada 8 ordenamientos lineares estaríamos repitiendo un ordenamiento circular, así que la cantidad de formas diferentes de ordenar las 8 porciones es

$$
\frac{1}{8} \cdot 8!
$$
### **b)**

Observemos que podemos definir las siguientes variables:

$$  
\begin{aligned}
X &= \text{Los gustos ananá y provolone juntos}\\
Y &= \text{Los gustos huevo duro y panceta juntos}\\
\end{aligned}
$$

La cantidad de ordenamientos lineares de los 4 gustos restantes, mas X e Y es igual a $6!$, por cada uno de estos ordenamientos hay que tener en cuenta los ordenamientos de $X$ e $Y$, así que por principio multiplicativo es:

$$
6! \cdot 2! \cdot 2!
$$

Tener en cuenta que esa es la cantidad de ordenamientos lineares, pero al tener una situación donde el ordenamiento es circular, cada 6 ordenamientos lineares tenemos un nuevo ordenamiento circular. Así que la cantidad de formar de ordenar los gustos de la pizza según el enunciado es:

$$
\frac{1}{6} \cdot 6! \cdot 2! \cdot 2!
$$
