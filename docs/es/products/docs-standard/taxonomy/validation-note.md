# Nota de validación

> Puedes acceder a la [plantilla de nota de validación aquí](https://github.com/vslices/docs-standard/blob/main/templates/validation-note.md)

Una Nota de validación (*Validation Note* en inglés) preserva evidencia reunida después de probar, construir, revisar, observar o usar algo.

Su propósito es capturar qué fue confirmado, rechazado, cambiado o aprendido para que el trabajo futuro pueda empezar desde un mejor entendimiento. Una Nota de validación responde:

> ¿Qué aprendimos?

La validación no es solo pruebas. Puede venir de retroalimentación de implementación, retroalimentación de usuarios, revisión de expertos de dominio, comportamiento en producción, experimentos, prototipos u observación operacional.

## Propósito

Una Nota de validación ayuda al equipo a preservar:

* **objetivo de validación**: qué se estaba validando.
* **evidencia**: qué fue observado, probado, revisado o medido.
* **resultado**: qué fue confirmado, rechazado o cambiado.
* **aprendizaje**: qué entiende mejor el equipo ahora.
* **impacto**: qué documentos, decisiones, comportamientos o implementaciones deberían cambiar.
* **incertidumbre restante**: qué todavía necesita más evidencia.
* **siguiente acción**: qué debería ocurrir después de la validación.

El objetivo es evitar que el aprendizaje desaparezca después de la implementación o revisión.

## Cuándo usarla

Usa una Nota de validación cuando la evidencia cambie o confirme conocimiento del que depende trabajo futuro. Es especialmente útil cuando:

* **se probó un supuesto**: el equipo necesita registrar si sobrevivió.
* **se validó un comportamiento**: un caso de uso, *feature* o flujo de trabajo fue contrastado con la realidad.
* **la implementación reveló restricciones**: construir expuso límites técnicos, operacionales o de dominio.
* **la retroalimentación cambió el entendimiento**: usuarios, partes interesadas o expertos de dominio aclararon algo importante.
* **una decisión necesita revisión**: la evidencia confirma, desafía o invalida una decisión previa.
* **el comportamiento en producción enseña algo**: el uso real revela patrones, problemas u oportunidades.

## Cuándo no usarla

Una Nota de validación puede ser innecesaria cuando:

* **nada significativo cambió**: el resultado no afecta entendimiento o decisiones futuras.
* **la evidencia es demasiado débil**: una Nota de soporte puede ser mejor hasta que exista más evidencia.
* **el resultado solo es completar una tarea**: terminar trabajo no es lo mismo que aprender de él.
* **la validación pertenece a otro lugar**: casos de prueba detallados, métricas o incidentes pueden necesitar su propio formato.
* **la nota repetiría documentación existente**: actualiza el documento relacionado en su lugar.

## Versión mínima

Usa la versión mínima cuando el equipo necesite preservar un resultado de aprendizaje pequeño pero útil.

```md
# Validation Note

## Validation target

¿Qué se estaba validando?

## Evidence

¿Qué fue observado, probado, revisado o medido?

## Result

¿Qué fue confirmado, rechazado o cambiado?

## Learning

¿Qué entendemos mejor ahora?

## Impact

¿Qué documentos, decisiones, comportamientos o implementaciones están afectados?

## Next action

¿Qué debería ocurrir después?
```

## Versión ampliada

Usa la versión ampliada cuando la validación afecte decisiones importantes, supuestos riesgosos o evolución futura.

```md
# Validation Note

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

| Estándar           | Afinidad | Soporta                                                                                                                                |
| ------------------ | -------- | -------------------------------------------------------------------------------------------------------------------------------------- |
| ISO/IEC/IEEE 29148 | Alta     | <ul><li>Validación</li><li>Evidencia</li><li>Supuestos</li><li>Retroalimentación</li><li>Impacto</li><li>Trazabilidad</li></ul>        |
| ISO/IEC/IEEE 42010 | Media    | <ul><li>Actualizaciones de justificación</li><li>Aprendizaje de arquitectura</li><li>Relaciones entre evidencia y decisiones</li></ul> |

| Práctica  | Afinidad     | Soporta                                                                                                                                        |
| --------- | ------------ | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| arc42     | Media        | <ul><li>Riesgos</li><li>Decisiones</li><li>Retroalimentación de calidad</li><li>Notas de evolución</li></ul>                                   |
| C4 Model  | Baja         | Retroalimentación que:<ul><li>Puede afectar límites</li><li>Puede afectar diagramas de arquitectura</li></ul>            |
| 4+1 Model | Baja / Media | <ul><li>Retroalimentación de escenarios</li><li>Validación de comportamiento</li></ul>                                                         |
| ADR       | Media        | <ul><li>Revisión de decisiones previas</li><li>Confirmación de decisiones</li><li>Desafío de decisiones</li><li>Decisiones superadas</li></ul> |

## Artefactos relacionados

Una Nota de validación puede apoyar o ser apoyada por:

| Artefacto                                        | Relación                                                                              |
| ------------------------------------------------ | ------------------------------------------------------------------------------------- |
| [Documento de contexto](context-document.md)     | Actualiza el escenario después de que aparece nueva evidencia.                        |
| [Documento de proceso](process-document.md)      | Confirma o desafía cómo se realiza realmente el trabajo.                              |
| [Documento de caso de uso](use-case-document.md) | Valida comportamiento esperado, consecuencias, errores o reglas.                      |
| [Documento de capacidad](capability-document.md) | Confirma si una capacidad apoya necesidades reales.                                   |
| [Registro de decisión](decision-record.md)       | Valida, desafía o supera una decisión.                                                |
| [Vocabulario de dominio](domain-vocabulary.md)   | Actualiza términos cuando la evidencia aclara el lenguaje.                            |
| [Nota de soporte](support-note.md)               | Captura retroalimentación temprana antes de que se convierta en<br/>aprendizaje validado. |

## Errores comunes

Errores comunes incluyen:

* **tratar entrega como validación**: que algo funcione técnicamente no prueba que haya resuelto el problema correcto.
* **registrar conclusiones sin evidencia**: lectores futuros no pueden entender por qué se confía en el resultado.
* **ignorar resultados negativos**: los supuestos fallidos son aprendizaje valioso.
* **no actualizar artefactos relacionados**: la nota captura aprendizaje, pero la documentación y la implementación permanecen igual.
* **ocultar incertidumbre**: el equipo trata evidencia parcial como verdad final.
* **sobredocumentar pruebas rutinarias**: no todo resultado de prueba necesita una Nota de validación.

## Preguntas de ejemplo

Una Nota de validación debería ayudar a responder:

* ¿Qué fue validado?
* ¿Qué evidencia se reunió?
* ¿Qué fue confirmado, rechazado o cambiado?
* ¿Qué aprendimos?
* ¿Qué supuesto, decisión, comportamiento o capacidad está afectado?
* ¿Qué sigue siendo incierto?
* ¿Qué debería cambiar después?
* ¿La siguiente iteración debería continuar, ajustarse o cambiar de dirección?

## Continuidad

Una Nota de validación preserva continuidad entre entrega y entendimiento renovado.

```text
Implementación o revisión
-> Evidencia
-> Aprendizaje
-> Documentos y decisiones actualizadas
-> Siguiente implementación
-> Evolución
```

Cuando la validación permanece explícita, es menos probable que el equipo repita supuestos equivocados o ignore lo que el sistema enseñó después de ser construido.
