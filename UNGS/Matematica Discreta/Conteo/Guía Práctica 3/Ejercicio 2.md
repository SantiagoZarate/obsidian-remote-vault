---
tags:
  - Inclusión-Exclusión
status: Done
correcto: true
---

## Encuentre El Número De Permutaciones De Los Números 1, 2, 3, 4, 5, 6 Tal Que El 2 no Esté En El Segundo Lugar Ni El 5 Esté En El Quinto Lugar

**Respuesta**

Sea $S$ el conjunto cuyos elementos son números de 6 dígitos, definimos las siguientes propiedades.

$$  
\begin{aligned}
P_1 &= \text{El 2 esta en el segundo lugar}\\
P_2 &= \text{El 5 esta en el último lugar}\\
\end{aligned}
$$

Definimos $A_1 \subset S$ cuyos elementos satisfacen $P_1$, y también $A_2 \subset S$ cuyos elementos satisfacen $P_2$

Bajo estas definiciones el problema se resuelve calculando el cardinal de $\overline{A_1} \cap \overline{A_2}$ y para ello usaremos el principio inclusión-exclusión para 2 propiedades.

$$
|\overline{A_1} \cap \overline{A_2}| = |S| - |A_1| - |A_2| + |A_1 \cap A_2|
$$

Ahora necesitamos obtener los cardinales.

- $|S|$ = La cantidad de permutaciones de 6 dígitos sin dígitos repetidos es $6!$
- $|A_1|$ = Calcular la cantidad de permutaciones donde el 2 este en la segunda posición, fijamos el 2 a esa posición y permutamos los restantes 5 dígitos, eso es $5!$
- $|A_2|$ = De manera análoga al razonamiento de calcular $|A_1|$ , esto es $5!$
- $|A_1 \cup A_2|$ = Calcular la cantidad de permutaciones donde el 2 este en la segunda posición y el 5 en la última, por lo que tenemos que permutar los 4 dígitos restantes, eso es igual a $4!$

Entonces la cantidad de permutaciones de los dígitos propuesta por el enunciado con sus restricciones es:

$$
6! - 5! - 5! + 4!
$$
