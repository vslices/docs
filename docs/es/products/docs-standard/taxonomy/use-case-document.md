# Documento de caso de uso

> Puedes acceder a la [plantilla de documento de caso de uso aquí](https://github.com/vslices/docs-standard/blob/main/templates/use-case-document.md)

Un Documento de caso de uso (*Use Case Document* en inglés) preserva el significado de un comportamiento dentro de un contexto de dominio.

Su propósito es describir qué significa una interacción, operación o comportamiento esperado, qué consecuencia produce y qué debe ser válido para que ese comportamiento tenga sentido. Un Documento de caso de uso responde:

> ¿Qué significa este comportamiento?

Un caso de uso no es solo una secuencia de pasos. Explica el resultado esperado, reglas de negocio, validaciones, consecuencias y errores relevantes alrededor de un comportamiento.

## Propósito

Un Documento de caso de uso ayuda al equipo a preservar:

* **significado de dominio**: por qué este comportamiento importa dentro del dominio.
* **intención del actor**: quién necesita el comportamiento y qué intenta lograr.
* **consecuencia esperada**: qué debería cambiar después de que el comportamiento tenga éxito.
* **validaciones**: qué debe ser verdadero antes o durante el comportamiento.
* **reglas de negocio**: condiciones que moldean qué está permitido o denegado.
* **errores esperados**: casos de falla conocidos que pertenecen al dominio.
* **contexto relacionado**: escenario, proceso, flujo de trabajo o capacidad que da significado al comportamiento.

El objetivo es hacer explícito el comportamiento esperado antes o durante la implementación.

## Cuándo usarlo

Usa un Documento de caso de uso cuando un comportamiento necesite suficiente claridad para guiar diseño, implementación o validación.

Es especialmente útil cuando:

* **el comportamiento tiene significado de dominio**: la acción cambia algo importante en el negocio.
* **las validaciones importan**: el sistema debe rechazar o permitir comportamiento según reglas explícitas.
* **las consecuencias importan**: el éxito cambia estado, responsabilidad, disponibilidad, compromiso o visibilidad.
* **los errores son esperados**: algunas fallas son parte del dominio y deberían modelarse explícitamente.
* **la implementación necesita guía**: los desarrolladores necesitan más que un nombre de *feature* o una tarea corta.
* **la validación necesita claridad**: el equipo necesita saber qué demuestra que el comportamiento funciona.

## Cuándo no usarlo

Un Documento de caso de uso puede ser innecesario cuando:

* **el comportamiento es trivial**: el resultado esperado es obvio y de bajo riesgo.
* **el contexto todavía no está claro**: puede necesitarse primero un Documento de contexto o Documento de proceso.
* **solo necesita explicación un proceso**: el equipo intenta describir cómo se realiza el trabajo.
* **solo existe una tarea técnica**: el trabajo todavía no tiene comportamiento de dominio significativo.
* **basta con una Nota de soporte**: el comportamiento todavía es temprano, incierto o exploratorio.

## Versión mínima

Usa la versión mínima cuando el equipo necesite una definición ligera de comportamiento.

```md
# Use Case Document

## Use case

¿Qué comportamiento se está describiendo?

## Meaning

¿Qué significa este comportamiento en el dominio?

## Actor

¿Quién necesita o dispara este comportamiento?

## Expected consequence

¿Qué cambia si esto tiene éxito?

## Validations

¿Qué debe ser verdadero?

## Expected errors

¿Qué puede fallar de una forma conocida y relevante para el dominio?

## Related artifacts

¿Qué escenario, proceso, flujo de trabajo, capacidad o decisión apoya este caso de uso?
```

## Versión ampliada

Usa la versión ampliada cuando el comportamiento sea complejo, riesgoso, cargado de reglas o crítico para la implementación.

```md
# Use Case Document

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

## Afinidad con estándares

Este documento puede apoyar la alineación con estándares y prácticas de documentación existentes. No vuelve la documentación conforme por sí mismo.

| Estándar           | Afinidad | Soporta                                                                                                                                                          |
| ------------------ | -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ISO/IEC/IEEE 29148 | Alta     | <ul><li>Lenguaje relacionado con requisitos</li><li>Significado del comportamiento</li><li>Validaciones</li><li>Errores esperados</li><li>Trazabilidad</li></ul> |
| ISO/IEC/IEEE 42010 | Media    | <ul><li>Intereses</li><li>Justificación del comportamiento</li><li>Relaciones</li><li>Impacto de decisiones</li></ul>                                            |

| Práctica  | Afinidad | Soporta                                                                                                                    |
| --------- | -------- | -------------------------------------------------------------------------------------------------------------------------- |
| arc42     | Media    | <ul><li>Comportamiento en tiempo de ejecución</li><li>Riesgos</li><li>Decisiones</li><li>Conexiones con glosario</li></ul> |
| C4 Model  | Baja     | <ul><li>Conciencia de contexto</li><li>Conciencia de límites alrededor del comportamiento</li></ul>                        |
| 4+1 Model | Alta     | <ul><li>Escenarios</li><li>Razonamiento orientado a casos de uso</li></ul>                                                 |
| ADR       | Media    | <ul><li>Decisiones relacionadas con comportamiento</li><li>Reglas</li><li>*Tradeoffs*</li></ul>                            |

## Artefactos relacionados

Un Documento de caso de uso puede apoyar o ser apoyado por:

| Artefacto                                        | Relación                                                                   |
| ------------------------------------------------ | -------------------------------------------------------------------------- |
| [Documento de contexto](context-document.md)     | Explica el escenario donde importa el comportamiento.                      |
| [Documento de proceso](process-document.md)      | Explica el proceso o flujo de trabajo donde aparece el comportamiento.     |
| [Vocabulario de dominio](domain-vocabulary.md)   | Preserva términos necesarios para entender el comportamiento.              |
| [Documento de capacidad](capability-document.md) | Identifica capacidades estables requeridas por el caso de uso.             |
| [Registro de decisión](decision-record.md)       | Explica elecciones tomadas debido al comportamiento, reglas o *tradeoffs*. |
| [Nota de validación](validation-note.md)         | Captura evidencia sobre si el comportamiento funcionó como se esperaba.    |
| [Nota de soporte](support-note.md)               | Captura reglas, ejemplos, errores o supuestos inciertos.                   |

## Errores comunes

Errores comunes incluyen:

* **describir solo pasos**: el documento omite consecuencia, validación y significado.
* **escribir tareas técnicas como casos de uso**: el comportamiento no tiene propósito de dominio visible.
* **ignorar errores esperados**: las fallas de dominio se convierten en excepciones ocultas o lógica improvisada.
* **ocultar validaciones**: las reglas permanecen implícitas hasta la implementación.
* **olvidar la intención del actor**: el documento dice qué ocurre, pero no por qué importa.
* **mezclar proceso con caso de uso**: el documento explica toda la forma de trabajar en vez de un comportamiento significativo.
* **tratar el éxito como obvio**: la consecuencia esperada nunca se vuelve explícita.

## Preguntas de ejemplo

Un Documento de caso de uso debería ayudar a responder:

* ¿Qué comportamiento estamos describiendo?
* ¿Qué significa este comportamiento en el dominio?
* ¿Quién lo necesita, lo dispara o se beneficia de él?
* ¿Qué debería cambiar cuando tiene éxito?
* ¿Qué debe ser válido antes o durante la ejecución?
* ¿Qué errores esperados pueden ocurrir?
* ¿Qué reglas de negocio moldean el comportamiento?
* ¿Qué capacidad, proceso o decisión depende de este caso de uso?

## Continuidad

Un Documento de caso de uso preserva continuidad entre comportamiento de dominio y comportamiento de implementación.

```text
Escenario o proceso
-> Comportamiento significativo
-> Validaciones y consecuencias
-> Capacidades y decisiones
-> Implementación y pruebas
-> Validación y evolución
```

Cuando los casos de uso permanecen explícitos, es menos probable que el equipo implemente acciones que funcionan técnicamente pero no representan correctamente el dominio.
