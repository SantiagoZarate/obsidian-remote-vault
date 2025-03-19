## Fuentes De Cambios

### Requerimientos
  - Faltantes, erróneos o innecesarios
  - Cambios en la arquitectura
  - Diseño e implementación
  - Cambios en el negocio
  - Necesidades del usuario
  - Inciertas o desconocidas
  - Demandas del mercado
  - Cambio de interesados en el proyecto

### Tecnología
- Plataformas
- Interfaces con componentes externos
- Cambios en componentes de 3ros
- Cambios en tecnología o metodologías de desarrollo
- Utilización de nuevas tecnologías
- Cambio de tecnología obsoleta

## Proceso De Administración De Cambio

**1ra etapa:**
Análisis de impacto, evaluación, aprobación, priorización, planificación
**2da etapa:**
Desarrollo prueba
**3ra etapa:**
Validación, implementación, cierre

Es muy importante el triangulo de negociación, donde la modificación de cualquier arista (Recursos, Schedule, Funcionalidad) modifica las demás.

## Gestión De Riesgo

El peligro esta relacionada a un tema físico, el incidente para I.T, es un tema no resuelto, no es un riesgo. Un ejemplo es si al construir una casa, el plano fuera rechazado, por lo tanto habría que rearmarlo.

Hay categorías de riesgos.

**Conocidos - Conocidos:**
Podemos conocer la forma de solucionarlos, Conozco el riesgo y conozco de que manera gestionarlo

**Conocidos - Desconocidos:**
En este caso tenemos que tomarnos el tiempo para aprender, por ejemplo, una nueva tecnología.

**Desconocidos - Desconocidos:**
Aparece una situación novedosa no prevista, por lo tanto no tenemos experiencia de como mitigarla. ej: La pandemia de 2019.

## Creencias

Sirven para tratar de desmitificar.

- Hablar de riesgos es un signo de madurez profesional por ser cautos
- Hablar con un sponsor acerca de un equipo que tenga control total de un proyecto es muy improbable de tener
- Se debe compartir los posibles problemas latentes en el proyecto, dar el aviso y también el plan de acción

## Restricciones

Son límites que tenemos en el proyecto que acotan nuestros margenes y deberían despertar la identificación de riesgos, es crucial identificarlas al inicio del proyecto y también durante el proyecto.

## Fuentes De Riesgos V2

- Usuarios no capacitados para adaptar una nueva tecnología o no del todo compremetido con el proyecto, por ejemplo no hay devolución sincera.
- Cantidad de cambio excesivo, calendarios, costos o presupuestos irreales
- Falta de calidad en el producto. Diseño inadecuado
- Proceso y ambiente de desarrollo. Nuevas tecnologías
- Soluciones mágicas (Nuestros usuarios quieren que aprete un botón y haga todo)

En muy importante clasificar el **tipo de error** que encontramos, para sumar antecedentes y ver en que área nos esta costando más.

- Lógica de backend
- Diseño de BBDD
- Diseño UX/UI

## Impacto De Riesgos

- El impacto más drástico es que se llegue a la cancelación del proyecto.
- Baja de moral
- Daño a la imagen del equipo o empresa
- Problemas legales

## Gestión De Riesgo Ágil

Un scrum master puede manejar riesgos para la organización del equipo

Un integrante del equipo de scrum puede manejar riesgos del delivery o del proceso

Un P.O puede manejar riesgos financieros o riesgos del producto

## Actitud Para la Administración De Riesgos

**Proactividad**
- Anticipar problemas
- Dirigirse a las causas
- Prevenir y minimizar los riesgos via mitigarlos
- Prepararse para las consecuencias a fin de minimizar el impacto
- Utilizar un proceso ordenado y conocido

**Crisis**
- Arreglar los problemas cuando ocurren
- Dirigirse a los síntomas
- Reaccionar ante las consecuencias

### Administración Proactiva De Riesgos

En la etapa de visión puede mostrar riesgos para el negocio

En la etapa de diseño puede mostrar riesgos técnicos.

Todo el proyecto puede mostrar riesgos de organización.

### Proceso De Administración De Riesgos

Identificar, Analizar, Planificar, Seguir, Controlar

![[Pasted image 20250318191000.png]]

## Identificación De Riesgo

Forma de expresar el riesgo

Condición -> Consecuencia

Si sucede que se va nuestro P.O vamos a tener un impacto alto en el proyecto

## Dos Aspectos Del Riesgo

Cualitativo, Analizar la probabilidad de que ocurra y el impacto, se puede usar una matriz de riesgo en donde

Formas de medir la probabilidad:

- Alta, Media o Baja
Le asignamos un valor a cada medida, Por ej 1 a 3.

Formas de medir la severidad:

Asignamos un valor que mida la seriedad de que algo ocurra.

con estos datos podemos crear una matriz de evaluación de riesgos.

$$\text{Exposición} = \text{Probabilidad} \cdot Severidad$$

| Descripción                                                     | Prob. ocurrencia | Severidad | Exposición | Mitigacion                                        | Contingencia                                        |
| --------------------------------------------------------------- | ---------------- | --------- | ---------- | ------------------------------------------------- | --------------------------------------------------- |
| Desarrollador Andres, no disponible por prioridad de proyecto 5 | 3                | 3         | 9          | Avanzar diseño para comenzar desarrollo           | Reasignar a Pablo a las tareas de Andrés            |
| Cambios regulatorios por ajuste a inflación                     | 2                | 3         | 6          | Consultar a legales sobre expectativas de cambio. | Programas de ajuste de precios externos al SIstema. |

## Planes Frente a Los Riesgos

**Plan de mitigación**

Planificar y tomas las acciones necesarias de antemano para llevar la exposición del riesgo a un nivel aceptable

**Plan de contingencia**

*Buscar definición*


