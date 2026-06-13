# Documento de proceso

> Puedes acceder a la [plantilla de documento de proceso aquí](https://github.com/vslices/docs-standard/blob/main/templates/process-document.md)

Un Documento de proceso preserva cómo opera un work line.

Su propósito es hacer visibles las responsabilidades, roles, reglas de coordinación, workflows, _handoffs_ y resultados lo suficiente como para apoyar mejores decisiones de diseño e implementación.

Un Documento de proceso responde:

> ¿Cómo lo hacemos?
>
> ¿Qué se hace?

Un Documento de proceso no es un manual operativo completo. Describe el conocimiento de proceso que importa para entender, mejorar, automatizar o preservar cómo se realiza el trabajo.

## Propósito

Un Documento de proceso ayuda al equipo a preservar:

* **work process**: cómo se realiza un work line en la práctica.
* **responsibilities**: quién posee, ejecuta, aprueba, apoya o reacciona al trabajo.
* **roles and positions**: qué cargos, equipos, áreas o sistemas participan.
* **coordination rules**: cómo los participantes organizan el trabajo entre ellos.
* **workflows**: secuencias concretas de pasos, decisiones, _handoffs_ y participantes responsables.
* **exceptions**: rutas alternativas, fallos, retrabajo o casos poco comunes.
* **friction**: retrasos, ambigüedad, duplicación, trabajo manual o coordinación frágil.

El objetivo es entender cómo está organizado el trabajo antes de cambiarlo o automatizarlo.

## Cuándo usarlo

Usa un Documento de proceso cuando la forma en que se realiza el trabajo afecte el entendimiento, la planificación o la implementación.

Es especialmente útil cuando:

- __the work line needs operational clarity__: el equipo necesita entender cómo se produce actualmente el valor.
- __responsibilities are important__: los roles, la propiedad, las aprobaciones o las reacciones afectan el proceso.
- __coordination is fragile__: el trabajo depende de _handoffs_, tiempo, comunicación o acuerdos implícitos.
- __several workflows exist__: el proceso contiene múltiples rutas, variantes o casos operativos.
- __rules shape the process__: las condiciones de negocio afectan lo que puede ocurrir y quién debe actuar.
- __automation is being considered__: el software puede apoyar, reemplazar o modificar el trabajo existente.
- __current behavior is inconsistent__: distintas personas describen el proceso de manera diferente.

## Cuándo no usarlo

Un Documento de proceso puede ser innecesario cuando:

- __the process is trivial__: la forma en que se realiza el trabajo no afecta decisiones de diseño.
- __the scenario is still unclear__: primero puede necesitarse un Documento de contexto o una Nota de soporte.
- __only one interaction matters__: un Documento de caso de uso puede ser suficiente.
- __only a sequence of steps matters__: una pequeña nota de workflow puede ser suficiente.
- __the team is documenting every operational detail__: el documento se convierte en un manual de procedimiento exhaustivo.
- __the process is too unstable__: puede ser mejor una Nota de soporte hasta que el work process sea más claro.

## Versión mínima

Usa la versión mínima cuando el equipo necesite una descripción ligera de cómo se realiza el trabajo.

```md
# Documento de proceso

## Work process

¿Cómo se realiza este work line?

## Purpose

¿Por qué existe este proceso?

## Participants and responsibilities

¿Quién participa y de qué es responsable?

## Main workflow

- Step 1.
- Step 2.
- Step 3.

## Outcome

¿Qué produce este proceso?

## Pain points or risks

¿Qué hace que este proceso sea frágil, lento, poco claro o riesgoso?
```

## Afinidad con estándares

Este documento puede apoyar la alineación con estándares y prácticas de documentación existentes. No vuelve la documentación conforme por sí mismo.

| Standard or practice | Affinity | Supports | Missing for stricter alignment |
| --- | --- | --- | --- |
| arc42 | Medium / High | Runtime behavior, process movement, risks, responsibilities, and operational concerns. | Complete runtime view, building block view, and deployment integration. |
| ISO/IEC/IEEE 29148 | Medium | Process-related requirements, assumptions, business rules, and validation inputs. | Formal requirement statements, attributes, verification methods, and requirements management. |
| 4+1 View Model | Medium | Process-oriented view thinking and scenario support. | Complete process view and relationship with other architecture views. |
| ISO/IEC/IEEE 42010 | Medium | Concerns, relationships, and process constraints that may shape architecture. | Formal viewpoints, views, correspondence rules, and architecture description framework. |
| C4 Model | Low / Medium | Boundary and interaction awareness. | Visual model hierarchy and structural diagrams. |
| ADR | Low / Medium | Process constraints that may justify decisions. | Formal decision record lifecycle. |

## Versión ampliada

Usa la versión ampliada cuando el proceso sea complejo, riesgoso, transversal o probable de guiar la implementación.

```md
# Documento de proceso

## Work process

## Purpose

## Scope

## Related scenario or work line

## Participants, roles, and responsibilities

## Preconditions

## Coordination rules

## Main workflow

## Alternative workflows

## Exceptions and rework

## Business rules

## Handoffs

## Inputs

## Outputs

## Systems or tools involved

## Pain points

## Risks

## Related artifacts
```

## Artefactos relacionados

Un Documento de proceso puede apoyar o ser apoyado por:

- __Documento de contexto__: explica el scenario y el work line donde existe el proceso.
- __Vocabulario de dominio__: preserva términos usados dentro del proceso.
- __Documento de caso de uso__: describe el significado, las consecuencias y las validaciones de un comportamiento específico.
- __Documento de capacidad__: identifica capacidades estables necesarias para realizar o mejorar el proceso.
- __Registro de decisión__: explica elecciones tomadas por restricciones del proceso.
- __Nota de validación__: captura lo aprendido después de cambiar o probar el proceso.
- __Nota de soporte__: captura responsabilidades inciertas, variantes de workflow, riesgos, supuestos o preguntas abiertas.

## Errores comunes

Errores comunes incluyen:

- __confundir proceso con workflow__: el documento solo enumera pasos y omite responsabilidades o coordinación.
- __documentarlo todo__: el proceso se vuelve demasiado grande para guiar decisiones.
- __escribir solo el camino feliz__: las excepciones y el retrabajo permanecen invisibles.
- __ignorar _handoffs___: las partes más frágiles del proceso desaparecen.
- __mezclar comportamiento actual y objetivo__: los lectores no pueden distinguir qué existe hoy y qué se propone.
- __ocultar la propiedad__: las responsabilidades permanecen implícitas.
- __saltar a la automatización__: el equipo diseña software antes de entender el trabajo.
- __no actualizar después del cambio__: el proceso documentado ya no coincide con la realidad.

## Preguntas de ejemplo

Un Documento de proceso debería ayudar a responder:

- ¿Cómo se realiza este work line?
- ¿Por qué existe este proceso?
- ¿Quién participa y de qué es responsable?
- ¿Cómo coordinan el trabajo los participantes?
- ¿Qué workflows existen dentro de este proceso?
- ¿Qué ocurre primero, después y al final?
- ¿Dónde se mueve el trabajo entre personas, áreas, sistemas o herramientas?
- ¿Qué hace que el proceso sea lento, frágil, riesgoso o poco claro?
- ¿Qué casos de uso, capacidades o decisiones dependen de este proceso?

## Continuidad

Un Documento de proceso preserva continuidad entre la estructura operativa y el comportamiento del software.

```text
work line
-> work process
-> responsibilities and workflows
-> use cases and capabilities
-> decisions and implementation
-> validation and evolution
```

Cuando el comportamiento del proceso sigue siendo explícito, es menos probable que el equipo construya software que funcione técnicamente pero falle operacionalmente.
