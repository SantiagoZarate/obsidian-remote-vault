## Un Determinado Club Cuenta Con 60 Miembros, 30 De Ellos Residentes En El Partido De Malvinas Argentinas Y Los Restantes En El De San Miguel. Se Desea Conformar Un Comité Con 8 Miembros

**a)** ¿De cuántas formas puede conformarse?

**b)** ¿De cuántas formas puede conformarse si al menos uno de los 8 debe ser un residente de Malvinas Argentinas?

**c)** ¿De cuántas formas puede conformarse si al menos tres miembros deben residir en San Miguel y al menos tres deben residir en Malvinas Argentinas?

**Respuesta**

**a)**

Observemos que se nos pide seleccionar 8 miembros de un grupo de 60 personas, y que en este caso el orden en que los escoja no nos importar, por lo tanto la cantidad de formas en que puede conformarse dicho grupo es de $C(60,8)$

**b)**

En el caso de que uno de los 8 integrantes del grupo sea de Malvinas Argentinas, nos queda por seleccionar 7 miembros del grupo de personas, notar que no podemos seleccionar la persona que ya fue seleccionado, por lo tanto nos quedan $C(59,7)$ formas de armar el grupo con un residente de Malvinas Argentinas.

**c)**

En el caso de que necesite tener 3 miembros como mínimo de cada localidad, seleccionamos 3 del grupo de 30 personas que residen en Malvinas Argentinas, es decir que tenemos $C(30, 3)$ formas de seleccionarlos, hacemos lo mismo con las personas de Polvorines, nos quedan también $C(30,3)$ formas de seleccionarlos.

Las dos personas restantes del grupo tienen que ser seleccionadas del total de miembros original, pero descartamos a los 3 seleccionados de Malvinas Argentinas y los 3 seleccionados de Polvorines, así que nos quedan $C(54, 2)$ formas de seleccionar las ultimas dos personas.

Notar que para cada una de las formas de seleccionar las personas por localidad vamos a contar con $C(54,2)$ formas de seleccionar las ultimas dos personas, por lo que por principio multiplicativo es:

$$
C(30,3) \cdot C(30,3) \cdot C(54,2)
$$
