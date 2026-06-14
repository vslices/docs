# Escenario "Unirse a un proyecto existente"

Los escenarios de "unirse a un proyecto existente" (*Joining Existing Project Scenarios* en inglés) son contextos de trabajo donde una persona o equipo entra a trabajo que ya está en progreso. El proyecto puede que ya use *VSlices Method* o puede que use otra forma de trabajo.

El objetivo no es reiniciar el proyecto. Es incorporarse al camino de continuidad actual antes de cambiar el trabajo.

## Idea central

Incorporarse a un proyecto existente no debería comenzar solo desde tareas. Las tareas describen qué debería hacer alguien. Pero no siempre explican:

* por qué el trabajo importa
* qué contexto lo sostiene
* qué decisiones le dieron forma
* qué *feedback* lo cambió

La pregunta no es *¿Qué tareas deberíamos tomar?*, es: **¿De qué camino de continuidad forman parte estas tareas?**.

## Cuándo aplica esta guía

Usa esta guía cuando:

* una nueva persona se incorpora a un proyecto
* un nuevo equipo se incorpora a una iniciativa en curso
* el trabajo ya está planificado o en progreso
* decisiones existentes afectan el trabajo actual
* existe documentación, pero necesita interpretación
* existe implementación, pero la intención no está clara
* el proyecto tiene *stakeholders*, usuarios o restricciones operacionales activas
* el equipo necesita contribuir sin perder el contexto original

Esta guía aplica tanto si el proyecto es nuevo para una persona como si es nuevo para todo el equipo.

## Riesgo principal

El riesgo principal es entrar a través de ejecución sin entender intención. Esto puede crear:

* cambios que resuelven una tarea, pero no el problema
* descubrimiento duplicado
* decisiones repetidas
* implementación que viola contexto previo
* documentación que ignora conocimiento existente
* *feedback* desconectado del trabajo actual
* mejoras locales que debilitan el sistema completo

Un proyecto en progreso ya tiene historia. Parte de esa historia es conocimiento útil; parte puede estar desactualizada o ser accidental.

El equipo debería entender lo suficiente para distinguir la diferencia.

## Modalidad inicial útil

Incorporarse a un proyecto existente no siempre requiere elegir una nueva modalidad. Primero, identifica el contexto de trabajo actual.

| Situación                                                                                                   | Modalidad útil                                                        | Razón                                                                                       |
| ----------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- |
| El contexto, los límites o<br/>la historia del proyecto no<br/>están claros.                                        | [***Context-First***](../../design/modalities/context-first/index.md) | El equipo necesita entender la continuidad<br/>circundante antes de actuar.                     |
| El trabajo actual está<br/>centrado en un dolor<br/>conocido o una decisión<br/>activa.                                 | [***Problem-First***](../../design/modalities/problem-first/index.md) | El equipo necesita entender el problema detrás<br/>de las tareas.                               |
| El proyecto tiene suficiente<br/>contexto y una contribución<br/>pequeña puede producir<br/>*feedback* de forma segura. | [***Slice-First***](../../design/modalities/slice-first/index.md)     | El equipo puede aprender contribuyendo un<br/>cambio acotado.                                   |
| El proyecto ya tiene una<br/>modalidad activa.                                                                  | Continuar la<br/>modalidad actual                                         | El equipo debería incorporarse al camino de<br/>continuidad actual antes de cambiar el énfasis. |

La primera responsabilidad es orientarse. Cambiar de modalidad demasiado pronto puede reiniciar trabajo innecesariamente.

## Qué observar primero

Antes de contribuir, observa cómo está conectado el trabajo actual. Algunas preguntas útiles incluyen:

* ¿Qué escenario o línea de trabajo está activa?
* ¿Qué problema u oportunidad se está abordando?
* ¿Qué decisiones ya dan forma a la dirección actual?
* ¿Qué documentos o conversaciones preservan el contexto actual?
* ¿Qué implementación ya existe?
* ¿Qué *feedback* ha cambiado recientemente el trabajo?
* ¿Qué sigue siendo incierto?
* ¿Quién depende del comportamiento actual?
* ¿Qué restricciones son técnicas, de negocio u operacionales?
* ¿Qué partes del trabajo todavía están siendo validadas?

El objetivo no es aprender todo el proyecto. Es entender el camino de continuidad del trabajo al que se está incorporando.

