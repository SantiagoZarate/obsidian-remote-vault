## Un Colectivo De Larga Distancia Parte De la Terminal Con 40 Pasajeros. El Recorrido Tiene 16 Paradas En Las Cuales Los Pasajeros Descienden, Pero Nadie Más Sube. ¿De Cuántas Formas Los Pasajeros Pueden Descender Si En Cada Parada Baja Al Menos Uno Y En la Parada 16 Se Vacía El Colectivo?

Nota: Importa el orden en que los pasajeros bajan en cada parada.

**Respuesta**

Definamos las variables $X_i$ con $1 \le i \le 16$ , donde cada variable representa la cantidad de pasajeros que bajan en la parada $i$, el problema se resume a contar las posibles soluciones en $\mathbb{N}$ de la siguiente ecuación:

$$
x_1 + x_2 + ... + x_{16} = 40
$$

haciendo uso del teorema 1 de ecuaciones lineares con coeficientes unitarios sabemos que la cantidad de soluciones es $\begin{pmatrix} 39 \\ 15 \end{pmatrix}$

> [!NOTE] Tip
> Falta ver como contar el orden de descenso de los pasajeros
