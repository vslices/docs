# Escenario "Introducir method"

Un escenario "Introducir method" es un contexto de trabajo donde un equipo u organización no usa actualmente VSlices Method, pero está abierto a mejorar cómo mantiene conectado el conocimiento, las decisiones, la implementación y el feedback.

El objetivo no es adoptar todo Method de una vez. Es introducir una costura útil de continuidad.

## Idea central

!!! principle "Principio de continuidad"

    VSlices Method debería introducirse desde trabajo que ya está ocurriendo.

Un equipo no debería comenzar cambiando todo su proceso. Debería comenzar preservando una pieza de conocimiento de la que depende el trabajo actual o futuro.

La pregunta no es *¿Cómo adoptamos VSlices Method?*, sino *¿dónde se está perdiendo continuidad ahora?*.

## Cuándo aplica esta guía

Usa esta guía cuando:

* el trabajo ya está ocurriendo
* el equipo ya tiene una forma de trabajo
* existe documentación, pero está desconectada de la implementación
* se toman decisiones, pero no se preservan
* los tickets describen tareas sin intención suficiente
* el feedback aparece, pero no cambia el trabajo futuro
* aparece confusión repetida entre personas o equipos
* el equipo está abierto a una mejora liviana

Esta guía no busca reemplazar la forma de trabajo del equipo. Busca hacer que el trabajo existente sea más continuo.

## Riesgo principal

El riesgo principal es intentar introducir VSlices Method como un proceso completo.

Eso puede crear resistencia, ceremonia innecesaria o una sensación falsa de madurez.

Un equipo puede no necesitar nuevas etapas, reuniones o plantillas. Puede necesitar una mejor forma de preservar:

* por qué importa un cambio
* qué contexto lo sostiene
* qué decisión fue tomada
* qué permanece incierto
* qué feedback cambió el trabajo
* qué trabajo futuro no debería tener que redescubrir

!!! risk "Riesgo a evitar"

    Method debería entrar por utilidad, no por doctrina.

Si no mejora una decisión real, una conversación real o un cambio real, probablemente se está introduciendo demasiado pronto o con demasiado peso.

## Modalidad inicial útil

Introducir Method en un proyecto en curso debería comenzar desde la incertidumbre que más está afectando el trabajo.

| Situación                                                                               | Modalidad útil                                                      | Razón                                                                                     |
| --------------------------------------------------------------------------------------- | ------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| El equipo siente dolor repetido, pero no sabe dónde se está rompiendo la continuidad.   | [**Context-First**](../../design/modalities/context-first/index.md) | El equipo necesita entender la pérdida de continuidad antes de cambiar cómo trabaja.      |
| Un artefacto o práctica pequeña puede mejorar el trabajo en curso de inmediato.         | [**Problem-First**](../../design/modalities/problem-first/index.md) | El equipo puede validar Method mediante una mejora acotada y útil.                        |
| El contexto de trabajo circundante es demasiado incierto para intervenir con seguridad. | [**Slice-First**](../../design/modalities/slice-first/index.md)     | El equipo necesita aprender mediante una intervención pequeña antes de ampliar el cambio. |

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

## Costuras de continuidad

Una costura de continuidad es un punto pequeño donde Method puede conectar conocimiento que hoy está desconectado.

Una costura útil puede consistir en:

* agregar contexto a un elemento de trabajo activo;
* registrar una decisión importante;
* aclarar un término ambiguo del dominio;
* preservar un resultado de validación;
* conectar un caso de uso con un cambio de implementación;
* documentar una excepción de flujo de trabajo;
* capturar una incertidumbre antes de construir;
* revisar un supuesto desactualizado después de recibir feedback.

!!! principle "Principio de Continuidad"

    Una costura es útil cuando ayuda al trabajo real a continuar con menos suposiciones.

    No necesita cambiar todo el proceso para mejorar la continuidad.


## Apoyo documental

Los documentos pueden ayudar a recuperar continuidad en un escenario digitalizado.

| Necesidad de conocimiento | Documento útil |
| --- | --- |
| Los términos son ambiguos o inconsistentes. | Domain Vocabulary — [Taxonomy](../../docs-standard/taxonomy/domain-vocabulary.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/domain-vocabulary.md) |
| El escenario de negocio circundante no está claro. | Context Document — [Taxonomy](../../docs-standard/taxonomy/context-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/context-document.md) |
| El trabajo actual depende de workflows o handoffs. | Process Document — [Taxonomy](../../docs-standard/taxonomy/process-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/process-document.md) |
| Un comportamiento específico necesita cambiarse o preservarse. | Use Case Document — [Taxonomy](../../docs-standard/taxonomy/use-case-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/use-case-document.md) |
| Está emergiendo una habilidad estable del negocio. | Capability Document — [Taxonomy](../../docs-standard/taxonomy/capability-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/capability-document.md) |
| Debe elegirse una dirección bajo tradeoffs. | Decision Record — [Taxonomy](../../docs-standard/taxonomy/decision-record.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/decision-record.md) |
| Evidencia desde uso, operación o revisión cambia el entendimiento. | Validation Note — [Taxonomy](../../docs-standard/taxonomy/validation-note.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/validation-note.md) |
| Las observaciones todavía son locales, inciertas o temporales. | Support Note — [Taxonomy](../../docs-standard/taxonomy/support-note.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/support-note.md) |

Usa el documento más liviano que proteja continuidad.

{% include-markdown "shared/readings/document-stage-affinity-admonition.md" %}

## Enfoque sugerido

Comienza con trabajo que ya está ocurriendo. No detengas el proyecto para introducir Method.

Un enfoque útil es:

1. Elegir un elemento de trabajo activo, problema o decisión.
2. Identificar dónde la continuidad es débil.
3. Agregar la estructura útil más pequeña de Method.
4. Usarla durante trabajo real.
5. Observar si ayuda a las personas a tomar mejores decisiones.
6. Preservar el aprendizaje.
7. Decidir si vale la pena introducir otra costura de continuidad.

Method debería crecer solo donde sigue demostrando utilidad.

## Errores comunes

Introducir Method puede fallar cuando el método se vuelve más importante que el trabajo.

Algunos errores comunes incluyen:

* introducir demasiados documentos a la vez;
* pedirle al equipo que cambie todo su proceso inmediatamente;
* explicar Method antes de resolver un problema real;
* tratar las plantillas como el valor;
* crear documentación que nadie usa;
* reemplazar conversaciones con artefactos;
* ignorar prácticas existentes del equipo;
* forzar terminología de VSlices antes de que ayude;
* medir adopción en vez de continuidad.

!!! risk "No confundas adopción con utilidad"

    El primer objetivo no es que el equipo adopte Method.

    Es que el trabajo gane continuidad suficiente para decidir, construir o aprender mejor.


## Principio guía

!!! principle "Principio de Continuidad"

    Introduce VSlices Method mediante una costura útil de continuidad.

Preserva una pieza de conocimiento de la que depende el trabajo futuro.

Si ayuda, repite. Si no ayuda, reduce la estructura hasta que ayude.