## Conocimiento a preservar

Incorporarse a un proyecto existente puede revelar continuidad faltante o frágil.

Preserva conocimiento cuando ayude a nuevos contribuidores o al trabajo futuro a evitar adivinar. El conocimiento útil puede incluir:

* vocabulario del proyecto que no es obvio
* decisiones que explican la implementación actual
* supuestos activos
* restricciones conocidas
* límites actuales del *workflow* o caso de uso
* resultados de validación que dieron forma a la dirección actual
* diferencias entre la intención documentada y la implementación real
* preguntas de *onboarding* que revelan conocimiento oculto
* conocimiento desactualizado que debería revisarse

Quienes se incorporan suelen exponer conocimiento implícito. Esas preguntas no deberían tratarse como interrupciones. Son señales de **dónde la continuidad puede necesitar soporte**.

## Soporte documental

| Necesidad de conocimiento                                        | Documento útil                                                                                                                                                                                                      |
| ---------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Los términos no están claros<br/>para quienes se incorporan.         | Vocabulario de dominio — [Taxonomía](../../docs-standard/taxonomy/domain-vocabulary.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/domain-vocabulary.md)       |
| El escenario circundante<br/>necesita orientación.                   | Documento de contexto — [Taxonomía](../../docs-standard/taxonomy/context-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/context-document.md)           |
| El trabajo actual depende de<br/>*workflows* o *handoffs*.           | Documento de proceso — [Taxonomía](../../docs-standard/taxonomy/process-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/process-document.md)            |
| Un comportamiento necesita<br/>clarificar intención y consecuencias. | Documento de caso de uso — [Taxonomía](../../docs-standard/taxonomy/use-case-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/use-case-document.md)     |
| Una capacidad estable explica<br/>varios cambios relacionados.       | Documento de capacidad — [Taxonomía](../../docs-standard/taxonomy/capability-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/capability-document.md) |
| La dirección existente depende<br/>de *tradeoffs* pasados.           | Registro de decisión — [Taxonomía](../../docs-standard/taxonomy/decision-record.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/decision-record.md)               |
| *Feedback* reciente cambió el<br/>entendimiento actual.              | Nota de validación — [Taxonomía](../../docs-standard/taxonomy/validation-note.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/validation-note.md)                 |
| Las preguntas u observaciones<br/>todavía son inciertas.             | Nota de soporte — [Taxonomía](../../docs-standard/taxonomy/support-note.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/support-note.md)                             |

Usa documentos para incorporarte al trabajo, no para auditar todo el proyecto.

> La afinidad documento-etapa (*Document-Stage affinity*) se describe en la página [afinidad documento-etapa](../document-stage-affinity.md).

## Enfoque sugerido

Comienza con el trabajo activo. No intentes entenderlo todo antes de contribuir. Un enfoque útil es:

1. Identificar el ítem de trabajo, caso de uso, capacidad o línea de trabajo actual.
2. Encontrar el contexto y las decisiones que explican por qué existe.
3. Entender la etapa actual de la iteración.
4. Clarificar qué se sabe, qué es incierto y qué ya está decidido.
5. Contribuir a una parte pequeña del trabajo.
6. Preservar cualquier conocimiento faltante descubierto durante la incorporación.
7. Devolver el *feedback* al contexto compartido.

El equipo debería entrar a través de continuidad y luego contribuir mediante entrega.

## Errores comunes

Incorporarse a trabajo existente suele fallar cuando la ejecución comienza antes de la orientación. Algunos errores comunes incluyen:

* comenzar desde *tickets* sin entender intención
* reescribir contexto que ya existe
* ignorar decisiones previas
* tratar decisiones antiguas como siempre correctas
* tratar decisiones antiguas como siempre incorrectas
* cambiar implementación sin saber quién depende de ella
* pedir documentación completa antes de contribuir
* mantener privadas las preguntas de *onboarding*
* crear nuevos documentos que duplican conocimiento existente

Los proyectos existentes necesitan respeto y curiosidad. No obediencia ciega. No reemplazo heroico.

## Principio guía

Incorpórate al camino de continuidad antes de incorporarte a la lista de tareas. Entiende suficiente contexto, decisiones, comportamiento y *feedback* para contribuir sin romper intención.

Preserva el conocimiento que te ayudó a incorporarte, para que la siguiente persona no tenga que redescubrirlo.
