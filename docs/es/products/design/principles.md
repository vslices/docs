# Principios de VSlices Design

VSlices Design usa modalidades para adaptar el proceso de diseño a distintos tipos de incertidumbre.

Una modalidad no es una metodología rígida. Es una forma de decidir cuánta comprensión, contexto, planificación y feedback de implementación necesita un equipo antes de avanzar.

- Algunas situaciones requieren una base contextual amplia antes de definir artefactos de software.
- Algunas situaciones requieren un análisis de problema enfocado.
- Algunas situaciones requieren una pequeña vertical slice para aprender de la implementación lo antes posible.

VSlices Design usa dos metáforas complementarias para explicar este movimiento:

- la pirámide invertida: explica cómo el equipo entiende un negocio.
- la pirámide de construcción: explica cómo el equipo convierte ese entendimiento en valor.

Juntas, ambas metáforas describen la idea central de VSlices Design:

> Antes de construir artefactos de software, el equipo debe entender de dónde viene su material.

Una feature no debería aparecer como una decisión aislada; debería construirse a partir de granos de entendimiento del dominio que fueron descubiertos, seleccionados, moldeados y colocados con intención.

La pirámide es la geometría inicial usada por VSlices Design porque representa entendimiento acumulado. Otras geometrías pueden explorarse en el futuro cuando distintas restricciones del dominio requieran distintas herramientas de razonamiento.

## La pirámide invertida

La pirámide invertida representa el negocio como una superficie amplia de conocimiento de dominio.

La punta estrecha está en la parte inferior, la base ancha está en la parte superior, y allí hay muchos granos de arena:

- concepts
- words
- actors
- areas
- departments
- roles
- flows
- rules
- exceptions
- assumptions
- problems
- opportunities
- business signals

Esos granos dan forma al negocio. Pero no todos son igual de relevantes para el objetivo actual.

Para entender el negocio, el equipo debe quitar los granos que cubren el área que se está explorando, pero quitar granos no significa eliminarlos.

Significa entenderlos, descubrir qué son, cómo se relacionan entre sí, por qué existen y si importan para el objetivo actual.

Cuanto más profundo va el equipo, más precisa se vuelve la comprensión. En la superficie, el equipo puede reconocer solo vocabulario y actores.

Más abajo, el equipo empieza a encontrar flows, responsabilidades, reglas, puntos de dolor, riesgos y posibles cambios.

Más abajo todavía, el equipo puede descubrir la forma de use cases, procesos, capabilities, services y features.

La pirámide invertida es la metáfora del descubrimiento; explica de dónde viene la arena.

## La pirámide de construcción

Una vez que el equipo ha extraído suficiente arena del contexto de negocio, puede empezar a construir.

La pirámide de construcción representa cómo el entendimiento del dominio se convierte en valor de negocio.

La primera iteración crea la base inicial de la pirámide. Esa base es importante porque da al equipo una sensación temprana de:

* cuán grande puede ser el dominio
* cuántas áreas o actores están involucrados
* cuánta incertidumbre existe
* dónde pueden aparecer los primeros límites
* qué partes del dominio pueden requerir exploración más profunda

Una pirámide grande necesita una base fuerte.

De la misma manera, un sistema grande o complejo necesita suficiente entendimiento contextual antes de que el equipo empiece a definir artefactos de software precisos. Cada nueva iteración añade más arena al sitio de construcción.

Pero cada grano tiene un significado diferente según dónde caiga.

- Si cae cerca de la base, puede representar nuevo entendimiento del dominio.
- Si cae un poco por encima de la base, puede representar un flow recién descubierto o un proceso adyacente.
- Si cae alrededor del medio, puede convertirse en un use case, una definición de proceso o un límite de responsabilidad.
- Si cae cerca de la parte superior, puede indicar la necesidad de un service, capability o component formal.
- Si llega a la punta, puede convertirse en una feature concreta lista para implementarse y entregarse.

