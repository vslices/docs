# Registro de decisión

> Puedes acceder a la [plantilla de registro de decisión aquí](https://github.com/vslices/docs-standard/blob/main/templates/decision-record.md)

Un Registro de decisión preserva una decisión importante, el contexto que la moldeó y las consecuencias que el equipo aceptó.

Su propósito es explicar por qué se eligió una dirección para que el trabajo futuro pueda entender, revisar o cambiar esa decisión deliberadamente. Un Registro de decisión responde:

> ¿Por qué elegimos esto?

Una decisión puede tratar sobre lenguaje de dominio, diseño de procesos, alcance, arquitectura, implementación, validación o documentación.

## Propósito

Un Registro de decisión ayuda al equipo a preservar:

- __decision__: la dirección seleccionada.
- __context__: la situación, restricción, riesgo o necesidad que hizo relevante la decisión.
- __options__: alternativas que el equipo consideró.
- __rationale__: por qué se eligió esta opción.
- __tradeoffs__: qué ganó, perdió, aceptó o pospuso el equipo.
- __consequences__: qué cambia por la decisión.
- __review conditions__: cuándo debería revisarse la decisión.

El objetivo es preservar razonamiento, no justificar decisiones después del hecho.

## Cuándo usarlo

Usa un Registro de decisión cuando una decisión afecte el entendimiento futuro, la implementación o la evolución. Es especialmente útil cuando:

- __the decision is hard to reverse__: cambiarla después puede ser costoso.
- __the decision affects several artifacts__: contextos, procesos, casos de uso, capacidades o implementación pueden depender de ella.
- __tradeoffs matter__: el equipo aceptó costos, riesgos o restricciones.
- __alternatives were plausible__: los lectores futuros pueden preguntarse por qué no se eligió otra opción.
- __the decision shapes boundaries__: la propiedad, la responsabilidad, la arquitectura o el alcance pueden cambiar.
- __the decision may be challenged later__: preservar el contexto evita repetir la misma discusión.

## Cuándo no usarlo

Un Registro de decisión puede ser innecesario cuando:

- __the decision is trivial__: la elección no tiene impacto futuro significativo.
- __the decision is fully reversible__: cambiarla después es barato y obvio.
- __the team is only recording tasks__: el trabajo de implementación no siempre necesita un registro de decisión.
- __the decision is still unclear__: una Nota de soporte puede ser mejor hasta que se entiendan las opciones.
- __the record is used as approval theater__: el documento existe para parecer formal, no para preservar razonamiento.

## Versión mínima

Usa la versión mínima cuando el equipo solo necesite preservar el razonamiento central.

```md
# Registro de decisión

## Decision

¿Qué elegimos?

## Context

¿Por qué era necesaria esta decisión?

## Rationale

¿Por qué elegimos esta dirección?

## Consequences

¿Qué cambia por esta decisión?

## Status

Draft, active, superseded o archived.
```

## Versión ampliada

Usa la versión ampliada cuando la decisión sea riesgosa, discutida, arquitectónica o probable de afectar la evolución futura.

```md
# Registro de decisión

## Decision

## Status

## Context

## Problem or tension

## Options considered

## Selected option

## Rationale

## Tradeoffs

## Consequences

## Accepted risks

## Rejected alternatives

## Related artifacts

## Review conditions
```

## Afinidad con estándares

Este documento puede apoyar la alineación con estándares y prácticas de documentación existentes. No vuelve la documentación conforme por sí mismo.

| Standard or practice | Affinity | Supports | Missing for stricter alignment |
| --- | --- | --- | --- |
| ADR | High | Decision, rationale, options, tradeoffs, consequences, and review conditions. | A strict ADR template, numbering scheme, and governance workflow. |
| arc42 | High | Architecture decisions, risks, constraints, and rationale. | Complete arc42 architecture documentation structure. |
| ISO/IEC/IEEE 42010 | Medium / High | Architecture rationale, concerns, decisions, relationships, and consequences. | Formal architecture decision model inside a conforming architecture description. |
| ISO/IEC/IEEE 29148 | Medium | Requirements-related decisions, assumptions, validation impact, and traceability. | Formal requirements management and verification structure. |
| 4+1 View Model | Medium | Decisions affecting scenarios, logical structure, process, development, or physical views. | Complete 4+1 view model. |
| C4 Model | Medium | Decisions that may affect context, container, component, or code diagrams. | Diagram notation and visual model hierarchy. |

## Artefactos relacionados

Un Registro de decisión puede apoyar o ser apoyado por:

- __Documento de contexto__: explica el scenario o restricción detrás de la decisión.
- __Documento de proceso__: muestra las condiciones de proceso que influyeron en la decisión.
- __Documento de caso de uso__: describe el comportamiento afectado por la decisión.
- __Documento de capacidad__: explica las capacidades moldeadas por la decisión.
- __Vocabulario de dominio__: preserva decisiones de lenguaje o nombrado.
- __Nota de validación__: confirma, cuestiona o actualiza la decisión.
- __Nota de soporte__: captura opciones tempranas, riesgos o supuestos antes de tomar una decisión.

## Errores comunes

Errores comunes incluyen:

- __registrarlo todo__: el equipo crea registros de decisión para elecciones sin impacto real.
- __escribir solo la respuesta final__: los lectores futuros no pueden entender por qué se tomó la decisión.
- __ocultar _tradeoffs___: el registro finge que la opción elegida no tuvo costo.
- __ignorar opciones rechazadas__: luego se vuelven a debatir las mismas alternativas.
- __usar decisiones como autoridad__: el registro se convierte en una forma de detener la discusión en lugar de preservar el razonamiento.
- __no revisar decisiones antiguas__: el contexto cambió e invalidó la decisión, pero el registro permanece activo.

## Preguntas de ejemplo

Un Registro de decisión debería ayudar a responder:

- ¿Qué decidimos?
- ¿Por qué era necesaria esta decisión?
- ¿Qué alternativas se consideraron?
- ¿Por qué se eligió esta opción?
- ¿Qué _tradeoffs_ aceptamos?
- ¿Qué riesgos aceptamos conscientemente?
- ¿Qué artefactos o elecciones de implementación dependen de esta decisión?
- ¿Cuándo debería revisarse esta decisión?

## Continuidad

Un Registro de decisión preserva continuidad entre el razonamiento y el cambio futuro.

```text
context or problem
-> options and tradeoffs
-> selected decision
-> affected artifacts
-> implementation consequences
-> validation and evolution
```

Cuando las decisiones siguen siendo explícitas, el equipo puede evolucionar el sistema sin perder el razonamiento que lo moldeó.
