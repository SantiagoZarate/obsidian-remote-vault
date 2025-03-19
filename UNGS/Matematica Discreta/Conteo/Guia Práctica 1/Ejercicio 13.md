---
tags:
  - "Combinación"
---
## ¿De Cuántas Formas Se Pueden Elegir Subconjuntos De Tres Elementos Del Conjunto Formado Por Las Letras A, B, C, D, E?

**Respuesta:**

Definimos el conjunto L = {A, B, C, D, E}

Sea el conjunto S cuyos elementos sean subconjuntos de tres elementos de $L$, para resolver lo planteado en el enunciado es igual a obtener $|S|$,

Elemento de S podrían ser:

- {A, B, C}
- {A, B, D}
- {A, B, E}

El subconjunto {A, C, B} no se considera distinto de {A, B, C}, ya que en los subconjuntos el orden no importa.

Por combinatoria tenemos que la cantidad de formas de elegir subconjuntos de tres elementos de $|L|$ es C(5, 3)

$$  
\begin{aligned}
|S| = C(5, 3)
= \frac{5!}{(5 - 3)! \cdot 3!}
= \frac{5!}{2! \cdot 3!} 
= \frac{5\cdot4\cdot3!}{2!\cdot3!}
= \frac{20}{2}
= 10
\end{aligned}
$$

$$  
\begin{aligned}
C(10,8) &= C(10,2)\\
C(10,8) &= \frac{10!}{(10-8)!\cdot8!} = \frac{10!}{2!\cdot8!} = \frac{10\cdot9\cdot8!}{2!\cdot8!} = \frac{10\cdot9}{2} = 45\\
C(10,2) &= \frac{10!}{(10-2)!\cdot2!} = \frac{10!}{8!\cdot2!} = \frac{10\cdot9\cdot8!}{8!\cdot2!} = \frac{10\cdot9}{2} = 45
\end{aligned}
$$ 
