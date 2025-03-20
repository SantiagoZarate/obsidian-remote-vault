---
status: Done
tags:
  - Permutación-Circular
  - Multiplicidad
---

## En Un Jardín De Infantes Hay 5 Niños Y Dos Familiares Adultos Por Cada Uno De Ellos Dispuestos a Realizar Un Acto Conmemorativo. En Dicho Acto la Maestra Determinó Que Los Cinco Grupos Familiares Debían Formar Una Ronda. ¿De Cuántas Formas Distintas Pueden Formar la Ronda Si Cada Niño Debe Tener a Ambos Lados a Sus Respectivos Familiares?

**Repuesta**

Para simplificar la terminología, los familiares adultos representan a la madre y el padre.

Observemos que podemos tener dos ordenamientos por cada grupo familiar:

$$
\text{Madre}\,\text{Niño}\,\text{Padre}
$$
$$
\text{Padre}\,\text{Niño}\,\text{Madre}
$$

el siguiente ordenamiento no cumple con lo pedido en el enunciado:

$$
\text{Niño}\,\text{Padre}\,\text{Madre}
$$

Definamos el conjunto $G$ = {$G_1$, $G_2$ , ... , $G_5$} cuyos elementos son los grupos familiares compuestos por los niños con sus familiares.

Necesitamos calcular las 5-permutaciones de un grupo de 5, por *teorema 2* de permutaciones circulares sabemos que es $4!$, Para cada uno de estos ordenamientos cada uno de los grupos familiares tiene 2 formas de ordenarse, como expliqué al principio.

Así que por principio multiplicativo tenemos que la cantidad de formas en sentar a los grupos familiares es:

$$
4! \cdot 2⁵
$$
