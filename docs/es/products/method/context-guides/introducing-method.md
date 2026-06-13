# Escenario "Introducir Method"

Los escenarios donde puedes "introducir Method" (*Introducing Method Scenarios* en inglés) son contextos de trabajo donde un equipo u organización no usa actualmente *VSlices Method*, pero está abierto a mejorar cómo el conocimiento, las decisiones, la implementación y el *feedback* se mantienen conectados.

El objetivo no es adoptar todo el método de una vez. Es introducir una costura útil de continuidad.

## Idea central

*VSlices Method* debería introducirse a través de trabajo real. Un equipo no debería comenzar cambiando todo su proceso. Debería comenzar preservando una pieza de conocimiento de la que depende el trabajo actual o futuro.

La pregunta no es *¿Cómo adoptamos VSlices Method?*, es: **¿Dónde se está perdiendo continuidad actualmente?**

## Cuándo aplica esta guía

Usa esta guía cuando:

* el trabajo ya está ocurriendo
* el equipo tiene su propio proceso
* existe documentación, pero está desconectada de la implementación
* se toman decisiones, pero no se preservan
* los *tickets* describen tareas sin suficiente intención
* aparece *feedback*, pero no cambia el trabajo futuro
* aparece confusión repetida entre personas o equipos
* el equipo está abierto a una mejora liviana

Esta guía no es para reemplazar cómo trabaja un equipo. Es para hacer que el trabajo existente sea más continuo.

## Riesgo principal

El riesgo principal es intentar introducir *VSlices Method* como un proceso completo. Eso puede crear resistencia, ceremonia o falsa madurez.

Puede que un equipo no necesite nuevas etapas, reuniones o *templates*. Puede que solo necesite una mejor forma de preservar:

* por qué importa un cambio
* qué contexto lo sostiene
* qué decisión se tomó
* qué sigue siendo incierto
* qué *feedback* cambió
* qué no debería redescubrir el trabajo futuro

*Method* debería entrar a través de utilidad, no de doctrina.

## Modalidad inicial útil

Introducir *Method* normalmente comienza con *Problem-First* o *Slice-First*.

| Situación                                                                                   | Modalidad útil                                                        | Razón                                                                                |
| ------------------------------------------------------------------------------------------- | --------------------------------------------------------------------- | ------------------------------------------------------------------------------------ |
| El equipo siente un dolor repetido, pero no sabe dónde se está rompiendo la continuidad.    | [***Context-First***](../../design/modalities/context-first/index.md) | El equipo necesita entender la pérdida de continuidad antes de cambiar cómo trabaja. |
| Un artefacto o práctica pequeña puede mejorar inmediatamente el trabajo en curso.           | [***Problem-First***](../../design/modalities/problem-first/index.md) | El equipo puede validar *Method* mediante una mejora acotada.                        |
| El contexto de trabajo circundante es demasiado poco claro para intervenir de forma segura. | [***Slice-First***](../../design/modalities/slice-first/index.md)     | El equipo necesita un entendimiento más amplio antes de introducir un cambio.        |

La modalidad seleccionada debería coincidir con la incertidumbre de adopción, no con una preferencia personal.

## Qué observar primero

Antes de sugerir prácticas de *Method*, observa cómo se mueve actualmente el trabajo. Algunas preguntas útiles incluyen:

* ¿Dónde se pierde intención?
* ¿Dónde las personas repiten las mismas explicaciones?
* ¿Dónde se toman decisiones?
* ¿Dónde se olvidan las decisiones?
* ¿Dónde la documentación deja de coincidir con la realidad?
* ¿Dónde la implementación pierde contexto de negocio?
* ¿Dónde desaparece el *feedback*?
* ¿Qué *handoffs* crean confusión?
* ¿Qué pequeña mejora ayudaría inmediatamente al trabajo actual?

El objetivo no es juzgar el proceso del equipo. Es encontrar una brecha de continuidad que valga la pena mejorar.

## Puntos de continuidad

