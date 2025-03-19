## ¿Cuántos Números Enteros Entre 10.000 Y 100.000 Existen Tal Que Cada Uno De Sus Dígitos Es Un 6, Un 7 O Un 8? ¿Cuántos Entre 10.000 Y 100.000 Son Tales Que Cada Uno De Sus Dígitos Es Un 6, Un 7, Un 8 O Un 0? #Multiplicidad 

**Respuesta:**

Sea el conjunto S cuyos elementos son los números enteros entre 10.000 y 100.000 y que sus dígitos sean 6, 7 u 8, lo pedido en el ejercicio se obtiene calculando $|S|$, y para ello vamos a hacer el siguiente análisis.

Contamos con 5 posiciones para colocar los números, a pesar de el limite sea 100.000, no nos interesa la sexta posición ya que el menor de los números válidos, en este caso el 6, se excede si lo usamos en la posición de la centena de miles, por lo que queda descartado.

En cada posición tenemos 3 posibles candidatos, 6, 7 u 8, y para cada uno de los números elegidos para esta posición, contamos con la misma cantidad de posibilidades para las posteriores posiciones.

Así que por principio de multiplicidad tenemos que:
$$  
\begin{aligned}
|S| &= 3 \cdot 3 \cdot 3 \cdot 3\\
|S| &= 3⁴
\end{aligned}
$$
Para resolver lo pedido en la siguiente pregunta del enunciado el análisis es bastante parecido al anterior, definimos el conjunto S de la misma manera, solo que ahora los números están formados enteramente por 6, 7, 8 u 0. 

Contamos con las mismas 5 posiciones, pero en este caso la primer posición puede ser ocupada por 3 números, 6,7 u 8, el 0 se descarta porque el limite inferior empieza a partir de 10.000. Las demás posiciones tienen 4 posibles valores.

Sin importar que numero se elige para cada posición esto no condiciona las posibilidades de elección para las siguientes posiciones.

Así que por principio de multiplicidad tenemos que:
$$  
\begin{aligned}
|S| &= 3 \cdot 4 \cdot 4 \cdot 4\\
|S| &= 3 \cdot 4³
\end{aligned}
$$