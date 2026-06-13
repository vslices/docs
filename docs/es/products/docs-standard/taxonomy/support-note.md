# Nota de soporte

> Puedes acceder a la [plantilla de nota de soporte aquí](https://github.com/vslices/docs-standard/blob/main/templates/support-note.md)

Una Nota de soporte preserva conocimiento útil que todavía no está listo o no es lo bastante importante como para convertirse en un documento formal.

Su propósito es capturar conceptos, supuestos, riesgos, preguntas, feedback, detalles de implementación o ideas de mejora sin añadir estructura innecesaria. Una Nota de soporte responde:

> ¿Qué no deberíamos perder todavía?

Una nota de soporte es intencionalmente ligera. Más adelante puede fusionarse en un documento, enlazarse desde otro artefacto, ser reemplazada o archivada.

## Propósito

Una Nota de soporte ayuda al equipo a preservar:

- __early knowledge__: ideas, observaciones o hallazgos que todavía se están formando.
- __uncertainty__: supuestos, riesgos, preguntas abiertas y conceptos poco claros.
- __local detail__: información útil en un contexto específico pero no lo bastante amplia para un documento completo.
- __temporary learning__: feedback, notas de implementación o descubrimientos que quizá importen más adelante.
- __future candidates__: conocimiento que puede convertirse en parte de un Documento de contexto, Documento de proceso, Documento de caso de uso, Documento de capacidad, Registro de decisión o Nota de validación.

El objetivo es preservar conocimiento útil sin forzar una estructura prematura.

## Tipos comunes

Las Notas de soporte pueden incluir:

- __Concept Note__: captura un concepto temprano antes de que forme parte del Vocabulario de dominio u otro documento.
- __Assumption Note__: captura algo que el equipo cree verdadero pero todavía no ha validado.
- __Risk Note__: captura una posible fuente de falla, malentendido, retraso, retrabajo o complejidad accidental.
- __Open Question__: captura algo que el equipo todavía necesita entender.
- __Feature Note__: captura una idea temprana de feature antes de que su caso de uso, capacidad o alcance estén claros.
- __Feedback Note__: captura input de usuarios, expertos del dominio, stakeholders, implementación u operación.
- __Implementation Note__: captura detalle técnico útil que todavía no es un registro de decisión.
- __Scope Note__: captura lo que puede estar incluido, excluido, pospuesto o intencionalmente ignorado.
- __Improvement Note__: captura una posible mejora antes de que se convierta en un cambio planificado.

## Cuándo usarla

Usa una Nota de soporte cuando el conocimiento deba preservarse, pero un documento formal sería demasiado. Es especialmente útil cuando:

- __the idea is early__: el equipo todavía no sabe dónde pertenece.
- __the knowledge is uncertain__: el equipo necesita seguir un supuesto, riesgo o pregunta.
- __the detail is local__: la información importa, pero solo en un contexto estrecho.
- __the team needs speed__: escribir un documento completo ralentizaría el aprendizaje sin añadir valor.
- __the knowledge may evolve__: la nota puede convertirse más adelante en parte de un documento mayor.

## Cuándo no usarla

Una Nota de soporte puede ser insuficiente cuando:

- __the knowledge is stable and reused__: un documento formal puede ser mejor.
- __the note affects major decisions__: puede necesitarse un Registro de decisión.
- __the note describes expected behavior__: un Documento de caso de uso puede ser más claro.
- __the note describes a process__: un Documento de proceso puede ser mejor.
- __the note validates something important__: puede necesitarse una Nota de validación.
- __too many notes repeat the same topic__: probablemente el conocimiento deba consolidarse.

## Estructura sugerida

Usa la estructura más pequeña que preserve la nota.

```md
# Support Note

## Type

Concept, assumption, risk, question, feedback, implementation, scope, or improvement.

## Note

What should be preserved?

## Context

Where did this appear?

## Why it matters

Why could this matter later?

## Status

Open, active, resolved, superseded, or archived.

## Related artifacts

Which documents, decisions, or notes are connected?
```

## Afinidad con estándares

Este documento puede apoyar la alineación con estándares y prácticas de documentación existentes. No vuelve la documentación conforme por sí mismo.

| Standard or practice | Affinity | Supports | Missing for stricter alignment |
| --- | --- | --- | --- |
| ISO/IEC/IEEE 29148 | Medium | Assumptions, risks, open questions, feedback, and early requirement inputs. | Formal requirement statements, attributes, verification, and requirements management. |
| ISO/IEC/IEEE 42010 | Medium | Early concerns, stakeholder notes, rationale inputs, and relationships. | Formal viewpoints, views, correspondences, and architecture description framework. |
| arc42 | Medium | Risks, constraints, open questions, glossary candidates, and decision inputs. | Complete arc42 structure and formal section placement. |
| ADR | Medium | Early decision inputs, options, assumptions, and risks. | Formal decision record and governance lifecycle. |
| C4 Model | Low | Early notes about boundaries, systems, and responsibilities. | Diagram notation and model hierarchy. |
| 4+1 View Model | Low | Early scenario, behavior, or view-related notes. | Complete architecture view model. |

## Errores comunes

Errores comunes incluyen:

- __usar notas para siempre__: el conocimiento estable nunca se convierte en documentación formal.
- __crear demasiadas notas desconectadas__: el conocimiento útil se vuelve difícil de encontrar.
- __ocultar decisiones importantes__: se usa una nota cuando se necesita un Registro de decisión.
- __tratar supuestos como hechos__: la incertidumbre desaparece de la documentación.
- __no resolver preguntas__: las preguntas abiertas siguen abiertas después de que el equipo conoce la respuesta.
- __no consolidar notas repetidas__: el conocimiento relacionado permanece fragmentado.

## Preguntas de ejemplo

Una Nota de soporte debería ayudar a responder:

- ¿Qué conocimiento útil no deberíamos perder?
- ¿Es esto un concepto, supuesto, riesgo, pregunta, feedback, detalle de implementación, nota de alcance o idea de mejora?
- ¿Dónde apareció este conocimiento?
- ¿Por qué podría importar más adelante?
- ¿Sigue abierto, activo, resuelto, reemplazado o archivado?
- ¿Debería esta nota convertirse en parte de un documento formal?

## Continuidad

Una Nota de soporte preserva continuidad entre el descubrimiento temprano y la documentación estructurada.

```text
observation or idea
-> support note
-> related document or decision
-> validation or archive
-> future learning
```

Cuando las notas siguen siendo ligeras, el equipo puede preservar conocimiento emergente sin convertir cada observación en un documento formal.
