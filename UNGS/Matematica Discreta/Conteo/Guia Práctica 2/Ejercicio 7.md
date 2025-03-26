---
tags:
  - Permutación
  - Multiplicidad
status: Done
---

## ¿De Cuántas Formas Distintas Se Pueden Ordenar 17 Libros Distintos En 4 Estantes Diferentes, Cada Uno De Ellos Con Capacidad Para 17 Libros?

**Respuesta**

Observar que podemos plantear el problema como contar el ordenamiento de 17 libros distintos, y luego entre los espacios de los libros colocar separadores que representarían el fin de un estante y el comienzo de otro.

Contar las permutaciones de 17 libros es igual a $17!$, para cada uno de estos ordenamientos tenemos 18 espacios, Notar que tenemos 3 separados ya que en el enunciado se nos dice que se usan 4 estantes distintos. Para cada separador, teniendo en cuenta que no importa que haya un mínimo de libros por estantería, tenemos 18 posibles espacios, por principio multiplicativo la cantidad de formas distintas de ordenar los libros según lo pedido en el enunciado es:

$$
17! \cdot 18³
$$
