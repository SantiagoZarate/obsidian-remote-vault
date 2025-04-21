## Una Empresa Fabrica Dulce De Los Siguientes Sabores: Pera, Ananá, Manzana, Durazno, Ciruela, Damasco, Frutilla, Arándano, Membrillo Y Naranja. Los Envasa En Un Único Tipo De Frasco Cada Uno Con Su Correspondiente Etiqueta . En Un Supermercado Se Tiene Un Exhibidor De Plataforma Circular Rotatoria Donde Se Quieren Ubicar Los Frascos De Esta Empresa Para Exhibirlos

**a)** ¿De cuántas formas distintas se pueden ordenar los productos de esta marca en la
plataforma si debe haber un frasco de cada sabor, el de ananá, el de pera y el de manzana deben estar consecutivos en la presentación , y el de frutilla y el de arándano no deben estar juntos?

**b)** ¿De cuántas formas distintas se pueden ordenar en el exhibidor 12 productos de esta marca de dulces si deben estar presentes todos los sabores?

**Respuesta**

### **a)**

Observar que contamos con productos de 10 sabores distintos, de esos 10, vamos a agrupar los frascos de ananá, pera y manzana, de modo tal que cuando se ordenen estén juntos, de manera temporal vamos a dejar al frasco de arándano fuera de la distribución.

entonces contar los ordenamientos circulares de 7 elementos (seis frascos más el elemento que agrupa a los tres frascos para asegurar que estén seguidos) es igual a

$$ \frac{1}{7} \cdot 7! $$Para cada uno de estos ordenamientos tenemos que contar las permutaciones del elemento que agrupa los tres sabores que deben estar juntos, por principio multiplicativo tenemos que:

$$ \frac{1}{7} \cdot 7! \cdot 3! $$

y ahora nos falta ubicar el frasco de sabor de arándano, notar que si ubicamos 7 elementos en ronda tenemos 7 espacios que se generan entre cada frasco de la ronda, de estos 7 espacios sabemos que no podemos ubicarlo antes o después del frasco de sabor de frutilla por lo que finalmente contamos con 5 posibles lugares donde ubicar el frasco de arándano, por lo que por principio multiplicativo tenemos que:

$$ \frac{1}{7} \cdot 7! \cdot 3! \cdot 5 $$

esto equivale a la cantidad de formas de ubicar los frascos en ronda con tal que se respeten las condiciones del enunciado.

### **b)**

Observar que si se nos pide que deben estar presentes todos los gustos, como mínimo vamos a tener que ubicar 10 frascos, uno de cada sabor, por lo que nos queda por elegir 2 sabores más,

%%
1 - Usar el teorema de combinatoria con elementos repetidos
2 - Hacer por casos, uno donde agarro 2 frascos del mismo sabor, y otro donde 2 frascos, uno de cada sabor entre 10 distintos y eso sumarlo
%%

Definimos el conjunto $S$ cuyos elementos son las formas de distribuir 12 frascos cumpliendo la condición que estén presentes todos los sabores mencionados en el enunciado.

Definimos los siguientes subconjuntos de $S$:

- $A_1$ : Tal que haya 3 frascos del mismo sabor y los 9 frascos restantes de una sabor cada uno.
- $A_2$: Tal que haya 2 gustos que tengan repetición, y los restantes 8 frascos de un sabor cada uno

Notar que se cumple $S = A_1 \cap A_2$ y que $A_1 \cap A_2 = \emptyset$ por lo tanto $A_1$ y $A_2$ es una partición de $S$, por lo tanto:

$$ |S| = |A_1| + |A_2| $$

Calculemos los cardinales:

- $|A_1|$ = Notar que tenemos 10 posibles sabores de los que podemos elegir tener 3 frascos, y los restantes 9 sabores tienen 1 frascos, uno de las formas de armas la selección de 12 frascos puede ser 3 de pera, y los restantes de frascos de un sabor distinto cada uno.

  tenemos que contar los ordenamientos circulares de 12 elementos donde hay un tipo de elemento que tiene tres repeticiones, esto por cada uno de los sabores por lo que por principio multiplicativo tenemos que:

  $$ \frac{1}{12} \cdot \frac{12!}{3!} \cdot 10 $$

  esto equivale al cardinal de $A_1$

- $|A_2|$ = Un par de sabores deben tener dos frascos, y los restantes 8 sabores un frasco cada uno, por lo que contar los ordenamientos circulares de 12 elementos donde dos tipos de elementos tengan dos repeticiones, para cada uno de estos ordenamientos tenemos que contar también las formas de seleccionar 2 sabores de los 10 posibles entonces por principio multiplicativo tenemos que:
  $$ \frac{1}{12} \cdot \frac{12!}{2! \cdot 2!} \cdot C(10,2) $$
  esto equivale al cardinal de $A_2$

  Ahora hacemos la sumatoria de ambos cardinales:

