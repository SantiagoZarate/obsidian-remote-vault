## En Un Laboratorio Se Tienen 6 Computadoras Numeradas Del 1 Al 6, Y Seis Aulas Numeradas Del 1 Al 6. Suponiendo Que Se Quiere Poner Una Computadora En Cada Aula

**a)** ¿De cuántas formas se puede asignar una computadora a cada aula con la condición de que las computadoras 1 y 5 no sean asignadas a aulas numeradas consecutivamente?

Nota: No importa el orden en que se asignan las computadoras.

**b)** ¿De cuántas formas se puede asignar una computadora a cada aula si, además de las condiciones del ítem anterior, se tiene que considerar el orden en que se las instala en las aulas?

Nota: No se pueden instalar dos o m ́as computadoras al mismo tiempo.

**Respuesta**

### **a)**

Sea $S$ el conjunto cuyos elementos son números de 6 dígitos del 1-6, donde cada posición del número representa que computadora se asigna a cada aula, por el ejemplo con el número 234561, estamos diciendo que en la 1er aula va la 2da computadora, en la segunda va la 3er computadora, y así hasta la última posición.

Definimos $A \subset S$ tal que sus elementos tienen a los dígitos 1 y 5 en posiciones contiguas, por definición de complemento tenemos $\overline{A}$ tal que los dígitos 1 y 5 no están juntos, resolver el problema es calcular $|\overline{A}|$, por lo que por principio de sustracción es:

$$ |\overline{A}| = |S|  - |A| $$

pasemos a calcular los cardinales:

- $|S|$ = $6!$, ya que es la cantidad de permutaciones del número de 6 dígitos sin restricciones
- $|A|$ = Tomamos a los dígitos 1 y 5 como si fuera uno solo para asegurar la condición que estén juntos, y luego necesitamos contar la cantidad de repeticiones de 5 elementos, eso $5!$, para cada uno de estos ordenamientos tenemos que contar las permutaciones de 1 y 5 que es $2!$, por principio multiplicativo nos queda $5! \cdot 2!$

Ahora podemos continuar en nuestro calculo de $\overline{A}$:

$$  
\begin{aligned}
|\overline{A}| &= |S|  - |A| \\
|\overline{A}| &= 6!  - 5! \cdot 2! \\
|\overline{A}| &= 720  - 240 \\
|\overline{A}| &= 480 \\
\end{aligned}
$$

Esto equivale a la cantidad de formas de asignar las computadoras a cada sala respetando la condición del enunciado.

### **b)**
