## 1. En la Casa De Juan Hay 10 Libros Distintos

**a)** ¿De cuántas Formas Distintas Puede Guardar Juan Los 10 Libros Si Dispone De Una Caja Roja, Una Verde Y Una Azul, Todas Ellas Con Capacidad Para Guardar Todos Los Libros?
**b)** ¿De cuántas Formas Distintas Puede Juan Ordenar Los 10 Libros En Dos Estantes De Su Biblioteca Si Cada Estante Tiene Capacidad Para Los Diez Libros?
**c)** ¿De cuántas Formas Distintas Puede Juan Ubicar Los Libros En Dos Estantes Si En El Primero De Ellos Debe Colocar 7 Libros Y En El Segundo Los Restantes?

**Respuesta**

### **a)**

Sea el conjunto $L$ cuyos elementos son los 10 libros, definimos $S$ el conjunto cuyos elementos son las distintas maneras de guardar los elementos de $L$ en alguna de las 3 cajas. Lo pedido en el enunciado se resuelve calculando $|S|$

Por cada uno de los elementos de $L$ contamos con 3 opciones donde guardarlo, y sin importar cual elijamos, para el siguiente elemento seguimos contando con las mismas opciones ya que las cajas tienen capacidad suficiente, así que por principio multiplicativo es:

$$  
\begin{aligned}
3 \cdot 3 \cdot 3 ... = 3^{10}
\end{aligned}
$$

Entonces las formas distintas para ordenar los 10 libros es $3^{10}$

### **b)**

Seguimos utilizando el conjunto $L$ y definimos el conjunto $M$ cuyos elementos son las formas en que se pueden guardar los elementos de $L$ en 2 estanterías.

Definimos los siguientes subconjuntos de $M$

$$  
\begin{aligned}
N_1 &= \text{Elementos con 10 libros en la 1er estanteria y 0 en la 2da}\\
N_2 &= \text{Elementos con 9 libros en la 1er estanteria y 1 en la 2da}\\
N_3 &= \text{Elementos con 8 libros en la 1er estanteria y 2 en la 2da}\\
N_4 &= \text{Elementos con 7 libros en la 1er estanteria y 3 en la 2da}\\
N_5 &= \text{Elementos con 6 libros en la 1er estanteria y 4 en la 2da}\\
N_6 &= \text{Elementos con 5 libros en la 1er estanteria y 5 en la 2da}\\
\end{aligned}
$$

Para calcular $|N_1$ nos interesa contar los ordenamientos de 10 elementos de $L$ para la primer estantería y para uno de los casos se le asignan la cantidad de ordenamientos de 0 elementos de $L$ para la segunda estantería. entonces usando le función de permutación y el principio multiplicativo nos queda la siguiente cuenta

$$|N_1| = P(10,10) \cdot P(10,0)$$

Por definición de $P(n,r)$, Notar que $P(10,0) = 1$, ya que $r = 0$

Se usa el mismo análisis para los restantes subconjuntos de $M$

$$  
\begin{aligned}
|N_2| &= P(10,9) \cdot P(10,1)\\
|N_3| &= P(10,8) \cdot P(10,2)\\
|N_4| &= P(10,7) \cdot P(10,3)\\
|N_5| &= P(10,6) \cdot P(10,4)\\
|N_6| &= P(10,5) \cdot P(10,5)\\
\end{aligned}
$$ 

Definimos $\overline{N_1}$ y por definición de complemento es el conjunto cuyos elementos son los ordenamientos con 0 libros en la 1er estantería y 10 en la 2da, el calculo de $|\overline{N_1}|$ es el mismo al de $|N_1|$.

Esto mismo razonamiento se puede aplicar a los subconjuntos ${N_2}$, $N_3$, $N4$ y $N_5$, de esta manera obtenemos el cardinal de los ordenamientos posibles.

entonces el calculo para obtener $|M|$ es:

$$
\begin{aligned}
|M| = \\
(
P(10,9) \cdot P(10,1) +
P(10,8) \cdot P(10,2) +
P(10,7) \cdot P(10,3) +
P(10,6) \cdot P(10,4)
) \cdot 2 \\+
P(10,5) \cdot P(10,5)
\end{aligned}
$$

### **c)**

Lo pedido en la consigna esta respondido haciendo el calculo de $|N_4|$ que es $P(10,7) \cdot P(10,3)$, esto lo sabemos por el análisis del punto anterior
