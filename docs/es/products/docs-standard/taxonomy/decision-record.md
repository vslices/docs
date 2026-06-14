# Registro de decisión

> Puedes acceder a la [plantilla de registro de decisión aquí](https://github.com/vslices/docs-standard/blob/main/templates/decision-record.md)

Un Registro de decisión (*Decision Record* en inglés) preserva una decisión importante, el contexto que la moldeó y las consecuencias que el equipo aceptó.

Su propósito es explicar por qué se eligió una dirección para que el trabajo futuro pueda entender, revisar o cambiar esa decisión deliberadamente. Un Registro de decisión responde:

> ¿Por qué elegimos esto?

Una decisión puede tratar sobre lenguaje de dominio, diseño de procesos, alcance, arquitectura, implementación, validación o documentación.

## Propósito

Un Registro de decisión ayuda al equipo a preservar:

* **decisión**: la dirección seleccionada.
* **contexto**: la situación, restricción, riesgo o necesidad que hizo relevante la decisión.
* **opciones**: alternativas que el equipo consideró.
* **justificación**: por qué se eligió esta opción.
* ***tradeoffs***: qué ganó, perdió, aceptó o postergó el equipo.
* **consecuencias**: qué cambia debido a la decisión.
* **condiciones de revisión**: cuándo debería revisarse la decisión.

El objetivo es preservar razonamiento, no justificar decisiones después del hecho.

## Cuándo usarlo

Usa un Registro de decisión cuando una decisión afecte el entendimiento, la implementación o la evolución futura. Es especialmente útil cuando:

* **la decisión es difícil de revertir**: cambiarla más adelante puede ser costoso.
* **la decisión afecta varios artefactos**: contextos, procesos, casos de uso, capacidades o implementación pueden depender de ella.
* **los *tradeoffs* importan**: el equipo aceptó costos, riesgos o restricciones.
* **las alternativas eran plausibles**: lectores futuros pueden preguntarse por qué no se eligió otra opción.
* **la decisión moldea límites**: la propiedad, responsabilidad, arquitectura o alcance pueden cambiar.
* **la decisión puede ser cuestionada después**: preservar contexto evita repetir la misma discusión.

## Cuándo no usarlo

Un Registro de decisión puede ser innecesario cuando:

* **la decisión es trivial**: la elección no tiene impacto futuro significativo.
* **la decisión es completamente reversible**: cambiarla más adelante es barato y evidente.
* **el equipo solo está registrando tareas**: el trabajo de implementación no siempre necesita un registro de decisión.
* **la decisión todavía no está clara**: una Nota de soporte puede ser mejor hasta que las opciones se entiendan.
* **el registro se usa como teatro de aprobación**: el documento existe para parecer formal, no para preservar razonamiento.

## Versión mínima

Usa la versión mínima cuando el equipo solo necesite preservar el razonamiento central.

```md
# Decision Record

## Decision

¿Qué elegimos?

## Context

¿Por qué se necesitaba esta decisión?

## Rationale

¿Por qué elegimos esta dirección?

## Consequences

¿Qué cambia debido a esta decisión?

## Status

Borrador, activo, superado o archivado.
```

## Versión ampliada

Usa la versión ampliada cuando la decisión sea riesgosa, disputada, arquitectónica o probable de afectar la evolución futura.

```md
# Decision Record

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

| Estándar | Afinidad     | Soporta                                                                                                                                                                          |
| ------------------- | ------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ISO/IEC/IEEE 42010  | Media / Alta | <ul><li>Justificación de arquitectura</li><li>Intereses</li><li>Decisiones</li><li>Relaciones</li><li>Consecuencias</li></ul>                                                    |
| ISO/IEC/IEEE 29148  | Media        | <ul><li>Decisiones relacionadas con requisitos</li><li>Supuestos</li><li>Impacto de validación</li><li>Trazabilidad</li></ul>                                                    |

| Práctica | Afinidad     | Soporta                                                                                                                                                                          |
| ------------------- | ------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| arc42               | Alta         | <ul><li>Decisiones de arquitectura</li><li>Riesgos</li><li>Restricciones</li><li>Justificación</li></ul>                                                                         |
| 4+1 Model      | Media        | <ul><li>Decisiones que afectan escenarios</li><li>Estructura lógica</li><li>Procesos</li><li>Desarrollo</li><li>Vistas físicas</li></ul>                                         |
| C4 Model            | Media        | Decisiones: <ul><li>Que pueden afectar diagramas de contexto</li><li>Sobre contenedores</li><li>Sobre componentes</li><li>Sobre código</li></ul> |
| ADR                 | Alta         | <ul><li>Decisión</li><li>Justificación</li><li>Opciones</li><li>*Tradeoffs*</li><li>Consecuencias</li><li>Condiciones de revisión</li></ul>                                      |## Artefactos relacionados

Un Registro de decisión puede apoyar o ser apoyado por:

| Artefacto                                        | Relación                                                                           |
| ------------------------------------------------ | ---------------------------------------------------------------------------------- |
| [Documento de contexto](context-document.md)     | Explica el escenario o restricción detrás de la decisión.                          |
| [Documento de proceso](process-document.md)      | Muestra condiciones de proceso que influyeron en la decisión.                      |
| [Documento de caso de uso](use-case-document.md) | Describe comportamiento afectado por la decisión.                                  |
| [Documento de capacidad](capability-document.md) | Explica capacidades moldeadas por la decisión.                                     |
| [Vocabulario de dominio](domain-vocabulary.md)   | Preserva decisiones de lenguaje o elecciones de nombres.                           |
| [Nota de validación](validation-note.md)         | Confirma, desafía o actualiza la decisión.                                         |
| [Nota de soporte](support-note.md)               | Captura opciones tempranas, riesgos o supuestos antes de que se<br/>tome una decisión. |

## Errores comunes

Errores comunes incluyen:

* **registrar todo**: el equipo crea registros de decisión para elecciones sin impacto real.
* **escribir solo la respuesta final**: lectores futuros no pueden entender por qué se tomó la decisión.
* **ocultar *tradeoffs***: el registro finge que la opción elegida no tuvo costo.
* **ignorar opciones rechazadas**: las mismas alternativas se debaten nuevamente después.
* **usar decisiones como autoridad**: el registro se vuelve una forma de detener la discusión en lugar de preservar razonamiento.
* **no revisar decisiones antiguas**: el contexto cambió e invalida la decisión, pero el registro permanece activo.

## Preguntas de ejemplo

Un Registro de decisión debería ayudar a responder:

* ¿Qué decidimos?
* ¿Por qué se necesitaba esta decisión?
* ¿Qué alternativas se consideraron?
* ¿Por qué se eligió esta opción?
* ¿Qué *tradeoffs* aceptamos?
* ¿Qué riesgos mantuvimos conscientemente?
* ¿Qué artefactos o elecciones de implementación dependen de esta decisión?
* ¿Cuándo debería revisarse esta decisión?

## Continuidad

Un Registro de decisión preserva continuidad entre razonamiento y cambio futuro.

```text
Contexto o problema
-> Opciones y tradeoffs
-> Decisión seleccionada
-> Artefactos afectados
-> Consecuencias de implementación
-> Validación y evolución
```

Cuando las decisiones permanecen explícitas, el equipo puede evolucionar el sistema sin perder el razonamiento que le dio forma.
