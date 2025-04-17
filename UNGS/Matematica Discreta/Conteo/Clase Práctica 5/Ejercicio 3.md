## Cinco Amigos Se Reúnen a Cenar En Un Restaurante Y Encargan Cinco Platos Diferentes. Al Tiempo, Concurren Nuevamente Al Mismo Lugar, Y Habiendo Quedado Muy Conformes Deciden Ordenar Los Mismo Platos, Pero De Manera Que Ninguno De Ellos Repita la Comida Anterior ¿De Cuántas Maneras Puede Hacerse la Nueva Elección?

**Respuesta**

Declaramos las siguientes variables

$$  
\begin{aligned}
a &= \text{Cantidad de platos 1}\\
b &= \text{Cantidad de platos 2}\\
c &= \text{Cantidad de platos 3}\\
d &= \text{Cantidad de platos 4}\\
e &= \text{Cantidad de platos 5}\\
\end{aligned}
$$

El problema se resume a encontrar la cantidad de soluciones a esta ecuación:

$$ a + b + c + d + e = 5 $$

con las siguientes restricciones:

$$  
\begin{aligned}
0 \le a \le 4\\
0 \le b \le 4\\
0 \le c \le 4\\
0 \le d \le 4\\
0 \le e \le 4\\
\end{aligned}
$$

La cota superior es 4 debido a que al tener 5 platos distintos, debemos restar uno, ya que no se puede repetir el plato que se pidió por primera vez

Para cada uno de las personas tenemos 4 posibles platos (en total tenemos 5, pero restamos el que eligió la vez pasada), por lo tanto por principio multiplicativo tenemos que:

$$ 4^5 $$

Equivale a la cantidad de formas de hacer esta nueva elección

De los 5 platos, por persona necesitamos contar las formas de permutar los platos a elegirlos, lo que equivale a $P(5,4)$
