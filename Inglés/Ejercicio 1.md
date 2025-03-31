## Una Embotelladora De Vinos Tiene 45 Cajas Del Mismo Vino Que Debe Repartir Entre Cinco Vinotecas De la Zona. Teniendo En Cuenta Los Requerimientos De Cada Cliente Para la Entrega De Esta Semana, la Embotelladora Debe Repartir Todas Las Cajas Sabiendo Que

- La vinoteca R&M tiene que recibir por lo menos 7 cajas
- La vinoteca Tintillo necesita recibir más de 12 cajas
- La vinoteca Momentos espirituosos tiene que recibir exactamente 9 cajas
- La vinoteca Trapiche Hnos como mínimo 6 cajas
- La vinoteca Tinto y Blanco hizo un pedido del vino pero no tiene apuro en recibir el mismo en esta entrega.

## ¿De Cuántas Formas Distintas Puede la Embotelladora Repartir Todas Las Cajas De Vino Entre Sus Cinco Clientes?

**Respuesta**

### Usando Ecuaciones Lineales Con Coeficiente Unitario

Representaremos a cada una de las cantidad de vinos por vinoteca con las siguientes variables:

$$  
\begin{aligned}
X_1 &= \text{Cantidad de vinos para la vinoteca RyM}\\
X_2 &= \text{Cantidad de vinos para la vinoteca Tintillo}\\
X_3 &= \text{Cantidad de vinos para la vinoteca Momentos Espirituosos}\\
X_4 &= \text{Cantidad de vinos para la vinoteca Trapiche Hnos}\\
X_5 &= \text{Cantidad de vinos para la vinoteca Tinto y Blando}\\
\end{aligned}
$$

Resolver lo pedido en el enunciado es igual a calcular la cantidad de soluciones de la siguiente ecuación:

$$
X_1 + X_2 + X_3 + X_4 + X_5 = 45
$$

Con las siguientes restricciones:

$$
X_1 \ge 7; X_2 \ge 13; X_3 = 9; X_4 \ge 6; X_5 \ge 0
$$

Notar que la variable $X_3$ tiene un valor constante 9, por lo que podemos prescindir de ella y plantear la siguiente ecuación.

$$
X_1 + X_2 + X_4 + X_5 = 36
$$

Teniendo en cuenta las restricciones de cada variables, hacemos los siguientes arreglos/desplazamientos:

$$
X_1 - 7 \ge 7; X_2 - 13 \ge 13;X_4 - 6\ge 6; 
$$

Luego redefinimos las variables:

$$  
\begin{aligned}
A &= X_1 - 7 \Rightarrow A \ge 0\\
B &= X_2 - 13 \Rightarrow B \ge 0\\
C &= X_4 - 6 \Rightarrow C \ge 0\\
D &= X_5 \Rightarrow D \ge 0\\
\end{aligned}
$$

Entonces reescribimos la ecuación con estas nuevas variables:

$$  
\begin{aligned}
(A + 7)+ (B + 13) + (C + 6) + D &= 36 \\
A + B + C + D + 26 &= 36 \\
A + B + C + D &= 10
\end{aligned}
$$

Entonces nos queda la siguiente ecuación:

$$

A + B + C + D = 10

$$

Por teorema 2 sabemos que la cantidad de soluciones para esta ecuación donde las variables forman parte de los enteros no negativos con coeficientes unitarios es $C(13, 3)$

---

### Usando Combinatoria Con Elementos Repetidos

Asignamos las cajas de vinos a las restricciones mínimas para cada vinoteca:

- R&M: 7 cajas
- Tintillo: 13 cajas
- Momentos espirituosos: 9 cajas
- Trapiche Hnos: 6 cajas
- Tinto y Blanco: 0 cajas

Entonces del total de 45 cajas, quedan 10 cajas por asignar, de las 5 vinotecas destino, hay una que ya no se le pueden asignar mas cajas, en concreto la vinoteca Momentos Espirituosos.

Entonces el problema se resume a seleccionar a que vinoteca del siguiente conjunto $\{ \text{RyM}, \text{Tintillo}, \text{Momentos espirituosos}, \text{Tinto y Blanco} \}$ se le puede asignar a alguna de las restantes 10 cajas.

Luego por teorema de combinación con elementos repetidos, sabemos que esa cantidad es $C(13, 3)$

Finalmente y respondiendo al enunciado, la cantidad de formas de repartir los vinos es $C(13,3)$
