## Todos Los Martes Y Jueves 50 Estudiantes Cursan En Un Aula Que Tiene 75 Sillas Ordenadas En 5 Filas De 15 Sillas Cada Una

**a)** ¿De cuántas formas distintas se pueden sentar los 50 estudiantes en las 75 sillas?

**b)** Suponiendo que siempre asisten los 50 estudiantes, ¿cuál es la mínima cantidad de clases que deben pasar para garantizar que al menos 3 veces se sienten de la misma forma?

**Respuesta**

### **a)**

De las 75 sillas disponibles necesitamos seleccionar 50 que posteriormente se asignaran a cada una de las personas, la cantidad de formas de hacer esa selección es $\begin{pmatrix} 75 \\ 50 \end{pmatrix}$ , para cada uno de estos seleccionamientos tenemos que contar las permutaciones de personas, por principio multiplicativo tenemos que

$$\begin{pmatrix} 75 \\ 50 \end{pmatrix} \cdot 50! $$

Esto equivale a la cantidad de formas en las que los estudiantes pueden sentarse.

### **b)**

Observemos que en el enunciado se nos pide buscar la cantidad mínima de clases para asegurar cierta condición, por lo cual vamos a tener que hacer uso del principio del palomar, según el teorema 2, tenemos la siguiente formula que nos indica la cantidad mínima de palomas para asegurar la condición que haya $r$ palomas en al menos un palomar:

$$ n\cdot (r - 1) + 1  $$

En este caso reemplazamos las variables:

$$
\begin{pmatrix} 75 \\ 50 \end{pmatrix} \cdot 50! \cdot (3 - 1) + 1
$$

Esto equivale a la cantidad de clases necesarias para que al menos tres veces se hayan formado las mismas asignaciones de asientos.