La pirámide de construcción es la metáfora de la composición; explica cómo el entendimiento se convierte en valor.

## De la extracción a la construcción

VSlices Design se mueve entre ambas pirámides.

> Primero, el equipo extrae arena de la pirámide invertida.
>
> Luego, el equipo coloca esa arena en la pirámide de construcción.

El movimiento es:

1. Descubrir conocimiento del dominio.
2. Entender qué importa.
3. Organizar el conocimiento descubierto.
4. Dar forma a las ideas a partir de ese conocimiento.
5. Convertir ideas en artefactos de diseño.
6. Usar esos artefactos para guiar la implementación.
7. Entregar valor de negocio.

El equipo no debería construir la pirámide de construcción con arena aleatoria.

No debería crear features, services, screens, APIs o components solo porque parezcan plausibles. Esos artefactos necesitan respaldo.

Deben construirse a partir de material de negocio entendido.

## Por qué importan ambas pirámides

Un equipo puede intentar construir solo la parte superior de la pirámide de construcción.

Puede empezar directamente desde features, services, screens, APIs o estructuras de base de datos. A veces esto funciona, especialmente en dominios pequeños o bien conocidos.

Pero en dominios poco claros, manuales, fragmentados, heredados o complejos organizacionalmente, esto crea riesgo.

Sin suficiente base, los artefactos se apilan sin soporte. Pueden parecer progreso, pero son inestables o no están relacionados.

A medida que aparece más conocimiento, esos artefactos pueden colapsar, moverse, dividirse o necesitar ser reconstruidos en otro lugar.

VSlices Design existe para reducir ese riesgo.

No rechaza features, services, screens, APIs o componentes técnicos. Se niega a tratarlos como punto de partida cuando el dominio todavía no está claro.

## Base y altura

La pirámide de construcción tiene dos dimensiones útiles: __base__ y __altura__

La base representa soporte contextual; responde preguntas como:

- ¿Cuánto del dominio entendemos?
- ¿Cuánto contexto circundante necesitamos?
- ¿Qué conceptos, actores, flows y límites respaldan el objetivo actual?
- ¿Cuánta incertidumbre debería reducirse antes de construir?

La altura representa el movimiento hacia implementaciones concretas y responde preguntas como:

- ¿Qué tan rápido nos movemos hacia una feature?
- ¿Qué tan pronto validamos mediante implementación?
- ¿Qué tan concreto necesita ser el resultado de la iteración?
- ¿Cuánto valor podemos entregar con el entendimiento actual?

VSlices Design usa modalidades porque distintas situaciones necesitan proporciones distintas entre base y altura.

## Proporción de modalidad

Una modalidad de VSlices Design define la proporción entre base contextual y altura de implementación. No compiten; solo responden a distintos tipos de incertidumbre y contextos.

Las etapas son similares entre modalidades, pero cambia el énfasis. Una modalidad responde: _¿Cuánta base necesitamos antes de subir?_ 

> Context-First prioriza la base.
> Problem-First busca equilibrio entre base y altura.
> Slice-First prioriza la altura.

## Una forma simple de pensar las modalidades

Una modalidad puede entenderse mediante la relación entre base y altura:

```text
base / height
```

Context-First tiende hacia una base grande:

```text
base / height -> large
```

Problem-First tiende al equilibrio:

```text
base / height -> balanced
```

Slice-First tiende hacia una altura rápida:

```text
base / height -> small
```

Es una heurística de diseño que ayuda al equipo a razonar cuánta comprensión se necesita antes de avanzar hacia la construcción.

Y es una heurística que también implica que puedes cambiar de modalidad después de cada iteración.

## Principio central

VSlices Design sigue un principio simple:

> Entender el material de negocio antes de construir la estructura de software.

La pirámide invertida ayuda al equipo a entender el negocio; la pirámide de construcción ayuda al equipo a convertir ese entendimiento en valor.

Las modalidades ayudan al equipo a decidir cuánta comprensión se necesita antes de avanzar hacia la implementación.
