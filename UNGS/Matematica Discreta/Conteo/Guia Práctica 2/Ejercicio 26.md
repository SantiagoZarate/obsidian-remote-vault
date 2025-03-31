## Una Empresa Vende Bolsas Que Contienen 500 Piezas De Igual Diseño Cuya Finalidad Es El Uso En Juegos De Armado (tipo lego). Cada Pieza Puede Tener Uno De Entre 7 Colores Distintos. Suponiendo Que De Cada Color Debe Haber Al Menos 50, Pero De Color Rojo Debe Haber Como Mínimo 75, De Color Azul Más De 60, Y De Color Negro Exactamente 70. ¿Cuántas Tipos De Bolsas Distintas Puede Fabricar la Empresa?

Nota: Dos bolsas se consideran distintas si difieren en la cantidad de fichas de alguno de los colores

**Respuesta**

Observamos las restricciones de cada color:

$$  
\begin{aligned}
\text{Rojo} &\ge 75\\
\text{Azul} &\ge 61\\
\text{Negro} &= 70\\
\text{Color 4} &\ge 50\\
\text{Color 5} &\ge 50\\
\text{Color 6} &\ge 50\\
\text{Color 7} &\ge 50\\
\end{aligned}
$$

Del total de 500 piezas, restamos las 406 piezas que se necesitan para satisfacer las restricciones mínimas por color, por lo que nos quedan 94 piezas, donde cada una puede ser seleccionada entre 6 colores, notar que descartamos el color negro ya que va a ser siempre constante.

Entonces, por teorema de combinatoria con elementos repetidos, sabemos que la cantidad de bolsas distintas que puede fabricar la empresa es $C(99, 5)$
