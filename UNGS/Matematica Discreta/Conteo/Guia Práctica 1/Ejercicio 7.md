## En Una Habitación Hay 7 Puertas. ¿De Cuántas Formas Se Puede Entrar Por Una Puerta Y Salir Por Otra Distinta?

**Respuesta:**

Sea S el conjunto cuyos elementos son las combinaciones de puertas para entrar por una puerta y salir por otra distinta, sea el conjunto P = {$P_1, P_2,... , P_7$} donde cada elemento representa a cada una de las puertas del enunciado, ejemplos de elementos del conjunto S son:
$$
\{P_1, P_2\}, \{P_7, P_2\},\{P_4,P_5\}
$$
Un elemento invalido sería:
$$
\{P_2,P_2\}
$$
Ya que no se puede repetir la misma puerta para entrar y para salir.

Para calcular el ordenamiento en hilera de puertas hago uso de la formula de permutación.
$$P(7,2) 
= \frac{7!}{(7-2)!} 
= \frac{7!}{5!} 
= \frac{7\cdot6\cdot5!}{5!}
= 7\cdot6
$$
Entonces para calcular $|S|$ solo queda por resolver la cuenta $7\cdot6$