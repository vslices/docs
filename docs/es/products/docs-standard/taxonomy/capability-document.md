# Documento de capacidad

> Puedes acceder a la [plantilla de documento de capacidad aquí](https://github.com/vslices/docs-standard/blob/main/templates/capability-document.md)

Un Documento de capacidad preserva una capacidad estable requerida por el negocio o el sistema.

Su propósito es describir qué debe ser posible sin decidir demasiado pronto cómo debe implementarse. Un Documento de capacidad responde:

> ¿Qué debe poder hacer este negocio o sistema?

Una capacidad no es una feature, endpoint, screen, service o componente técnico. Es una habilidad que puede apoyar varios casos de uso, workflows, procesos o decisiones.

## Propósito

Un Documento de capacidad ayuda al equipo a preservar:

- __stable ability__: qué debe poder hacer el negocio o sistema.
- __business value__: por qué importa esta capacidad.
- __supported behavior__: qué casos de uso o workflows dependen de la capacidad.
- __boundaries__: qué incluye y qué excluye la capacidad.
- __rules and constraints__: qué da forma o limita la capacidad.
- __expected outcomes__: qué permite esta capacidad.
- __implementation independence__: la capacidad puede entenderse antes de elegir una estructura de código.

El objetivo es identificar capacidades significativas sin convertirlas demasiado pronto en componentes técnicos.

## Cuándo usarlo

Usa un Documento de capacidad cuando una habilidad sea lo suficientemente estable como para guiar diseño o implementación. Es especialmente útil cuando:

- __several use cases need the same ability__: la capacidad aparece repetidamente en el comportamiento.
- __a process depends on a stable ability__: el proceso no puede funcionar sin esta capacidad.
- __the ability may define a boundary__: la propiedad, la responsabilidad o la arquitectura pueden surgir alrededor de ella.
- __business value needs to stay visible__: el equipo debe recordar por qué importa la capacidad.
- __implementation options are still open__: el equipo necesita claridad antes de elegir un diseño.
- __future evolution is expected__: la capacidad puede crecer, dividirse o volverse más formal después.

## Cuándo no usarlo

Un Documento de capacidad puede ser innecesario cuando:

- __the behavior is isolated__: un Documento de caso de uso es suficiente.
- __the ability is too vague__: el equipo todavía no puede explicar qué debe ser posible.
- __the team is naming technical components__: el documento se está usando para justificar arquitectura demasiado pronto.
- __the capability is only a feature name__: no hay una capacidad estable detrás.
- __the domain is still unclear__: primero puede necesitarse un Documento de contexto, un Documento de proceso o una Nota de soporte.

## Versión mínima

Usa la versión mínima cuando el equipo necesite una definición ligera de la capacidad.

```md
# Documento de capacidad

## Capability

¿Qué debe poder hacer el negocio o sistema?

## Why it matters

¿Qué valor proporciona esta capacidad?

## Supported behavior

¿Qué casos de uso, workflows o procesos dependen de ella?

## Boundaries

¿Qué está incluido y qué está fuera?

## Rules or constraints

¿Qué da forma o limita esta capacidad?

## Related artifacts

¿Qué contexto, proceso, caso de uso, decisión o validación apoya esta capacidad?
```

## Versión ampliada

Usa la versión ampliada cuando la capacidad sea importante, reutilizada, riesgosa o probable de influir en la arquitectura.

```md
# Documento de capacidad

## Capability

## Purpose

## Business value

## Related scenario or work line

## Supported processes

## Supported workflows

## Supported use cases

## Boundaries

## Responsibilities

## Inputs

## Outputs

## Rules and constraints

## Expected outcomes

## Expected errors

## Dependencies

## Related decisions

## Validation notes

## Evolution notes
```

## Afinidad con estándares

Este documento puede apoyar la alineación con estándares y prácticas de documentación existentes. No vuelve la documentación conforme por sí mismo.

| Standard or practice | Affinity | Supports | Missing for stricter alignment |
| --- | --- | --- | --- |
| ISO/IEC/IEEE 42010 | Medium / High | Architecture concerns, boundaries, rationale, and relationships between capabilities and decisions. | Formal viewpoint, view, model kind, and architecture description framework. |
| arc42 | Medium / High | Building block thinking, responsibilities, boundaries, risks, and decisions. | Complete building block view, runtime view, deployment view, and quality requirements structure. |
| ISO/IEC/IEEE 29148 | Medium | Capability-related requirements, constraints, expected outcomes, and traceability. | Formal requirement statements, requirement attributes, and verification methods. |
| C4 Model | Medium | Boundary awareness that may later influence container or component views. | Visual model hierarchy and diagram notation. |
| 4+1 View Model | Medium | Logical and process-oriented architecture thinking. | Complete logical, process, development, and physical views. |
| ADR | Medium | Decisions about capability shape, split, ownership, or implementation direction. | Formal ADR lifecycle and governance process. |

## Artefactos relacionados

Un Documento de capacidad puede apoyar o ser apoyado por:

- __Documento de contexto__: explica el scenario o work line donde importa la capacidad.
- __Documento de proceso__: muestra qué procesos requieren la capacidad.
- __Documento de caso de uso__: describe comportamientos habilitados por la capacidad.
- __Vocabulario de dominio__: preserva el lenguaje usado para nombrar y explicar la capacidad.
- __Registro de decisión__: explica por qué la capacidad fue moldeada, dividida, fusionada o implementada de una forma específica.
- __Nota de validación__: captura evidencia de si la capacidad apoya necesidades reales.
- __Nota de soporte__: captura ideas tempranas de capacidad antes de que se vuelvan capacidades estables.

## Errores comunes

Errores comunes incluyen:

- __confundir capacidad con feature__: una feature entrega un comportamiento concreto, mientras que una capacidad describe una habilidad estable.
- __confundir capacidad con componente__: el documento se convierte en arquitectura antes de que la necesidad del dominio sea clara.
- __nombrar demasiado pronto__: el equipo asigna nombres formales a habilidades que todavía son vagas.
- __hacerla demasiado amplia__: la capacidad se convierte en un contenedor para comportamiento no relacionado.
- __hacerla demasiado estrecha__: la capacidad solo repite un caso de uso.
- __ignorar límites__: los lectores no pueden distinguir qué incluye o excluye la capacidad.
- __olvidar el valor__: la capacidad existe, pero nadie recuerda por qué importa.

## Preguntas de ejemplo

Un Documento de capacidad debería ayudar a responder:

- ¿Qué debe poder hacer el negocio o el sistema?
- ¿Por qué importa esta capacidad?
- ¿Qué casos de uso, workflows o procesos dependen de ella?
- ¿Qué incluye esta capacidad?
- ¿Qué queda fuera de esta capacidad?
- ¿Qué reglas, restricciones o resultados la moldean?
- ¿Podría esta capacidad convertirse en un límite?
- ¿Qué decisiones o validaciones dependen de esta capacidad?

## Continuidad

Un Documento de capacidad preserva continuidad entre las necesidades del dominio y la posible estructura de implementación.

```text
scenario or work line
-> work process and use cases
-> stable ability
-> decisions and implementation options
-> validation and evolution
```

Cuando las capacidades permanecen independientes de la implementación demasiado pronto, el equipo puede razonar sobre qué debe proporcionar el sistema antes de decidir cómo debe estructurarse.
