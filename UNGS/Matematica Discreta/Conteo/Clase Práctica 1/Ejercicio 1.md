## Un Menú Estudiantil Permite Seleccionar Una Entrada Entre Cuatro, Una Comida Caliente Entre Tres Y Un Postre Entre Cinco

 **a)** ¿De Cuántas Formas Puede Elegir Su Menú Un Estudiante?

**b)** ¿De cuántas formas puede hacerlo si desea que el salpicón de ave y la suprema de pollo no aparezcan en el mismo menú?

**Respuesta**

### **a)**

Sea el conjunto S cuyos elementos son las formas en que se puede armar un menu de estudiante, lo pedido en el enunciado se resuelve calculando $|S|$.

Notar que para cada selección de la entrada, podemos elegir cualquiera de las comidas calientes y cualquiera de los cinco postres, entonces por principio multiplicativo podemos calcular el cardinal de S, que es:

$$  
\begin{aligned}
|S| &= 4 \cdot 3 \cdot 5\\
|S| &= 60
\end{aligned}
$$ 

Entonces la cantidad de menúes estudiantiles que se pueden formar es 60

### **b)**

Para calcular las formas en la que se puedan formar menúes satisfaciendo la característica que el salpicón de ave y la suprema de pollo no este en el mismo menú podemos hacer el siguiente análisis.

Definimos el subconjunto $M$ de $S$ cuyos elementos son los menúes que tienen el salpicón de ave y la suprema de pollo en el menú, por definición de complemento tenemos $\overline{M}$ el conjunto cuyos elementos no tienen el salpicón de ave y la suprema de pollo en el menú al mismo tiempo.

Lo pedido en el enunciado se resuelve obteniendo $|M|$ que por principio de sustracción es:

$$
|\overline{M}| = |S| + |M|
$$

El cardinal de $S$ lo calculamos en el punto anterior, que es 60, por lo que nos resta calcular $M$.

- Para la entrada ya tenemos la elección del salpicón de ave
- Para la comida caliente tenemos la elección de la suprema de pollo
- Para el postre tenemos 5 opciones.

Entonces tenemos el siguiente cálculo:

$$  
\begin{aligned}
|M| &= 1 \cdot 1 \cdot 5\\
|M| &= 5
\end{aligned}
$$

Ahora que tenemos el cardinal de $M$ podemos obtener $|\overline{M}|$

$$  
\begin{aligned}
|\overline{M}| &= 60 - 5\\
|\overline{M}| &= 55
\end{aligned}
$$

Entonces la cantidad de formas de armar un menú en donde el salpicón de ave y la suprema de pollo compartan el menú es de 55.
