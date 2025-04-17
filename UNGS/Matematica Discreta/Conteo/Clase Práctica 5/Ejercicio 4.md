## La Clave PIN De Un Cliente Del Banco Nación Consiste En Un Número De Cuatro Dígitos Que Elige El Cliente. Por Razones De Seguridad, El Banco no Permite Que Dicho Número De PIN Contenga Dígitos Repetidos Y Tampoco Permite Que Ningún Dígito Del Número PIN Coincida Con El Dígito Que Ocupa la Misma Posición En la Escritura Del Año En Que Nació El Cliente. Por Ejemplo, Si El Cliente Nació En 1980 Entonces Además De Que Los Dígitos De la Clave PIN Tienen Que Ser Todos Distintos Entre Sí, El Primer Dígito De la Clave PIN no Puede Ser 1, El Segundo Dígito no Puede Ser 9, El Tercero no Puede Ser 8 Y El Último no Puede Ser 0. ¿De Cuántas Maneras Puede Elegir Su Clave PIN Un Cliente Nacido En 1980?

**Respuesta**

- Para la primer posición del número PIN contamos con 10 dígitos originalmente, pero no podemos elegir el 1, por lo tanto nos quedan 9 opciones
- Para la segunda posición contamos con 8 opciones (restamos el dígito 9 de los posibles, y el que elegimos para la 1er posición)
- Para la tercer posición contamos con 7 opciones
- Para la última posición contamos con 6 opciones

Por cada

Sea $S$ el conjunto cuyos elementos son números de cuatro dígitos del 0-9 tal que no contengan dígitos repetidos, declaramos las siguientes propiedades:

$$  
\begin{aligned}
P_1 &= \text{La primer debe ser un 1, 9, 8 o 0}\\
\end{aligned}
$$ 

Sea $S$ el conjunto cuyos elementos son números de cuatro dígitos del 0 al 9, definimos el subconjunto $A$ de $S$ tal que sus elementos están formados por los dígitos 1, 9, 8 o 0, por definición de complemento tenemos $\overline{A}$ tal que sus elementos no
