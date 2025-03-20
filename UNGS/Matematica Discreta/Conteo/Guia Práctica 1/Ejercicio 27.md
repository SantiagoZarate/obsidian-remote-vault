---
status: TODO
---

## ¿De Cuántas Formas Se Puede Pintar Un Cubo Con Seis Colores Dados De Tal Forma Que no Haya Dos Caras Del Cubo Pintadas Con El Mismo Color? Dos Coloraciones Se Consideran Iguales Si Pueden Superponerse De Manera Tal Que Cada Cara Tenga El Mismo Color

**Respuesta**

Observemos que el cubo tiene la cara de arriba, la cara de abajo y las 4 caras en los costados, estas ultimas caras las podemos pensar como un ordenamiento circular.

- Para la cara de arriba tenemos 6 posibles colores
- Para la cara de abajo tenemos 5, porque descartamos la que elegimos al principio
- Nos quedan 4 caras que van a ser ordenadas de manera circular, por lo que por *teorema 2 de permutaciones circular* sabemos que es 3!

Para cada una de las caras elegidas para la cara de arriba y la de abajo tenemos $3!$ ordenamientos para las caras de los costados, por lo que por principio multiplicativo tenemos que la cantidad de formas de pintar un cubo según lo pedido en el enunciado es

$$
6 \cdot 5 \cdot 3!
$$

> [!tip] No es lo buscado en el enunciado
> Notar que si yo al cubo lo giro de tal manera que la cara de arriba ahora esta en el lugar de la cara de abajo, la disposición de colores es la misma, pero yo lo estoy contando como una nueva forma de pintar el cubo
