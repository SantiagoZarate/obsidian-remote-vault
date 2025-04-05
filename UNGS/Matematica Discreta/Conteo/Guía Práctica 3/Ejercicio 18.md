## Un Juego Tiene Un Mazo De 40 Cartas, Diez Rojas Numeradas Del 1 Al 10, Diez Azules Numeradas Del 1 Al 10, Diez Verdes Numeradas Del 1 Al 10 Y Diez Blancas Numeradas Del 1 Al 10. Suponiendo Que Juegan 4 Personas, Se Le Reparten 10 Cartas a Cada Uno E Importa El Orden En Que Cada Jugador Recibe Sus Cartas. ¿De Cuántas Formas Distintas Se Pueden Repartir Las Cartas Con la Condición De Que El Jugador Uno no Tengan Todas Sus Cartas Del Mismo Color, Y El Jugador Dos Tenga Al Menos Dos Cartas Con El Mismo Número?

**Respuesta**

Posibles propiedades

- Jugador 1 no tenga sus cartas del mismo color
- Jugador 2 tenga al menos dos cartas con el mismo número

Para la prop 2

Definamos $1 \le i \le 10$ y las variables

$$
x_i = \text{cantidad de cartas con el número i}
$$

$$
x_1  + x_2 + x_3 + x_4 + x_5 + x_6 + x_7 + x_8 + x_9 + x_{10} = 10
$$

Con la restricción de

$$
2 \le x_i \le 4
$$

Definimos el conjunto $S$ cuyos elementos son las soluciones en $\mathbb{Z} \ge 0$ a la ecuación planteada, definimos las siguientes propiedades:

$$
p_j = x_j \le 2
$$

y los subconjuntos $A_j$ de $S$ con $1 \le j \le 9$ tal que los elementos de $A_j$ satisfacen la propiedad $P_j$. Bajo estas condiciones la cantidad de formar de que el jugador dos tenga al menos 2 cartas con el mismo número es igual a calcular el cardinal de $A_1 \cap A_2 \cap ... \cap A_9$ para ello haremos uso del principio I-E para 9 propiedades.
