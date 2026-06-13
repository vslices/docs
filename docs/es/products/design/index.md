# VSlices Design

VSlices Design ayuda a los equipos a decidir cuánta comprensión del dominio se necesita antes de convertir el conocimiento de negocio en software.

Proporciona modalidades de diseño, herramientas de razonamiento y heurísticas de modelado para pasar de material de negocio poco claro a decisiones de software más claras sin perder continuidad.

VSlices Design es intencionalmente independiente de VSlices Framework. No necesitas usar VSlices Framework para aplicar VSlices Design.

Framework puede ayudar más adelante a implementar algunas de las ideas descubiertas mediante Design, pero Design en sí mismo es un producto de razonamiento agnóstico al stack.

El propósito de VSlices Design es ayudar a los equipos a entender:

- qué contexto de negocio están trabajando
- cuánta incertidumbre existe
- qué tipo de enfoque de diseño es apropiado
- cómo el conocimiento del dominio se convierte en artefactos de software
- cuándo explorar ampliamente
- cuándo enfocarse en un problema específico
- cuándo aprender de una pequeña vertical slice

VSlices Design no asume que cada proyecto necesita la misma metodología.

Distintas situaciones requieren distintas formas de pasar del descubrimiento a la implementación.

## Propósito

Muchos proyectos de software comienzan desde artefactos que aparecen demasiado tarde en el proceso de razonamiento:

- user stories
- screens
- APIs
- database tables
- technical components
- implementation tasks

Estos artefactos son útiles, pero no siempre son el punto de partida correcto.

Cuando el dominio es poco claro, fragmentado, manual, heredado o complejo organizacionalmente, comenzar directamente desde la implementación puede crear complejidad accidental.

VSlices Design existe para reducir ese riesgo.

Su propósito es ayudar a los equipos a elegir la cantidad correcta de entendimiento, contexto, planificación y feedback de implementación antes de avanzar.

## ¿Qué problema resuelve?

Muchos equipos comienzan el diseño de software desde el primer artefacto visible:

- una screen
- una user story
- un endpoint
- una database table
- una tarea técnica
- una feature solicitada

Esos artefactos son útiles, pero a menudo aparecen después de que ya se omitieron preguntas importantes del dominio.

VSlices Design ayuda a los equipos a pausar antes de comprometerse demasiado pronto con una estructura.

Su pregunta principal es: ``` ¿Entendemos lo suficiente del material de negocio como para dar forma al software con seguridad?```

> A veces la respuesta requiere un descubrimiento contextual amplio.
> A veces requiere un análisis de problema enfocado.
> A veces requiere construir una pequeña vertical slice para aprender del feedback de la implementación.

VSlices Design ayuda a los equipos a elegir el punto de partida correcto para la incertidumbre que realmente enfrentan.

## ¿Cuándo debería usar VSlices Design?

Usa VSlices Design cuando el equipo necesite razonar sobre un sistema de software antes de decidir cómo debe construirse.

Es especialmente útil cuando el equipo enfrenta incertidumbre sobre el dominio, el problema, los límites o la forma de la solución. VSlices Design puede ayudar cuando:

- el contexto de negocio aún no está claro;
- el equipo no está seguro de dónde están los límites del sistema;
- los stakeholders describen soluciones antes de entender el problema subyacente;
- distintas personas usan palabras diferentes para el mismo concepto;
- el equipo necesita decidir cuánta exploración es necesaria antes de construir;
- el equipo quiere evitar diseñar arquitectura desde screens, tables, endpoints o tasks demasiado pronto;
- la implementación ya comenzó, pero el modelo de dominio todavía se siente inestable.

VSlices Design no solo es útil antes de la implementación. También puede usarse durante la implementación cuando aparece nuevo conocimiento del dominio, cuando una slice revela supuestos incorrectos o cuando el equipo se da cuenta de que la estructura actual ya no representa el negocio con claridad.

La pregunta principal es:

> ¿Entendemos lo suficiente del material de negocio como para dar forma con seguridad a la estructura del software?

Si la respuesta es no, VSlices Design ayuda al equipo a decidir qué tipo de entendimiento falta y qué modalidad podría ayudar después.

### Un ejemplo pequeño

Imagina que a un equipo se le pide automatizar un proceso interno de aprobación. Al principio, la solicitud suena simple:

> “Necesitamos una screen donde los managers puedan aprobar solicitudes.”

Si el equipo empieza desde la screen, la database table o el endpoint, podría codificar accidentalmente un proceso que aún no entiende.

Usando VSlices Design, el equipo pausa y pregunta qué tipo de incertidumbre está enfrentando.

Descubren que el problema real no es la screen de aprobación en sí. Distintos departamentos usan reglas de aprobación diferentes, algunas solicitudes requieren validación legal, algunas aprobaciones dependen de límites de presupuesto y algunos retrasos ocurren antes de que el manager siquiera reciba la solicitud.

En este caso, el equipo puede empezar con Context-First para entender el área de negocio antes de decidir qué estructura de software debe existir.

Más tarde, una vez que el contexto esté más claro, el equipo puede pasar a Problem-First para investigar por qué las aprobaciones son lentas.

Finalmente, una vez que una pequeña parte del proceso se entiende, el equipo puede usar Slice-First para construir y validar un flujo de aprobación acotado.

El objetivo no es retrasar la implementación, sino evitar construir software desde un entendimiento incompleto del material de negocio.

## Modalidades de diseño

VSlices Design usa modalidades para adaptar el proceso de diseño a distintos tipos de incertidumbre.

Una modalidad no es una metodología rígida. Es una forma de decidir cuánta base contextual se necesita antes de avanzar hacia la implementación. Las modalidades actuales de VSlices Design son:

- Context-First
- Problem-First
- Slice-First

Estas modalidades comparten el mismo flujo general de iteración:

```text
Understanding -> Contextualizing -> Planning -> Building -> Understanding
```

| Modality | Useful when | Starting question | Typical direction |
| --- | --- | --- | --- |
| Context-First | The domain is unclear, fragmented, manual, legacy-driven, or organizationally complex. | What business world are we entering? | Explore actors, processes, concepts, boundaries, language, responsibilities, and constraints. |
| Problem-First | The pain is visible, but the underlying cause or correct solution is still unclear. | What problem are we actually solving? | Clarify the problem, affected people, constraints, impact, alternatives, and candidate capabilities. |
| Slice-First | The team has enough clarity to build a small behavior and learn from it. | What useful behavior can we safely build now? | Implement a narrow vertical slice, validate assumptions, and use feedback to refine understanding. |

Lo que cambia es el énfasis.

## Mismo flujo, distinto énfasis

Las modalidades no compiten; responden a distintos tipos de incertidumbre.

Un equipo __no es__ “Context-First”, “Problem-First” o “Slice-First”. Un equipo __puede usar__ Context-First en una iteración, Problem-First __en la siguiente__ y Slice-First __una vez que se haya reducido suficiente incertidumbre__.

El flujo de iteración compartido sigue siendo el mismo:

```text
Understanding -> Contextualizing -> Planning -> Building -> Understanding
```

Lo que cambia es el énfasis.

- Context-First enfatiza entender el entorno de negocio antes de acotar la solución.
- Problem-First enfatiza clarificar un dolor específico antes de decidir qué construir.
- Slice-First enfatiza aprender de una pequeña implementación antes de expandir el modelo.

VSlices Design trata las modalidades como estrategias. No como identidades.

## Geometría del conocimiento

VSlices Design usa metáforas geométricas de forma intencional.

El modelo actual usa pirámides porque ayudan a explicar cómo el conocimiento del dominio se descubre, se compone y se transforma en valor de negocio.

La pirámide invertida representa el descubrimiento; ayuda a explicar cómo un equipo extrae entendimiento de un contexto de negocio amplio.

La pirámide de construcción representa la composición; ayuda a explicar cómo el conocimiento descubierto se convierte en ideas, artefactos, implementación y valor.

Esto no significa que todo dominio deba interpretarse siempre como una pirámide. La pirámide es la primera geometría útil porque representa entendimiento acumulado.

Las futuras versiones de VSlices Design pueden explorar otras metáforas geométricas cuando ayuden a explicar distintos tipos de restricciones del dominio.

Por ejemplo, un prisma puede ser útil cuando el conocimiento no fluye libremente porque está restringido por límites fuertes, regulaciones, sistemas heredados, silos organizacionales, contratos externos o responsabilidades fijas.

En ese sentido:

> Una pirámide explica cómo el conocimiento se convierte en valor.
> Un prisma explica qué impide que el conocimiento fluya libremente.

Estas geometrías no son metáforas decorativas.

Son herramientas de razonamiento.

Su propósito es ayudar a los equipos a entender cómo se comporta el conocimiento antes de decidir cómo debe diseñarse el software.

### Ejemplo: flujo de aprobación regulado

### Un ejemplo pequeño

Imagina que a un equipo se le pide automatizar la programación de citas para una pequeña red de clínicas. Al principio, la solicitud puede sonar simple:

> “Necesitamos una screen donde los pacientes puedan reservar citas.”

Pero el punto de partida correcto depende de la incertidumbre.

| Situation | Better starting modality | Why |
| --- | --- | --- |
| The team does not understand how clinics, professionals, rooms, availability, cancellations, and patient types interact. | Context-First | The domain is still unclear. Starting from a screen may hide important business rules. |
| The team knows the process, but the real pain is that patients miss appointments or staff spend too much time rescheduling manually. | Problem-First | The business problem is visible, but the solution should not be assumed too early. |
| The team already understands enough and wants to validate one useful behavior, such as sending a reminder 24 hours before an appointment. | Slice-First | A small behavior can be built safely and used to learn from real feedback. |
| The goal is not to delay implementation. The goal is to avoid building software from the wrong starting point. |  |  |

## Qué no es VSlices Design

VSlices Design no es una metodología universal. No afirma que todos los sistemas deban diseñarse de la misma manera. Y no asume que:

- Context-First es siempre correcto
- Problem-First es siempre correcto
- Slice-First es siempre correcto
- broad discovery es siempre requerido
- fast implementation es siempre mejor
- documentation es valiosa por defecto

VSlices Design valora la documentación solo cuando preserva la intención, reduce la ambigüedad o mejora la continuidad entre decisiones. El enfoque correcto depende de la incertidumbre, el riesgo, la madurez del dominio y la urgencia del negocio.

## Relación con la suite VSlices

VSlices Design es un producto dentro de la suite VSlices.

Se conecta con los otros productos, pero permanece independiente.

- VSlices Design proporciona las modalidades de diseño y las herramientas de razonamiento.
- VSlices Docs Standard puede proporcionar estructuras formales de documentación para preservar la intención descubierta.
- VSlices Method puede definir cómo se aplica el proceso de diseño a lo largo de un flujo de trabajo de ingeniería.
- VSlices Framework puede reflejar más adelante los conceptos resultantes como contexts, capabilities, features, flows, errors e integrations.

El objetivo es la continuidad.

El entendimiento del dominio no debería desaparecer cuando el equipo empieza a documentar.

La documentación no debería quedar desconectada de la arquitectura.

La arquitectura no debería quedar desconectada de la implementación.

La implementación debería seguir siendo trazable a la intención del negocio que la justificó.

## Principio central

VSlices Design sigue un principio simple: _Entender el material de negocio antes de construir la estructura de software_.

> A veces eso requiere un descubrimiento contextual amplio.
> A veces requiere un análisis de problema enfocado.
> A veces requiere una pequeña vertical slice.

La parte importante no es elegir la modalidad más sofisticada; es elegir la modalidad que encaja con la incertidumbre que el equipo realmente está enfrentando.
