# Nota de soporte

> Puedes acceder a la [plantilla de nota de soporte aquí](https://github.com/vslices/docs-standard/blob/main/templates/support-note.md)

Una Nota de soporte (*Support Note* en inglés) preserva conocimiento útil que todavía no está listo o no es lo suficientemente importante como para convertirse en un documento formal.

Su propósito es capturar conceptos, supuestos, riesgos, preguntas, retroalimentación, detalles de implementación o ideas de mejora sin agregar estructura innecesaria. Una Nota de soporte responde:

> ¿Qué no deberíamos perder todavía?

Una Nota de soporte es intencionalmente liviana. Más adelante puede fusionarse con un documento, enlazarse desde otro artefacto, superarse o archivarse.

## Propósito

Una Nota de soporte ayuda al equipo a preservar:

* **conocimiento temprano**: ideas, observaciones o hallazgos que todavía están tomando forma.
* **incertidumbre**: supuestos, riesgos, preguntas abiertas y conceptos poco claros.
* **detalle local**: información útil en un contexto específico, pero no lo suficientemente amplia para un documento completo.
* **aprendizaje temporal**: retroalimentación, notas de implementación o descubrimientos que pueden importar más adelante.
* **candidatos futuros**: conocimiento que puede convertirse en parte de un Documento de contexto, Documento de proceso, Documento de caso de uso, Documento de capacidad, Registro de decisión o Nota de validación.

El objetivo es preservar conocimiento útil sin forzar estructura prematura.

## Tipos comunes

## Tipos comunes

Las Notas de soporte pueden incluir:

| Tipo                      | Cuándo usarla                                                                                   | Uso                                                                                                    |
| ------------------------- | ----------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------ |
| Nota de concepto          | Cuando aparece una idea todavía<br/> inmadura.                                                       | Captura un concepto temprano antes de<br/>que se vuelva parte del Vocabulario de<br/>dominio u otro documento. |
| Nota de supuesto          | Cuando algo parece cierto, pero<br/>aún no está validado.                                           | Captura algo que el equipo cree<br/>verdadero, pero que todavía no ha<br/>validado.                            |
| Nota de riesgo            | Cuando algo podría fallar, retrasar<br/>o generar complejidad accidental.                           | Captura una posible fuente de falla,<br/>malentendido, retraso, retrabajo o<br/>complejidad accidental.        |
| Pregunta abierta          | Cuando el equipo todavía necesita<br/>entender algo.                                                | Captura algo que el equipo todavía<br/>necesita entender.                                                  |
| Nota de *feature*         | Cuando surge una idea de *feature*<br/>antes de tener claridad de caso<br/>de uso, capacidad o alcance. | Captura una idea temprana de *feature*<br/>antes de que su caso de uso, capacidad<br/>o alcance estén claros.  |
| Nota de _feedback_ | Cuando alguien aporta información<br/>que puede cambiar entendimiento<br/>o dirección.                  | Captura entrada de usuarios, expertos<br/>de dominio, partes interesadas,<br/>implementación u operación.      |
| Nota de<br/>implementación    | Cuando aparece detalle técnico<br/>útil, pero todavía no hay decisión.                              | Captura detalle técnico útil que todavía<br/>no es un Registro de decisión.                                |
| Nota de alcance           | Cuando algo puede incluirse,<br/>excluirse, postergarse o ignorarse<br/>intencionalmente.               | Captura qué puede incluirse, excluirse,<br/>postergarse o ignorarse<br/>intencionalmente.                      |
| Nota de mejora            | Cuando aparece una mejora posible,<br/>pero todavía no es un cambio<br/>planificado.                    | Captura una posible mejora antes de<br/>que se convierta en un cambio<br/> planificado.                         |

## Cuándo usarla

Usa una Nota de soporte cuando el conocimiento debería preservarse, pero un documento formal sería demasiado. Es especialmente útil cuando:

* **la idea es temprana**: el equipo todavía no sabe dónde pertenece.
* **el conocimiento es incierto**: el equipo necesita seguir un supuesto, riesgo o pregunta.
* **el detalle es local**: la información importa, pero solo en un contexto estrecho.
* **el equipo necesita velocidad**: escribir un documento completo frenaría el aprendizaje sin agregar valor.
* **el conocimiento puede evolucionar**: la nota puede convertirse más adelante en parte de un documento mayor.

## Cuándo no usarla

Una Nota de soporte puede ser insuficiente cuando:

* **el conocimiento es estable y reutilizado**: un documento formal puede ser mejor.
* **la nota afecta decisiones importantes**: puede necesitarse un Registro de decisión.
* **la nota describe comportamiento esperado**: un Documento de caso de uso puede ser más claro.
* **la nota describe un proceso**: un Documento de proceso puede ser mejor.
* **la nota valida algo importante**: puede necesitarse una Nota de validación.
* **demasiadas notas repiten el mismo tema**: probablemente el conocimiento debería consolidarse.

## Estructura sugerida

Usa la estructura más pequeña que preserve la nota.

```md
# Support Note

## Type

Concepto, supuesto, riesgo, pregunta, retroalimentación, implementación, alcance o mejora.

## Note

¿Qué debería preservarse?

## Context

¿Dónde apareció esto?

## Why it matters

¿Por qué podría importar más adelante?

## Status

Abierta, activa, resuelta, superada o archivada.

## Related artifacts

¿Qué documentos, decisiones o notas están conectados?
```

## Afinidad con estándares

Este documento puede apoyar la alineación con estándares y prácticas de documentación existentes. No vuelve la documentación conforme por sí mismo.

| Estándar           | Afinidad | Soporta                                                                                                                                   |
| ------------------ | -------- | ----------------------------------------------------------------------------------------------------------------------------------------- |
| ISO/IEC/IEEE 29148 | Media    | <ul><li>Supuestos</li><li>Riesgos</li><li>Preguntas abiertas</li><li>Retroalimentación</li><li>Entradas tempranas de requisitos</li></ul> |
| ISO/IEC/IEEE 42010 | Media    | <ul><li>Intereses tempranos</li><li>Notas de partes interesadas</li><li>Entradas de justificación</li><li>Relaciones</li></ul>            |

| Práctica  | Afinidad | Soporta                                                                                                                                |
| --------- | -------- | -------------------------------------------------------------------------------------------------------------------------------------- |
| arc42     | Media    | <ul><li>Riesgos</li><li>Restricciones</li><li>Preguntas abiertas</li><li>Candidatos de glosario</li><li>Entradas de decisión</li></ul> |
| C4 Model  | Baja     | <ul><li>Notas tempranas sobre límites</li><li>Sistemas</li><li>Responsabilidades</li></ul>                                             |
| 4+1 Model | Baja     | <ul><li>Notas tempranas relacionadas con escenarios</li><li>Comportamiento</li><li>Vistas</li></ul>                                    |
| ADR       | Media    | <ul><li>Entradas tempranas de decisión</li><li>Opciones</li><li>Supuestos</li><li>Riesgos</li></ul>                                    |

## Errores comunes

Errores comunes incluyen:

* **usar notas para siempre**: el conocimiento estable nunca se convierte en documentación formal.
* **crear demasiadas notas desconectadas**: el conocimiento útil se vuelve difícil de encontrar.
* **ocultar decisiones importantes**: se usa una nota cuando se necesita un Registro de decisión.
* **tratar supuestos como hechos**: la incertidumbre desaparece de la documentación.
* **no resolver preguntas**: las preguntas abiertas siguen abiertas después de que el equipo aprende la respuesta.
* **no consolidar notas repetidas**: el conocimiento relacionado permanece fragmentado.

## Preguntas de ejemplo

Una Nota de soporte debería ayudar a responder:

* ¿Qué conocimiento útil no debería perderse?
* ¿Esto es un concepto, supuesto, riesgo, pregunta, retroalimentación, detalle de implementación, nota de alcance o idea de mejora?
* ¿Dónde apareció este conocimiento?
* ¿Por qué podría importar más adelante?
* ¿Sigue abierta, activa, resuelta, superada o archivada?
* ¿Debería esta nota convertirse en parte de un documento formal?

## Continuidad

Una Nota de soporte preserva continuidad entre descubrimiento temprano y documentación estructurada.

```text
Observación o idea
-> Nota de soporte
-> Documento o decisión relacionada
-> Validación o archivo
-> Aprendizaje futuro
```

Cuando las notas permanecen livianas, el equipo puede preservar conocimiento emergente sin convertir cada observación en un documento formal.
