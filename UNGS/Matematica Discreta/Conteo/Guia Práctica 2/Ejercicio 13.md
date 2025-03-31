---
status: Done
tags:
  - Cantidad-Subconjuntos
---

## Se Tienen 50 Libros Distintos De Matemática Y 70 Libros Distintos De Física. Se Le Pide a Una Persona Que Elija la Cantidad De Libros Que Quiera, Por Lo Menos Uno, Con la Única Condición De Que Todos Sean De Matemática O Todos Sean De Física. ¿De Cuántas Maneras Podrá Hacer Dicha Selección?

**Respuesta**
Definimos el conjunto $M$ tal que sus elementos sean los 50 libros de matemática del enunciado, también definimos $F$ el conjunto cuyos elementos son los 70 libros de física. lo pedido en el enunciado se resuelve obteniendo sumando la cantidad de subconjuntos que se pueden formar de cada conjunto.

Para calcular la cantidad de subconjuntos de un conjunto sabemos que es $2^n$, donde $n$ es la cantidad de elementos de un conjunto, en este caso, la cantidad de subconjuntos de $M$ es $2^{50}$, de la misma manera, la cantidad de subconjuntos de $F$ es $2^{70}$

Notar que en el enunciado se especifica que al menos se debe tomar un libro, por lo que debemos restar el conjunto vacío de la cantidad de subconjuntos de $M$ y $K$

Luego la cantidad de maneras de hacer dicha selección es:

$$
(2^{50} - 1 ) + (2^{70} - 1)
$$
