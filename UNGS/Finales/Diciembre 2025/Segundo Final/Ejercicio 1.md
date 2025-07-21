El culto del psico-casco tiene 8 sedes. Para definir al líder del culto cada sede envía un psíquico que la represente. Los 8 representantes se ordenan en 4 duelos numerados del 1 al 4. El ganador del duelo 1 se enfrentará al ganador del duelo 2 y el ganador del duelo 3 se enfrentará al ganador del duelo 4. Finalmente, los ganadores de estos dos últimos duelos se enfrentarán para establecer a su líder.

(a) ¿Cuántas combinaciones posibles hay para el desarrollo del torneo en su totalidad?

(b) Los espectadores del torneo se dividen en 10 grupos, un grupo por cada sede, un grupo de neutrales y un grupo que protesta exigiendo que Mob sea el líder. Suponiendo que en cada grupo hay por lo menos 10 personas, ¿cuál es la mínima cantidad de espectadores que debe haber para que alguno de los grupos tenga por lo menos 25 personas?

**Respuestas**

## A-

Primero empecemos contando de que manera podemos seleccionar las parejas que componen los duelos, para la primer pareja tenemos que seleccionar 2 psíquicos de 8 psíquicos en total, para el segundo duelo tenemos que seleccionar 2 psíquicos entre 6 disponibles, así hasta formar todas las parejas, la selección de un psíquico no condiciona las cantidades de formas de seleccionar un psíquico para otros duelos, por lo que por principio multiplicativo tenemos que

$$
\begin{pmatrix} 8 \\ 2 \end{pmatrix} \cdot
\begin{pmatrix} 6 \\ 2 \end{pmatrix} \cdot
\begin{pmatrix} 4 \\ 2 \end{pmatrix} \cdot
\begin{pmatrix} 2 \\ 2 \end{pmatrix}
$$

es la cantidad de formas de seleccionar las parejas que conforman los duelos.

Ahora hay que tener en cuenta los posibles ganadores de cada duelo, por cada duelo tenemos 2 posibles resultados, ya que no se puede terminar un duelo en empate.

Luego en la primer ronda que tenemos 4 duelos, por cada uno de esos duelos tenemos 2 posibles resultados, lo que por principio multiplicativo tenemos que hay $2⁴$ posibles resultados en la ronda inicial.

Luego en la segunda ronda, donde tenemos al ganador del duelo 1 contra el ganador del duelo 2, y por otro lado tenemos al ganador del duelo 3 contra el ganador del duelo 4 tenemos 2² posibles resultados.

Por ultimo tenemos el duelo final donde tenemos 2 posibles resultados.

Cada una de los resultados en cada fase en independiente de la fase siguiente, por lo que por principio multiplicativo tenemos que 2⁷ son los resultados posibles, y estos resultados a su vez son independientes de las formas de armar las parejas, por lo que

$$
\begin{pmatrix} 8 \\ 2 \end{pmatrix} \cdot
\begin{pmatrix} 6 \\ 2 \end{pmatrix} \cdot
\begin{pmatrix} 4 \\ 2 \end{pmatrix} \cdot
\begin{pmatrix} 2 \\ 2 \end{pmatrix} \cdot 2⁷$$
es la cantidad de formas en las que se puede desarrollar el torneo.
