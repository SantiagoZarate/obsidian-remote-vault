## Un Tren De Carga Transporta 27 Containers Iguales Entre 7 Ciudades. Para En Las 7 Ciudades Si O Si Y Puede Dejar O no Mercadería, De Acuerdo a Los Pedidos

**a)** ¿De cuántas maneras podrá descargar los containers?

**b)** ¿De cuántas maneras debería descargar los containers si en cada ciudad si o si por lo menos dejará uno?

**c)** ¿De cuántas maneras, sabiendo que en la ciudad 2 debe dejar por lo menos 2 cajas, en la ciudad 5 más de 4 cajas y en el resto de las ciudades no hay restricciones?

**Respuesta**

### **a)**

Siendo que tenemos una cantidad ilimitada de containers que se pueden descargar por ciudad, usamos el teorema de combinatoria con elementos repetidos, donde tenemos que contar la cantidad de formas de seleccionar las ciudades a los que cada container se descargará, esto es igual a $C(33, 6)$

### **b)**

En caso de que tengamos que descargar si o si por lo menos uno, de los 27 containers originales, restamos 7, para poder satisfacer la cantidad mínima por ciudad, y ahora nos queda contar la cantidad de formas de seleccionar las ciudades en donde cada container sera descargado, eso es igual a $C(26, 6)$

### **c)**

Del total de 27 container restaremos las siguientes unidades para que se cumplan las restricciones mínimas.

- 2 en la ciudad 2
- mas de 4, o sea, al menos 5
entonces, nos quedan 20 container que deben ser repartidos entre 7 ciudades, necesitamos contar la cantidad de formas de seleccionar las ciudades en donde cada container será descargar, eso es igual a $C(26, 6)$
