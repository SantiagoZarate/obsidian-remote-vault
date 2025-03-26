---
tags:
  - Permutación-Repetidos
status: Done
---

## Considere Un Paralelepípedo Imaginario De 4 Unidades De Frente, 5 Unidades De Profundidad Y 6 Unidades De Alto. Una Rana Se Encuentra Ubicada En El Vértice Inferior Izquierda De la Cara Frontal Del Paralelepípedo Y Desea Llegar Al Vértice Ubicado 4 Unidades a la Derecha, 5 Unidades Atrás Y 6 Unidades Arriba. ¿Cuántos Caminos Puede Recorrer la Rana Si Sólo Puede Dar Saltos De Una Unidad Hacia la Derecha, O Hacia Atrás, O Hacia Arriba? Ejemplo: Uno De Los Posibles Caminos Que Puede Recorrer la Rana Es Dar 2 Saltos Hacia Arriba, Seguido Por 2 Saltos a la Derecha, Seguido De 5 Hacia Atrás, Otros 4 Saltos Hacia Arriba Y Finalmente 2 Saltos Hacia la Derecha

**Respuesta**

Observemos que podemos representar cada uno de los movimientos de la siguiente manera:

$$  
\begin{aligned}
X &= \text{Movimientos hacia la derecha}\\
Y &= \text{Movimientos hacia arriba}\\
Z &= \text{Movimientos hacia atra}\\
\end{aligned}
$$

Notar que la rana, no puede deshacer sus movimientos, es decir, si se mueve hacia la derecha no puede moverse a la izquierda, si se mueve arriba no puede moverse abajo, es decir, que la cantidad de movimientos en cada eje esta limitado al tamaño del paralelepípedo, así que podemos representar el camino con una palabra formado por las siguientes letras:

$$
\underline{XXXX}\,\underline{YYYYYY}\,\underline{ZZZZZ}
$$

Notar que dos caminos se consideran distintos si el orden de los movimientos es diferente, entonces el problema se resume a contar los ordenamientos en hilera de un conjunto con elementos repetidos, por *teorema* sabemos que eso es igual a:

$$
\frac{15!}{4!\cdot6!\cdot5!}
$$

Esto equivale a la cantidad de caminos que puede recorrer la rana para llegar a donde se pide en el enunciado.
