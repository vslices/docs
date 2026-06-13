# Nota de validación

> Puedes acceder a la [plantilla de nota de validación aquí](https://github.com/vslices/docs-standard/blob/main/templates/validation-note.md)

Una Nota de validación preserva la evidencia reunida después de probar, construir, revisar, observar o usar algo.

Su propósito es capturar qué se confirmó, rechazó, cambió o aprendió para que el trabajo futuro pueda empezar con un mejor entendimiento. Una Nota de validación responde:

> ¿Qué aprendimos?

La validación no es solo pruebas. Puede venir de _feedback_ de implementación, _feedback_ de usuarios, revisión de expertos del dominio, comportamiento en producción, experimentos, prototipos u observación operativa.

## Propósito

Una Nota de validación ayuda al equipo a preservar:

- __validation target__: qué se estaba validando.
- __evidence__: qué se observó, probó, revisó o midió.
- __result__: qué se confirmó, rechazó o cambió.
- __learning__: qué entiende mejor ahora el equipo.
- __impact__: qué documentos, decisiones, comportamientos o implementaciones deberían cambiar.
- __remaining uncertainty__: qué todavía necesita más evidencia.
- __next action__: qué debería pasar después de la validación.

El objetivo es evitar que el aprendizaje desaparezca después de la implementación o la revisión.

## Cuándo usarla

Usa una Nota de validación cuando la evidencia cambie o confirme conocimiento del que dependerá el trabajo futuro. Es especialmente útil cuando:

- __an assumption was tested__: el equipo necesita registrar si sobrevivió.
- __a behavior was validated__: un caso de uso, _feature_ o _workflow_ se comprobó contra la realidad.
- __implementation revealed constraints__: construir expuso límites técnicos, operativos o del dominio.
- __feedback changed understanding__: usuarios, stakeholders o expertos del dominio aclararon algo importante.
- __a decision needs review__: la evidencia confirma, cuestiona o invalida una decisión previa.
- __production behavior teaches something__: el uso real revela patrones, problemas u oportunidades.

## Cuándo no usarla

Una Nota de validación puede ser innecesaria cuando:

- __nothing meaningful changed__: el resultado no afecta el entendimiento o las decisiones futuras.
- __the evidence is too weak__: una Nota de soporte puede ser mejor hasta que exista más evidencia.
- __the result is only task completion__: terminar el trabajo no es lo mismo que aprender de él.
- __the validation belongs elsewhere__: casos de prueba detallados, métricas o incidentes pueden necesitar su propio formato.
- __the note would repeat existing documentation__: actualiza el documento relacionado en su lugar.

## Versión mínima

Usa la versión mínima cuando el equipo necesite preservar un resultado de aprendizaje pequeño pero útil.

```md
# Nota de validación

## Validation target

¿Qué se estaba validando?

## Evidence

¿Qué se observó, probó, revisó o midió?

## Result

¿Qué se confirmó, rechazó o cambió?

## Learning

¿Qué entendemos mejor ahora?

## Impact

¿Qué documentos, decisiones, comportamientos o implementaciones se ven afectados?

## Next action

¿Qué debería pasar después?
```

## Versión ampliada

Usa la versión ampliada cuando la validación afecte decisiones importantes, supuestos riesgosos o evolución futura.

```md
# Nota de validación

## Validation target

## Related assumption, decision, use case, or capability

## Validation method

## Evidence

## Result

## Learning

## Impact on documentation

## Impact on implementation

## Impact on decisions

## Remaining uncertainty

## Risks discovered

## Next action

## Related artifacts
```

## Afinidad con estándares

Este documento puede apoyar la alineación con estándares y prácticas de documentación existentes. No vuelve la documentación conforme por sí mismo.

| Standard or practice | Affinity | Supports | Missing for stricter alignment |
| --- | --- | --- | --- |
| ISO/IEC/IEEE 29148 | High | Validation, evidence, assumptions, feedback, impact, and traceability. | Formal verification plan, requirement verification method, audit-grade evidence controls, and requirements management workflow. |
| ADR | Medium | Reviewing whether previous decisions were confirmed, challenged, or superseded. | Formal architecture decision lifecycle and governance process. |
| ISO/IEC/IEEE 42010 | Medium | Rationale updates, architecture learning, and relationships between evidence and decisions. | Formal architecture description, viewpoints, views, and correspondence rules. |
| arc42 | Medium | Risks, decisions, quality feedback, and evolution notes. | Complete arc42 structure and formal quality scenario integration. |
| 4+1 View Model | Low / Medium | Scenario feedback and behavior validation. | Complete architecture view model and view-specific validation structure. |
| C4 Model | Low | Feedback that may affect boundaries or architecture diagrams. | Diagram notation and visual hierarchy. |

## Artefactos relacionados

Una Nota de validación puede apoyar o ser apoyada por:

- __Documento de contexto__: actualiza el scenario después de que aparece nueva evidencia.
- __Documento de proceso__: confirma o cuestiona cómo se realiza realmente el trabajo.
- __Documento de caso de uso__: valida comportamiento esperado, consecuencia, errores o reglas.
- __Documento de capacidad__: confirma si una capacidad apoya necesidades reales.
- __Registro de decisión__: valida, cuestiona o reemplaza una decisión.
- __Vocabulario de dominio__: actualiza términos cuando la evidencia aclara el lenguaje.
- __Nota de soporte__: captura _feedback_ temprano antes de que se convierta en aprendizaje validado.

## Errores comunes

Errores comunes incluyen:

- __tratar la entrega como validación__: que algo funcione técnicamente no prueba que resolvió el problema correcto.
- __registrar conclusiones sin evidencia__: los lectores futuros no pueden entender por qué el resultado es confiable.
- __ignorar resultados negativos__: los supuestos fallidos son aprendizaje valioso.
- __no actualizar artefactos relacionados__: la nota captura aprendizaje, pero la documentación y la implementación permanecen igual.
- __ocultar la incertidumbre__: el equipo trata la evidencia parcial como verdad final.
- __sobredocumentar pruebas rutinarias__: no todos los resultados de pruebas necesitan una nota de validación.

## Preguntas de ejemplo

Una Nota de validación debería ayudar a responder:

- ¿Qué se validó?
- ¿Qué evidencia se reunió?
- ¿Qué se confirmó, rechazó o cambió?
- ¿Qué aprendimos?
- ¿Qué supuesto, decisión, comportamiento o capacidad se ve afectado?
- ¿Qué sigue incierto?
- ¿Qué debería cambiar después?
- ¿La siguiente iteración debe continuar, ajustarse o cambiar de dirección?

## Continuidad

Una Nota de validación preserva continuidad entre la entrega y el entendimiento renovado.

```text
implementation or review
-> evidence
-> learning
-> updated documents and decisions
-> next implementation
-> evolution
```

Cuando la validación sigue siendo explícita, el equipo es menos propenso a repetir supuestos incorrectos o a ignorar lo que el sistema le enseñó después de ser construido.
