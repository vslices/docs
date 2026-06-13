# Documento de contexto

> Puedes acceder a la [plantilla de documento de contexto aquí](https://github.com/vslices/docs-standard/blob/main/templates/context-document.md)

Un Documento de contexto preserva el scenario donde está trabajando el equipo.

Su propósito es hacer visible el contexto de negocio, organizacional, operativo o del sistema lo suficiente como para apoyar mejores decisiones. Un Documento de contexto responde:

- ¿Dónde estamos trabajando?
- ¿Qué ofrece, opera o mantiene esta área?

Un Documento de contexto no es un mapa completo del negocio. Captura el contexto que importa para entender qué puede necesitar ser diseñado, mejorado, automatizado, integrado o preservado.

## Propósito

Un Documento de contexto ayuda al equipo a preservar:

- __scenario__: el contexto de negocio, organizacional, operativo o del sistema que se está observando.
- __work lines__: las áreas, departamentos, servicios, líneas de negocio u ofertas dentro del scenario.
- __actors and areas__: quién participa en el contexto.
- __current situation__: cómo se comporta el scenario hoy a alto nivel.
- __pain points and opportunities__: qué podría justificar trabajo futuro.
- __boundaries__: dónde comienza, termina o se vuelve poco claro el scenario.
- __uncertainty__: supuestos, riesgos y preguntas abiertas que todavía necesitan atención.

El objetivo es crear suficiente entendimiento compartido para evitar diseñar desde requisitos aislados.

## Cuándo usarlo

Usa un Documento de contexto cuando el scenario circundante afecte el entendimiento, la planificación o la implementación. Es especialmente útil cuando:

- __the scenario is unclear__: el equipo todavía no entiende dónde ocurre el trabajo.
- __several work lines exist__: el área incluye varios departamentos, servicios u ofertas.
- __many actors participate__: las responsabilidades, la propiedad o la colaboración pueden importar.
- __the current situation is fragmented__: el trabajo ocurre a través de pasos manuales, herramientas, documentos o sistemas heredados.
- __the change may affect adjacent work__: una mejora local podría impactar áreas o servicios cercanos.
- __the team needs a shared base__: documentos posteriores necesitan una referencia contextual estable.
- __the cost of misunderstanding is high__: construir desde un contexto débil podría crear complejidad accidental.

## Cuándo no usarlo

Un Documento de contexto puede ser innecesario cuando:

- __the change is small and isolated__: el contexto circundante no afecta la decisión.
- __the scenario is already understood__: la documentación existente o el conocimiento del equipo es suficiente.
- __only the process matters__: un Documento de proceso puede ser más útil.
- __only behavior matters__: un Documento de caso de uso puede ser suficiente.
- __the team needs fast feedback__: una pequeña _slice_ puede producir aprendizaje mejor y más seguro.
- __the document would become a full business map__: el equipo intenta documentarlo todo en lugar del contexto relevante.
- __a support note is enough__: el contexto sigue siendo temprano, pequeño o incierto.

## Versión mínima

Usa la versión mínima cuando el equipo necesite una base compartida ligera.

```md
# Documento de contexto

## Scenario

¿Dónde estamos trabajando?

## Why it matters

Por qué este scenario es relevante ahora.

## Scope

Qué está incluido y qué está intencionalmente fuera.

## Work lines

Qué áreas, departamentos, servicios u ofertas existen dentro de este scenario.

## Current situation

Cómo se comporta el scenario hoy a alto nivel.

## Actors and areas

¿Quién participa en este scenario?

## Pain points or opportunities

¿Qué podría justificar trabajo futuro?

## Open questions

¿Qué todavía necesita entenderse?
```

## Versión ampliada

Usa la versión ampliada cuando el scenario sea amplio, riesgoso, fragmentado o probable de guiar varios documentos futuros.

```md
# Documento de contexto

## Scenario

## Purpose

## Scope

## Out of scope

## Business background

## Work lines

## Actors, areas, and responsibilities

## Current situation

## Current systems or tools

## Pain points and opportunities

## Boundaries

## Relevant vocabulary

## Assumptions

## Risks

## Open questions

## Related artifacts
```

## Afinidad con estándares

Este documento puede apoyar la alineación con estándares y prácticas de documentación existentes. No vuelve la documentación conforme por sí mismo.

| Standard or practice | Affinity | Supports | Missing for stricter alignment |
| --- | --- | --- | --- |
| ISO/IEC/IEEE 42010 | High | Context, concerns, stakeholders, boundaries, relationships, and rationale inputs. | Formal architecture description, viewpoints, views, and correspondence model. |
| C4 Model | High | System context thinking, actors, systems, and boundary awareness. | Container, component, code views, and diagram notation. |
| arc42 | High | Context and scope, external interfaces, constraints, risks, and glossary connections. | Complete arc42 structure by default. |
| ISO/IEC/IEEE 29148 | Medium | Context for requirements, assumptions, risks, and traceability. | Formal requirements specification and management process. |
| 4+1 View Model | Medium | Scenario and context grounding for later views. | Complete architecture view model. |
| ADR | Low / Medium | Context for decisions and tradeoffs. | Decision-specific structure and governance. |

## Artefactos relacionados

Un Documento de contexto puede apoyar o ser apoyado por:

- __Vocabulario de dominio__: preserva términos importantes descubiertos dentro del scenario.
- __Documento de proceso__: describe cómo operan los work lines mediante responsabilidades y workflows.
- __Documento de caso de uso__: define el comportamiento esperado respaldado por el scenario.
- __Documento de capacidad__: identifica capacidades estables necesarias dentro del scenario o work line.
- __Registro de decisión__: explica decisiones tomadas por restricciones contextuales.
- __Nota de validación__: captura aprendizaje que cambia o confirma el scenario.
- __Nota de soporte__: captura hallazgos tempranos antes de que formen parte del contexto.

## Errores comunes

Errores comunes incluyen:

- __documentar todo el negocio__: el documento se vuelve demasiado amplio para guiar decisiones.
- __saltarse a soluciones__: el documento empieza a describir qué construir en lugar de dónde trabaja el equipo.
- __confundir scenario con proceso__: el documento sobreexplica cómo se realiza el trabajo.
- __confundir work line con workflow__: las áreas o servicios se describen como flujos paso a paso.
- __ignorar límites__: el equipo no puede decir dónde termina el scenario.
- __ocultar incertidumbre__: los supuestos y preguntas abiertas se escriben como hechos.
- __no actualizar después del aprendizaje__: el feedback de implementación cambia el scenario, pero el documento permanece congelado.

## Preguntas de ejemplo

Un Documento de contexto debería ayudar a responder:

- ¿Dónde estamos trabajando?
- ¿Por qué importa este scenario ahora?
- ¿Qué work lines existen dentro de este scenario?
- ¿Quién participa en este scenario?
- ¿Qué ocurre actualmente a alto nivel?
- ¿Qué pain points u oportunidades son visibles?
- ¿Qué límites son claros o poco claros?
- ¿Qué todavía no entendemos?
- ¿Qué documentos o decisiones dependen de este contexto?

## Continuidad

Un Documento de contexto preserva la continuidad entre la realidad de negocio descubierta y las decisiones de software posteriores.

```text
scenario
-> work lines
-> shared understanding
-> processes and use cases
-> capabilities and decisions
-> implementation scope
-> validation and evolution
```

Cuando el contexto sigue visible, los artefactos posteriores tienen menos probabilidades de quedar aislados del scenario que los justificó.
