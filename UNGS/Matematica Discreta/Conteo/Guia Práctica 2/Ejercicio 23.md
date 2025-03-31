---
tags:
  - Ecuación-Linear
status: Done
---

## Halle la Cantidad De Soluciones En Los Enteros no Negativos De

$$
x_1 + x_2 + x_3 + x_4 + x_5 = 50
$$

tales que:

**a)** $x_5 \gt 12$

**b)** $x_4 \ge 7 \text{ y } x_5 \gt 12.$

**Respuesta**

### **a)**

Teniendo en cuenta la restricción definimos la siguiente variable:

$$
Y = x_5 - 13 \Rightarrow Y \ge 0
$$

Entonces reescribimos la ecuación inicial:

$$  
\begin{aligned}
x_1 + x_2 + x_3 + x_4 + (Y + 13) &= 50\\
x_1 + x_2 + x_3 + x_4 + Y + 13  &= 50\\
x_1 + x_2 + x_3 + x_4 + Y  &= 37\\
\end{aligned}
$$

Entonces la cantidad de soluciones de la ecuación en los enteros no negativas, por *teorema 2* sabemos que es $C(41,4)$

**b)**

Teniendo en cuenta la restricción definimos la siguiente variable:

$$  
\begin{aligned}
Y &= x_4 - 7 \Rightarrow Y \ge 0\\
Z &= x_5 - 13 \Rightarrow Z \ge 0
\end{aligned}
$$ 

Entonces reescribimos la ecuación inicial:

$$  
\begin{aligned}
x_1 + x_2 + x_3 + (Y + 7) + (Z + 13) &= 50\\
x_1 + x_2 + x_3 + Y + Z + 7 + 13 &= 50\\
x_1 + x_2 + x_3 + Y + Z + 20 &= 50\\
x_1 + x_2 + x_3 + Y + Z &= 30\\
\end{aligned}
$$

Entonces la cantidad de soluciones de la ecuación en los enteros no negativas, por *teorema 2* sabemos que es $C(34,4)$
