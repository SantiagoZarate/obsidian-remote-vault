---
tags:
  - Ecuación-Linear
status: Done
---

## ¿En Cuántos De Los Números Entre 1 Y 1.000.000, Ambos Inclusive, la Suma De Sus Dígitos Es 6? ¿En Cuántos Es a Lo Sumo 6? ¿En Cuántos Es Al Menos 6?

**Respuesta**

Nuestra cota superior al ser 1.000.000, contamos con 7 dígitos, pero como la suma de los dígitos de dicha cota es 1 no lo vamos a tener en cuenta, así que tenemos hasta 6 dígitos.

Declaramos las siguientes variables:

$$  
\begin{aligned}
X_1 &= \text{Cantidad de unidades en las centena de miles}\\
X_2 &= \text{Cantidad de unidades en las decena de miles}\\
X_3 &= \text{Cantidad de unidades en los miles}\\
X_4 &= \text{Cantidad de unidades en los cienes}\\
X_5 &= \text{Cantidad de unidades en las decenas}\\
X_6 &= \text{Cantidad de unidades}\\
\end{aligned}
$$

Con las siguientes restricciones:

$$
x_1 \ge 0, x_2 \ge 0, x_3 \ge 0, x_4 \ge, x_5 \ge 0, x_6 \ge 0
$$

Entonces resolver lo pedido en el enunciado se resume a calcular la cantidad de soluciones que tiene la siguiente ecuación en los naturales no negativos.

$$
x_1 + x_2 + x_3 + x_4 + x_5 + x_6 = 6
$$

Por teorema sabemos que esto es igual a $C(11, 5)$
