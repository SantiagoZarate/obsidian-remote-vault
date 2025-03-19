## Las Patentes De Los Automóviles En Nuestro País Se Escriben Mediante Tres Letras Seguidas De Tres Números, Como Por Ejemplo SFX 984 - EEY 233. La Letra Ñ no Se Admite En Las Patentes Y Tanto Las Letras Como Los Números Pueden Repetirse. ¿Cuántas Patentes Diferentes Son Posibles?

**Respuesta:**

Sea S el conjunto de patentes posibles, definimos el subconjunto $S_1$ de $S$ cuyos elementos son las primeras 3 letras de la patente, y el subconjunto $S_2$ de S cuyos elementos son los 3 siguientes dígitos.

podemos ver que $S_1$ y $S_2$ es una partición de $S$, por lo que podemos calcular $|S|$ de la siguiente manera:
$$|S| = |S_1| + |S_2|$$
Para calcular los cardinales de $S_1$ tenemos que para la primer posición contamos con 26 posibles candidatos, y que por cada uno de las opciones que escojamos tendremos 26 posibles posibilidades para la segunda y tercera posición, esto es debido a que se permiten tener letras repetidas entre las patentes.

entonces tenemos que:
$$|S_1| = 26³$$
Para calcular el $|S_2|$ podemos hacer un análisis de manera análoga al conjunto anterior, solo que en este caso contamos con 10 posibilidades por posición, esto es así porque tenemos dígitos del 0 al 9, por lo que tenemos que:
$$|S_2| = 10³$$
Ahora que calculamos los cardinales de $|S_1|$ y $|S_2|$ y que para cada una de las tres primeras letras contamos con la posibilidad de asignar cualquier combinación de los siguientes tres números, por el principio de multiplicidad tenemos que: