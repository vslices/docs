# Escenario "Unirse a un proyecto existente"

Un escenario "Unirse a un proyecto existente" es un contexto de trabajo donde una persona o equipo entra a un trabajo que ya está en curso.

El proyecto puede usar VSlices Method, o puede usar otra forma de trabajo.

El objetivo no es reiniciar el proyecto. Es unirse al camino de continuidad actual antes de cambiar el trabajo.

## Idea central

!!! principle "Principio de Continuidad"

    Unirse a un proyecto existente no debería comenzar solo desde tareas.

Las tareas describen lo que alguien debería hacer, pero no siempre explican por qué importa el trabajo, qué contexto lo sostiene, qué decisiones le dieron forma o qué feedback lo cambió.

La pregunta no es *¿Qué tareas deberíamos tomar?*, sino *¿de qué camino de continuidad forman parte estas tareas?*.

## Cuándo aplica esta guía

Usa esta guía cuando:

* una persona nueva se une a un proyecto
* un equipo nuevo se une a una iniciativa en curso
* el trabajo ya está planificado o en progreso
* existen decisiones que afectan el trabajo actual
* existe documentación, pero necesita interpretación
* existe implementación, pero la intención no está clara
* el proyecto tiene stakeholders, usuarios o restricciones operativas activas
* el equipo necesita contribuir sin perder el contexto original

Esta guía aplica tanto cuando una persona se incorpora a un proyecto existente como cuando un equipo completo entra a trabajo ya iniciado.

## Riesgo principal

El riesgo principal es entrar por ejecución sin entender la intención.

Esto puede crear:

* cambios que resuelven una tarea, pero no el problema
* descubrimiento duplicado
* decisiones repetidas
* implementación que contradice el contexto previo
* documentación que ignora conocimiento existente
* feedback desconectado del trabajo actual
* mejoras locales que debilitan el sistema completo

Un proyecto en curso ya tiene historia. Parte de esa historia es conocimiento útil; otra parte puede estar desactualizada o ser accidental.

!!! risk "Riesgo a evitar"

    Antes de contribuir, el equipo necesita distinguir qué continuidad debe respetarse, qué decisiones deben revisarse y qué complejidad no debería heredarse.


## Modalidad inicial útil

Introducir Method en un proyecto en curso debería comenzar desde la incertidumbre que más está afectando el trabajo.

| Situación                                                                  | Modalidad útil                                                      | Razón                                                                          |
| -------------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------------------ |
| El equipo no entiende dónde se está perdiendo continuidad.                 | [**Context-First**](../../design/modalities/context-first/index.md) | El equipo necesita entender el contexto antes de cambiar cómo trabaja.         |
| Existe un dolor claro en la forma actual de trabajar.                      | [**Problem-First**](../../design/modalities/problem-first/index.md) | El equipo puede introducir Method resolviendo una fricción concreta.           |
| Una práctica pequeña puede mejorar el trabajo sin cambiar todo el proceso. | [**Slice-First**](../../design/modalities/slice-first/index.md)     | El equipo puede validar Method mediante una intervención acotada y observable. |

!!! risk "Riesgo a evitar"

    La modalidad elegida debería responder a la incertidumbre de adopción, no a la preferencia personal del equipo.


## Qué observar primero

Antes de sugerir prácticas de Method, observa cómo se mueve actualmente el trabajo.

| Observa                                                    | Para entender                                                   |
| ---------------------------------------------------------- | --------------------------------------------------------------- |
| Dónde se pierde intención                                  | Qué parte del trabajo deja de explicar por qué importa.         |
| Dónde las personas repiten las mismas explicaciones        | Qué conocimiento depende demasiado de memoria o conversación.   |
| Dónde se toman decisiones                                  | Qué momentos necesitan preservar contexto.                      |
| Dónde se olvidan decisiones                                | Qué continuidad se pierde entre decisión y trabajo futuro.      |
| Dónde la documentación deja de coincidir con la realidad   | Qué documentos necesitan actualización, reducción o reemplazo.  |
| Dónde la implementación pierde contexto de negocio         | Qué comportamiento necesita recuperar intención.                |
| Dónde desaparece el feedback                               | Qué aprendizaje no está cambiando decisiones futuras.           |
| Qué handoffs crean confusión                               | Dónde se rompe la continuidad entre personas, equipos o etapas. |
| Qué pequeña mejora ayudaría al trabajo actual de inmediato | Dónde Method puede entrar con utilidad real y poco peso.        |

El objetivo no es juzgar el proceso del equipo. Es encontrar una brecha de continuidad que valga la pena mejorar.

## Conocimiento a preservar

Unirse a un proyecto existente puede revelar continuidad ausente o frágil.

Preserva conocimiento cuando ayude a quienes se incorporan o al trabajo futuro a evitar suposiciones.

El conocimiento útil puede incluir:

* vocabulario del proyecto que no es obvio
* decisiones que explican la implementación actual
* supuestos activos
* restricciones conocidas
* límites actuales de flujo de trabajo o caso de uso
* resultados de validación que dieron forma a la dirección actual
* diferencias entre la intención documentada y la implementación real
* preguntas de onboarding que revelan conocimiento oculto
* conocimiento desactualizado que debería revisarse

!!! principle "Principio de Continuidad"

    Las personas nuevas suelen exponer conocimiento implícito.

    Sus preguntas no deberían tratarse como interrupciones. Son señales de dónde la continuidad puede necesitar apoyo.


## Apoyo documental

| Necesidad de conocimiento | Documento útil |
| --- | --- |
| Los términos no son claros para quienes se incorporan. | Domain Vocabulary — [Taxonomy](../../docs-standard/taxonomy/domain-vocabulary.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/domain-vocabulary.md) |
| El escenario circundante necesita orientación. | Context Document — [Taxonomy](../../docs-standard/taxonomy/context-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/context-document.md) |
| El trabajo actual depende de workflows o handoffs. | Process Document — [Taxonomy](../../docs-standard/taxonomy/process-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/process-document.md) |
| Un comportamiento necesita aclarar intención y consecuencias. | Use Case Document — [Taxonomy](../../docs-standard/taxonomy/use-case-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/use-case-document.md) |
| Una habilidad estable explica varios cambios relacionados. | Capability Document — [Taxonomy](../../docs-standard/taxonomy/capability-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/capability-document.md) |
| La dirección existente depende de tradeoffs pasados. | Decision Record — [Taxonomy](../../docs-standard/taxonomy/decision-record.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/decision-record.md) |
| El feedback reciente cambió el entendimiento actual. | Validation Note — [Taxonomy](../../docs-standard/taxonomy/validation-note.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/validation-note.md) |
| Las preguntas u observaciones todavía son inciertas. | Support Note — [Taxonomy](../../docs-standard/taxonomy/support-note.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/support-note.md) |

Usa documentos para unirte al trabajo, no para auditar todo el proyecto.

{% include-markdown "shared/readings/document-stage-affinity-admonition.md" %}

## Enfoque sugerido

Comienza con el trabajo activo. No intentes entenderlo todo antes de contribuir.

Un enfoque útil es:

1. Identificar el elemento de trabajo, caso de uso, capacidad o línea de trabajo actual.
2. Encontrar el contexto y las decisiones que explican por qué existe.
3. Entender la etapa actual de la iteración.
4. Aclarar qué se sabe, qué es incierto y qué ya fue decidido.
5. Contribuir a una parte pequeña del trabajo.
6. Preservar el conocimiento faltante descubierto durante la incorporación.
7. Devolver el feedback al contexto compartido.

El equipo debería entrar por continuidad y luego contribuir mediante entrega.

## Errores comunes

Unirse a trabajo existente suele fallar cuando la ejecución comienza antes que la orientación. Algunos errores comunes incluyen:

* comenzar desde tickets sin entender la intención
* reescribir contexto que ya existe
* ignorar decisiones previas
* tratar decisiones antiguas como siempre correctas
* tratar decisiones antiguas como siempre incorrectas
* cambiar implementación sin saber quién depende de ella
* pedir documentación completa antes de contribuir
* mantener preguntas de onboarding en privado
* crear documentos nuevos que duplican conocimiento existente

Los proyectos existentes necesitan respeto y curiosidad. No obediencia ciega. No reemplazo heroico.

## Principio guía

!!! principle "Principio de Continuidad"

    Únete al camino de continuidad antes de unirte a la lista de tareas.

Entiende suficiente contexto, decisiones, comportamiento y feedback para contribuir sin romper la intención.

Preserva el conocimiento que te ayudó a incorporarte, para que la siguiente persona no tenga que redescubrirlo.
