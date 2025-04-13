---
tags:
  - Multiplicidad
  - Combinación
status: Done
---

**a)** ¿Cuántas palabras de 8 letras se pueden formar con las letras de la palabra MURCIELAGO?

**b)** ¿Cuántas que contengan a todas las vocales?

**c)** ¿En cuántas aparecen todas las vocales y en el orden A E I O U? Ejemplo: ARECILOU

**Respuesta**

## **a)**

Observemos que la palabra dada no tiene letras repetidas, necesitamos contar las formas de seleccionar 8 letras de las 10 disponibles, eso es igual a $C(10, 8)$, por cada una de estas selecciones tenemos que contar sus ordenamientos, lo que es igual a $8!$.

Entonces, la cantidad de palabras de 8 letras que se pueden formar con las letras de la palabra dada es igual a :

$$
C(10, 8) \cdot 8!
$$
## **b)**

En este caso 5 de las 8 letras de la palabra van a estar ocupadas por las 5 vocales que tiene la palabra MURCIELAGO, por los que tenemos que contar las formas de seleccionar 3 consonantes de las 5 restantes, eso es igual a $C(5,3)$, por cada una de estas selecciones tenemos que contar la cantidad de formas de ordenar las 8 letras, eso es igual a $8!$.

Luego la cantidad de palabras de 8 letras que contengan todas las vocales es:

$$
C(5,3) \cdot 8!
$$
## **c)**

Notemos que solo existe un orden alfabético, entonces las cinco vocales presentes en las palabras de 8 letras van a estar en el siguiente orden:

$$
AEIOU
$$

Ahora necesitamos contar las formas de seleccionar 3 de las 5 consonantes restantes para formar palabras de 8 letras, esa cantidad es igual a $C(5,3)$. Por cada una de estas selecciones vamos a tener que ubicar las consonantes entre las vocales ya establecidas, tenemos 6 espacios disponibles entre las vocales, cada una de 3 consonantes que fueron seleccionadas cuentan con estos 6 espacios

Una vez ya hayamos elegido los espacios necesitamos contar los ordenamientos de las 3 letras que fueron seleccionadas, entonces por principio multiplicativo tenemos que:

$$
C(5,3) \cdot 6³ \cdot 3!
$$

equivale a la cantidad de palabras de 8 letras que tengan las vocales en orden alfabético.
