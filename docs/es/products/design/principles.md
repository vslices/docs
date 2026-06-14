# Entender los principios de VSlices Design

VSlices Design usa modalidades para adaptar el proceso de diseño a distintos tipos de incertidumbre.

Una modalidad no es una metodología rígida; es una forma de decidir cuánto entendimiento, contexto, planificación y _feedback_ de implementación necesita un equipo antes de avanzar.

- Algunas situaciones requieren una base contextual amplia antes de definir artefactos de _software_.
- Algunas situaciones requieren análisis enfocado de un problema.
- Algunas situaciones requieren una pequeña _vertical slice_ para aprender desde la implementación lo antes posible.

VSlices Design usa dos metáforas complementarias para explicar este movimiento:

- la pirámide invertida: explica cómo el equipo entiende un negocio.
- la pirámide de construcción: explica cómo el equipo convierte ese entendimiento en valor.

Juntas, ambas metáforas describen la idea central de VSlices Design:

> Antes de construir artefactos de _software_, el equipo debe entender de dónde viene su material.

Una _feature_ no debería aparecer como una decisión aislada. Debería construirse desde granos de entendimiento de dominio que fueron descubiertos, seleccionados, moldeados y colocados con intención.

La pirámide es la geometría inicial usada por VSlices Design porque representa entendimiento acumulado. Otras geometrías pueden explorarse en el futuro cuando distintas restricciones de dominio requieran distintas herramientas de razonamiento.

## La pirámide invertida

La pirámide invertida representa el negocio como una superficie amplia de conocimiento de dominio.

La punta estrecha está abajo, la base amplia está arriba, y hay muchos granos de arena ahí:

- conceptos
- palabras
- actores
- áreas
- departamentos
- roles
- flujos
- reglas
- excepciones
- supuestos
- problemas
- oportunidades
- señales de negocio

Esos granos dan forma al negocio. Pero no todos son igualmente relevantes para el objetivo actual.

Para entender el negocio, el equipo debe retirar los granos que cubren el área explorada, pero retirar granos no significa eliminarlos.

Significa entenderlos, descubrir qué son, cómo se relacionan entre sí, por qué existen y si importan para el objetivo actual.

Mientras más profundo va el equipo, más preciso se vuelve el entendimiento. En la superficie, el equipo puede reconocer solo vocabulario y actores.

Más abajo, el equipo empieza a encontrar flujos, responsabilidades, reglas, puntos de dolor, riesgos y posibles cambios.

Todavía más abajo, el equipo puede descubrir la forma de casos de uso, procesos, capacidades, servicios y _features_.

La pirámide invertida es la metáfora del descubrimiento; explica de dónde viene la arena.

## La pirámide de construcción

Una vez que el equipo ha extraído suficiente arena del contexto de negocio, puede empezar a construir.

La pirámide de construcción representa cómo el entendimiento de dominio se convierte en valor de negocio.

La primera iteración crea la base inicial de la pirámide. Esta base es importante porque le da al equipo una percepción temprana de:

- qué tan grande puede ser el dominio
- cuántas áreas o actores están involucrados
- cuánta incertidumbre existe
- dónde pueden aparecer los primeros límites
- qué partes del dominio pueden requerir exploración más profunda

Una pirámide grande necesita una base fuerte.

De la misma forma, un sistema grande o complejo necesita suficiente entendimiento contextual antes de que el equipo empiece a definir artefactos precisos de _software_. Cada nueva iteración agrega más arena al sitio de construcción.

Pero cada grano tiene un significado distinto dependiendo de dónde cae.

- Si cae cerca de la base, puede representar nuevo entendimiento de dominio.
- Si cae ligeramente sobre la base, puede representar un flujo recién descubierto o un proceso adyacente.
- Si cae alrededor del centro, puede convertirse en un caso de uso, definición de proceso o límite de responsabilidad.
- Si cae cerca de la parte superior, puede indicar la necesidad de un servicio formal, capacidad o componente.
- Si alcanza la punta, puede convertirse en una _feature_ concreta lista para ser implementada y entregada.

