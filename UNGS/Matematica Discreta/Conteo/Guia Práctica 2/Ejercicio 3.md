---
tags:
  - Permutación-Repetidos
status: Done
---

## Un Hombre Trabaja En Un Edificio Localizado a Doce Cuadras Al Este Y Cinco Cuadras Al Norte De Su Casa. Así, Cuando Va a Trabajar Caminando, Recorre 17 Cuadras

**a)** ¿De cuántas formas distintas puede el hombre ir de su casa al trabajo caminando exactamente 17 cuadras?

**b)** ¿De cuántas formas distintas puede el hombre ir de su casa al trabajo caminando exactamente 17 cuadras si además no quiere caminar dos cuadras seguidas hacia el norte?

**Respuesta**

### **a)**

Observemos que el hombre puede salir de la casa y hacer las 5 cuadras hacia el norte y luego las 12 cuadras al este, o primero las 12 cuadras al este y luego las 5 al norte, es decir, el orden en que recorre las cuadras no importa.

Usaremos la siguiente definición para resolver el problema:

$$  
\begin{aligned}
X &= \text{Movimiento hacia el este}\\
Y &= \text{Movimiento hacia el norte}
\end{aligned}
$$

Podemos representar las cuadras que recorre el hombre formando una palabra conteniendo 12 $X$ y 5 $Y$.

Contamos con el siguiente multiconjunto $S$:

$$
\{ 12 \cdot X, 5 \cdot Y  \}
$$

Notar que cualquier ordenamiento de los elementos de $S$ representaría una forma en la que el hombre llegue al trabajo, por lo que necesitamos contar los ordenamientos de $S$, teniendo en cuenta que tiene 2 tipos de elementos, necesitamos el número de permutaciones de los 17 elementos, lo que por *teorema 2* es:

$$
\frac{17!}{5!\cdot12!}
$$
### **b)**

De manera análoga al análisis anterior, el ordenamiento de la palabra que representa el recorrido del hombre no puede tener dos $Y$ contiguas

Sea $P$ el conjunto cuyos elementos son las palabras que se formas con las letras del multiconjunto $S$ del punto anterior, definimos $M\subset P$ cuyos elementos son las palabras sin tener dos Y contiguas.

Notemos que tenemos 12 letras X, por lo tanto tenemos 13 espacios entre ellas, necesitamos seleccionar 5 espacios para que sean ocupados por letras Y, de esta forma nos aseguramos que no estás contiguas, eso es igual a $C(13,5)$

> [!NOTE] Otra forma de redactarlo
> "Notemos que tenemos 12 letras $X$, por lo tanto tenemos 13 espacios entre ellas (incluyendo los extremos). Necesitamos seleccionar 5 de esos 13 espacios para colocar las letras $Y$, de modo que no queden contiguas. Eso equivale a:


Entonces la cantidad de formar de hacer el recorrido según el enunciado es $C(13,5)$
