---
tags:
  - Ecuación-Linear
status: Done
---

## ¿Cuántas Soluciones En Los Naturales Mayores Que 7 Tiene la Ecuación

$$
x_1 + x_2 + x_3 + x_4 = 45?
$$
**Respuesta**

Teniendo en cuenta la restricción de que las variables tienen que ser mayores a 7, definimos las siguientes variables.

$$  
\begin{aligned}
A_1 &= x_1 - 8 \Rightarrow A_1 \ge 0 \\
A_2 &= x_2 - 8 \Rightarrow A_2 \ge 0 \\
A_3 &= x_3 - 8 \Rightarrow A_3 \ge 0 \\
A_4 &= x_4 - 8 \Rightarrow A_4 \ge 0 \\
\end{aligned}
$$

Podemos reescribir la ecuación original de esta forma

$$  
\begin{aligned}
(A_1 + 8) + (A_2 + 8) + (A_3 + 8) + (A_4 + 8) &= 45\\
A_1 + A_2 + A_3 +A_4 + 8 + 8 + 8 + 8 &= 45\\
A_1 + A_2 + A_3 +A_4 + 32 &= 45\\
A_1 + A_2 + A_3 +A_4 &= 12\\
\end{aligned}
$$

Entonces el problema se trasladar a encontrar la cantidad de soluciones a la siguiente ecuación en los naturales no negativos:

$$
A_1 + A_2 + A_3 +A_4 = 12
$$

Por *teorema 2* sabemos que esto es $C(15,3)$
