## ¿Cuántas Soluciones En Los Enteros Positivos Tiene $7 \le x_1 + x_2 + x_3 \gt 9$ Si Además Requerimos Que $x_1 \ge 4$?

**Respuesta**

$$
x_1 + x_2 + x_3 
$$

El resultado tiene que ser mayor igual a 7 y tiene que ser menos de 9

Podemos plantear la siguientes dos ecuaciones:

$$  
\begin{aligned}
a: x_1 + x_2 + x_3  &= 7\\
b: x_1 + x_2 + x_3  &= 8\\
\end{aligned}
$$

Para resolver $a$, teniendo en cuenta la restricción del enunciado, definimos la siguiente variable

$$
Y = x_1 - 3 \Rightarrow Y \ge 1
$$

Reescribimos $a$ usando la nueva variable:

$$  
\begin{aligned}
(Y + 3) + x_2 + x_3 &= 7 \\
Y + x_2 + x_3 + 3 &= 7 \\
Y + x_2 + x_3 &= 4 \\
\end{aligned}
$$

Entonces la cantidad de soluciones para esa ecuación en los enteros positivos, por *teorema 1* sabemos que es $C(3, 3)$

Ahora sigamos con la resolución de $b$, usamos la misma variable $Y$ ya definida y reescribimos la ecuación

$$  
\begin{aligned}
(Y + 3) + x_2 + x_3 &= 8 \\
Y + x_2 + x_3 + 3 &= 8 \\
Y + x_2 + x_3 &= 5 \\
\end{aligned}
$$

Entonces la cantidad de soluciones para esa ecuación en los enteros positivos, por *teorema 1* sabemos que es $C(4, 3)$

Ahora que tenemos la cantidad de soluciones para $a$ y $b$, la cantidad de soluciones a lo que pide el enunciado es C(3,3) + C(4,3)
