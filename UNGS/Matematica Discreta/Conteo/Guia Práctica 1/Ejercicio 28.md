## En El Instituto De Ciencias De la UNGS Trabajan 14 Investigadores De Computación Y 15 De Matemática

**a)** ¿De cuántas formas se puede formar un equipo de investigación de 11 personas si se puede elegir de entre los investigadores de Computación y de Matemática juntos?

**b)** ¿De cuántas formas se puede formar dos equipos de 11 personas cada uno, uno formado solamente por investigadores de Computación y otro solamente formado por investigadores de Matemática?

**c)** ¿De cuántas formas se puede formar un equipo de 11 personas, pudiendo elegir entre todos los investigadores de Computación y Matemática juntos, si debe estar conformado por más de 8 investigadores de Computación?

**Respuesta**

## **a)**

Observemos que se nos pide seleccionar 11 personas de un conjunto con un total de 29, lo que por combinatoria sabemos que es $C(29,11)$

**b)**

> [!tip] Separadores
> En clase, en un ejercicio donde teníamos que agrupar cartas en 5 mazos, decidimos agregar separadores, quizás puede ser util aca

Sea $C$ el conjunto cuyos elementos son las formas de armar un equipo de 11 investigadores de Computación, se nos pide obtener $C$, y por cada uno de las selecciones tenemos que tener en cuenta las formas de armar un equipo de 11 investigadores de Matemática, así que por principio multiplicativo lo que pedido en en enunciado se obtiene resolviendo

$$|C| \cdot \text{Ordenamientos de 11 investigadores de Matemática}$$

Para calcular $|C|$ tenemos que contar las formas de seleccionar 11 personas de un grupo de 14, lo que es $C(14,11)$, Para contar los ordenamientos del otro grupo necesitamos contar las formas de seleccionar 11 personas de un grupo de 15 personas, lo que es igual a $$C(15,11)$$

Entonces la cantidad de formas de armar ambos equipo es $C(14,11) \cdot C(15,11)$

**c)**

Sea $S$ el conjunto cuyos elementos sean las formas de armar un equipo de 11 personas a partir de 29 investigadores, definimos $H \subset S$ cuyos elementos tienen como máximo 2 investigadores de computación, por definición de complemento tenemos que $\overline{H}$ es el conjunto cuyos elementos tienen al menos 9 investigadores de computación. por principio de sustracción sabemos que:

$$
|\overline{H}| = |S| - |H| 
$$

Sabemos que $|S| = C(29,11)$ ya es la cantidad de seleccionar 11 personas de un grupo de 29 personas.

Ahora necesitamos calcular $|H|$, es decir la cantidad de formas de seleccionar 11 personas donde como máximo tengamos 2 investigadores de computación, como el orden de los integrantes del equipo no importa, tenemos que seleccionar 2 personas de un grupo de 14 investigadores de computación y por cada uno de las selecciones nos quedan por elegir 9 personas de un grupo de 15 investigadores de computación, lo que por principio de multiplicación es igual a:

$$  
\begin{aligned}
|H| &= C(14,2) \cdot C(15,9)\\
|H| &= 91 \cdot 5005\\
|H| &= 455455
\end{aligned}
$$ 

Ahora podemos seguir en la búsqueda de $\overline{H}$

$$  
\begin{aligned}
|\overline{H}| &= |S| - |H|\\
|\overline{H}| &= C(29,11) - 455455\\
\end{aligned}
$$

**Desarrollo de combinatorios**

---

$$
\begin{pmatrix} 14 \\ 2 \end{pmatrix} =
\frac{14!}{(14-2)! \cdot 2!} =
\frac{14!}{12! \cdot 2!}=
\frac{14 \cdot 13 \cdot 12!}{12! \cdot 2!} =
\frac{182}{2} = 
91
$$
---
$$
\begin{pmatrix} 15 \\ 9 \end{pmatrix} =
\frac{15!}{(15-9)! \cdot 9!} =
\frac{15!}{6! \cdot 9!}=
\frac{15 \cdot 14 \cdot 13 \cdot 12 \cdot 11 \cdot 10 \cdot 9!}{6! \cdot 9!} =
\frac{3603600}{720} = 
5005
$$
