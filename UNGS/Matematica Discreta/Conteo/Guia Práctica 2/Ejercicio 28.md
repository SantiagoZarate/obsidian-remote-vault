---
tags:
  - Combinación-Repetidos
status: Incomplete
---

## Cierta Caja Musical Tiene Una Pieza Circular Con 20 Espacios a Lo Largo De Su Borde Donde Se Pueden Colgar Campanitas Elegidas Entre 4 Tipos Distintos. Suponiendo Que Al Menos Un Espacio no Debe Quedar Vacío, Que Hay Suficientes Campanitas Para Que Las 20 Sean Del Mismo Tipo Y Que Las Campanitas Del Mismo Tipo Son Indistinguibles

**a)** ¿De cuántas formas distintas se pueden elegir las campanitas sin considerar como se ubicarán en la pieza circular?

**b)** En una elección al azar se tomaron 3 campanitas del tipo uno, 3 del tipo dos, 5 del tipo tres y 4 del tipo cuatro. ¿De cuántas formas distintas se pueden ubicar estas campanitas en el borde de la pieza circular con la condición de que las campanitas del tipo 1 estén todas juntas, las del tipo 2 estén todas juntas y no haya dos espacios vacíos consecutivos?

**Respuesta**

### **a)**

La cantidad de formas distintas de seleccionar 20 campanitas entre 4 tipos distintos, sabiendo que tenemos una cantidad ilimitada por tipo, sabemos que por *teorema* de combinatoria con elementos repetidos es $C(23, 3)$

### **b)**

Definimos los siguientes conjuntos:

$$  
\begin{aligned}
A &= \text{las 3 campanas elegidas del grupo 1}\\
B &= \text{las 3 campanas elegidas del grupo 2}\\
\end{aligned}
$$

Ahora definimos el siguiente multiconjunto $P$:

$$
\{1 \cdot A, 1 \cdot B, 5 \cdot \text{Campanas Tipo 3}, 4 \cdot \text{Campanas Tipo 4} \}
$$