Un punto de continuidad (*continuity seam* en inglés) es un lugar pequeño donde *Method* puede conectar conocimiento que actualmente está desconectado. Algunas puntos útiles pueden incluir:

* agregar contexto a un ítem de trabajo activo
* registrar una decisión importante
* clarificar un término de dominio ambiguo
* preservar un resultado de validación
* conectar un caso de uso con un cambio de implementación
* documentar una excepción de *workflow*
* capturar una incertidumbre antes de construir
* revisar un supuesto obsoleto después de recibir *feedback*

Un punto es útil cuando ayuda a que el trabajo real continúe con menos adivinanza.

## Soporte documental

Los documentos pueden apoyar la introducción de *Method*, pero solo cuando resuelven un problema actual de continuidad.

| Brecha de continuidad                                          | Documento útil                                                                                                                                                                                                      |
| -------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Las personas usan el mismo término con significados distintos. | Vocabulario de dominio (*Domain Vocabulary*) — [Taxonomía](../../docs-standard/taxonomy/domain-vocabulary.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/domain-vocabulary.md)       |
| Una tarea carece de contexto circundante.                      | Documento de contexto (*Context Document*) — [Taxonomía](../../docs-standard/taxonomy/context-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/context-document.md)           |
| Un *workflow* o *handoff* se malentiende.                      | Documento de proceso (*Process Document*) — [Taxonomía](../../docs-standard/taxonomy/process-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/process-document.md)            |
| Un comportamiento necesita intención más clara.                | Documento de caso de uso (*Use Case Document*) — [Taxonomía](../../docs-standard/taxonomy/use-case-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/use-case-document.md)     |
| Una capacidad estable necesita ser nombrada.                   | Documento de capacidad (*Capability Document*) — [Taxonomía](../../docs-standard/taxonomy/capability-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/capability-document.md) |
| Una decisión puede afectar el trabajo futuro.                  | Registro de decisión (*Decision Record*) — [Taxonomía](../../docs-standard/taxonomy/decision-record.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/decision-record.md)               |
| El *feedback* debería cambiar lo que ocurre después.           | Nota de validación (*Validation Note*) — [Taxonomía](../../docs-standard/taxonomy/validation-note.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/validation-note.md)                 |
| Una observación es útil, pero todavía incierta.                | Nota de soporte (*Support Note*) — [Taxonomía](../../docs-standard/taxonomy/support-note.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/support-note.md)                             |

No introduzcas documentos como paquete. Introduce el documento más pequeño que proteja el trabajo actualmente en riesgo.

> La afinidad documento-etapa (*Document-Stage affinity*) se describe en la página [afinidad documento-etapa](../document-stage-affinity.md).

## Enfoque sugerido

Comienza con trabajo en curso. No pauses el proyecto para introducir *Method*. Un enfoque útil es:

1. Elegir un ítem de trabajo, problema o decisión activa.
2. Identificar dónde la continuidad es débil.
3. Agregar la estructura útil más pequeña de *Method*.
4. Usarla durante trabajo real.
5. Observar si ayuda a las personas a tomar mejores decisiones.
6. Preservar el aprendizaje.
7. Decidir si vale la pena introducir otra costura.

*Method* debería crecer solo donde siga demostrando utilidad.

## Errores comunes

Introducir *Method* puede fallar cuando el método se vuelve más importante que el trabajo. Algunos errores comunes incluyen:

* introducir demasiados documentos a la vez
* pedir a las personas que cambien todo su proceso inmediatamente
* explicar *Method* antes de resolver un problema real
* tratar los *templates* como el valor
* crear documentación que nadie usa
* reemplazar conversación con artefactos
* ignorar prácticas existentes del equipo
* forzar terminología de *VSlices* antes de que ayude
* medir adopción en vez de continuidad

El primer objetivo no es adopción, es utilidad.

## Principio guía

Introduce *VSlices Method* mediante una costura útil de continuidad. Preserva una pieza de conocimiento de la que depende el trabajo futuro.

Si eso ayuda, repite. Si no ayuda, reduce la estructura hasta que ayude.