La pirámide de construcción es la metáfora de la composición; explica cómo el entendimiento se convierte en valor.

## Desde extracción hacia construcción

VSlices Design se mueve entre ambas pirámides.

> Primero, el equipo extrae arena desde la pirámide invertida.
>
> Luego, el equipo coloca esa arena en la pirámide de construcción.

El movimiento es:

1. Descubrir conocimiento de dominio.
2. Entender qué importa.
3. Organizar el conocimiento descubierto.
4. Dar forma a ideas desde ese conocimiento.
5. Convertir ideas en artefactos de diseño.
6. Usar esos artefactos para guiar la implementación.
7. Entregar valor de negocio.

El equipo no debería construir la pirámide de construcción con arena aleatoria.

No debería crear _features_, servicios, pantallas, APIs o componentes solo porque parecen plausibles. Esos artefactos necesitan soporte.

Deberían construirse desde material de negocio entendido.

## Por qué ambas pirámides importan

Un equipo puede intentar construir solo la punta de la pirámide de construcción.

Puede empezar directamente desde _features_, servicios, pantallas, APIs o estructuras de base de datos. A veces esto funciona, especialmente en dominios pequeños o bien conocidos.

Pero en dominios poco claros, manuales, fragmentados, impulsados por legado u organizacionalmente complejos, esto crea riesgo.

Sin suficiente base, los artefactos se apilan sin soporte. Pueden parecer progreso, pero son inestables o no están relacionados.

A medida que aparece más conocimiento, esos artefactos pueden colapsar, moverse, dividirse o necesitar ser reconstruidos en otro lugar.

VSlices Design existe para reducir ese riesgo.

No rechaza _features_, servicios, pantallas, APIs o componentes técnicos. Se niega a tratarlos como punto de partida cuando el dominio todavía no está claro.

## Base y altura

La pirámide de construcción tiene dos dimensiones útiles: __base__ y __altura__.

La base representa soporte contextual. Responde preguntas como:

- ¿Cuánto del dominio entendemos?
- ¿Cuánto contexto circundante necesitamos?
- ¿Qué conceptos, actores, flujos y límites sostienen el objetivo actual?
- ¿Cuánta incertidumbre debería reducirse antes de construir?

La altura representa movimiento hacia implementaciones concretas. Responde preguntas como:

- ¿Qué tan rápido nos movemos hacia una _feature_?
- ¿Qué tan pronto validamos mediante implementación?
- ¿Qué tan concreto necesita ser el resultado de la iteración?
- ¿Cuánto valor podemos entregar desde el entendimiento actual?

VSlices Design usa modalidades porque distintas situaciones necesitan distintas proporciones entre base y altura.

## Proporción de modalidad

Una modalidad de VSlices Design define la proporción entre base contextual y altura de implementación. No compiten; solo responden a distintos tipos de incertidumbre y contextos.

Las etapas son similares entre modalidades, pero el énfasis cambia. Una modalidad responde: _¿Cuánta base necesitamos antes de movernos hacia arriba?_

> Context-First prioriza la base.
> Problem-First busca equilibrio entre base y altura.
> Slice-First prioriza la altura.

## Una forma simple de pensar las modalidades

Una modalidad puede entenderse mediante la relación entre base y altura:

```text
base / height
````

Context-First tiende hacia una base grande:

```text
base / height -> large
```

Problem-First tiende hacia el equilibrio:

```text
base / height -> balanced
```

Slice-First tiende hacia altura rápida:

```text
base / height -> small
```

Es una heurística de diseño que ayuda al equipo a razonar sobre cuánto contexto se necesita antes de moverse hacia la construcción.

Y es una heurística que también implica que puedes cambiar de modalidad después de cada iteración.

## Principio central

VSlices Design sigue un principio simple:

> Entender el material de negocio antes de construir la estructura de *software*.

La pirámide invertida ayuda al equipo a entender el negocio. La pirámide de construcción ayuda al equipo a convertir ese entendimiento en valor.

Las modalidades ayudan al equipo a decidir cuánto entendimiento se necesita antes de moverse hacia la implementación.
