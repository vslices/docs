# Documento de caso de uso

> Puedes acceder a la [plantilla de documento de caso de uso aquí](https://github.com/vslices/docs-standard/blob/main/templates/use-case-document.md)

Un Documento de caso de uso preserva el significado de un comportamiento dentro de un contexto de dominio.

Su propósito es describir qué significa una interacción, operación o comportamiento esperado, qué consecuencia produce y qué debe ser válido para que ese comportamiento tenga sentido. Un Documento de caso de uso responde:

> ¿Qué significa este comportamiento?

Un caso de uso no es solo una secuencia de pasos. Explica el resultado esperado, las reglas de negocio, las validaciones, las consecuencias y los errores relevantes alrededor de un comportamiento.

## Propósito

Un Documento de caso de uso ayuda al equipo a preservar:

- __domain meaning__: por qué este comportamiento importa dentro del dominio.
- __actor intention__: quién necesita el comportamiento y qué intenta lograr.
- __expected consequence__: qué debería cambiar cuando el comportamiento tiene éxito.
- __validations__: qué debe ser verdadero antes o durante el comportamiento.
- __business rules__: condiciones que moldean lo permitido o denegado.
- __expected errors__: casos de fallo conocidos que pertenecen al dominio.
- __related context__: scenario, process, workflow o capability que da significado al comportamiento.

El objetivo es hacer explícito el comportamiento esperado antes o durante la implementación.

## Cuándo usarlo

Usa un Documento de caso de uso cuando el comportamiento necesite suficiente claridad para guiar diseño, implementación o validación.

Es especialmente útil cuando:

- __the behavior has domain meaning__: la acción cambia algo importante en el negocio.
- __validations matter__: el sistema debe rechazar o permitir el comportamiento según reglas explícitas.
- __consequences matter__: el éxito cambia estado, responsabilidad, disponibilidad, compromiso o visibilidad.
- __errors are expected__: algunos fallos forman parte del dominio y deben modelarse explícitamente.
- __implementation needs guidance__: los desarrolladores necesitan más que un nombre de feature o una tarea corta.
- __validation needs clarity__: el equipo necesita saber qué demuestra que el comportamiento funciona.

## Cuándo no usarlo

Un Documento de caso de uso puede ser innecesario cuando:

- __the behavior is trivial__: el resultado esperado es obvio y de bajo riesgo.
- __the context is still unclear__: primero puede necesitarse un Documento de contexto o un Documento de proceso.
- __only a process needs explanation__: el equipo intenta describir cómo se realiza el trabajo.
- __only a technical task exists__: el trabajo todavía no tiene comportamiento de dominio significativo.
- __a support note is enough__: el comportamiento sigue siendo temprano, incierto o exploratorio.

## Versión mínima

Usa la versión mínima cuando el equipo necesite una definición ligera del comportamiento.

```md
# Documento de caso de uso

## Use case

¿Qué comportamiento se describe?

## Meaning

¿Qué significa este comportamiento en el dominio?

## Actor

¿Quién necesita o activa este comportamiento?

## Expected consequence

¿Qué cambia si esto tiene éxito?

## Validations

¿Qué debe ser verdadero?

## Expected errors

¿Qué puede fallar de una forma conocida y relevante para el dominio?

## Related artifacts

¿Qué scenario, process, workflow, capability o decision apoya este caso de uso?
```

## Versión ampliada

Usa la versión ampliada cuando el comportamiento sea complejo, riesgoso, pesado en reglas o crítico para la implementación.

```md
# Documento de caso de uso

## Use case

## Meaning

## Actor or trigger

## Related scenario

## Related process or workflow

## Preconditions

## Expected consequence

## Main behavior

## Alternative behavior

## Validations

## Business rules

## Expected errors

## Postconditions

## Inputs

## Outputs

## Related capabilities

## Related decisions

## Validation notes
```

## Artefactos relacionados

Un Documento de caso de uso puede apoyar o ser apoyado por:

- __Documento de contexto__: explica el scenario donde importa el comportamiento.
- __Documento de proceso__: explica el proceso o workflow donde aparece el comportamiento.
- __Vocabulario de dominio__: preserva términos necesarios para entender el comportamiento.
- __Documento de capacidad__: identifica capacidades estables requeridas por el caso de uso.
- __Registro de decisión__: explica elecciones tomadas por comportamiento, reglas o _tradeoffs_.
- __Nota de validación__: captura evidencia sobre si el comportamiento funcionó como se esperaba.
- __Nota de soporte__: captura reglas, ejemplos, errores o supuestos inciertos.

## Afinidad con estándares

Este documento puede apoyar la alineación con estándares y prácticas de documentación existentes. No vuelve la documentación conforme por sí mismo.

| Standard or practice | Affinity | Supports | Missing for stricter alignment |
| --- | --- | --- | --- |
| ISO/IEC/IEEE 29148 | High | Requirements-related language, behavior meaning, validations, expected errors, and traceability. | Formal requirement statements, requirement attributes, verification method, and requirements management process. |
| 4+1 View Model | High | Scenario and use-case-oriented thinking. | Complete 4+1 view model and connection to logical, process, development, and physical views. |
| ISO/IEC/IEEE 42010 | Medium | Concerns, behavior rationale, relationships, and decision impact. | Formal viewpoint, view, correspondence, and architecture description model. |
| arc42 | Medium | Runtime behavior, risks, decisions, and glossary connections. | Complete arc42 structure, especially runtime and building block integration. |
| ADR | Medium | Decisions related to behavior, rules, and _tradeoffs_. | Architecture-specific decision lifecycle and governance. |
| C4 Model | Low | Context and boundary awareness around the behavior. | Visual model hierarchy, container, component, and code views. |

## Errores comunes

Errores comunes incluyen:

- __describir solo pasos__: el documento omite consecuencia, validación y significado.
- __escribir tareas técnicas como casos de uso__: el comportamiento no tiene propósito de dominio visible.
- __ignorar errores esperados__: los fallos del dominio se convierten en excepciones ocultas o lógica ad hoc.
- __ocultar validaciones__: las reglas permanecen implícitas hasta la implementación.
- __olvidar la intención del actor__: el documento dice qué pasa, pero no por qué importa.
- __mezclar proceso con caso de uso__: el documento explica toda la forma de trabajar en lugar de un solo comportamiento significativo.
- __tratar el éxito como obvio__: la consecuencia esperada nunca se explicita.

## Preguntas de ejemplo

Un Documento de caso de uso debería ayudar a responder:

- ¿Qué comportamiento estamos describiendo?
- ¿Qué significa este comportamiento en el dominio?
- ¿Quién lo necesita, lo activa o se beneficia de él?
- ¿Qué debería cambiar cuando tiene éxito?
- ¿Qué debe ser válido antes o durante la ejecución?
- ¿Qué errores esperados pueden ocurrir?
- ¿Qué reglas de negocio moldean el comportamiento?
- ¿Qué capacidad, proceso o decisión depende de este caso de uso?

## Continuidad

Un Documento de caso de uso preserva continuidad entre el comportamiento del dominio y el comportamiento de la implementación.

```text
scenario or process
-> meaningful behavior
-> validations and consequences
-> capabilities and decisions
-> implementation and tests
-> validation and evolution
```

Cuando los casos de uso siguen siendo explícitos, es menos probable que el equipo implemente acciones que funcionen técnicamente pero no representen correctamente el dominio.
