# Escenario "Digitalizado"

Un escenario "Digitalizado" es un contexto de trabajo donde el software ya representa parte del negocio, proceso u organización.

Esto no significa que el dominio ya esté entendido. El software existente es evidencia, no es automáticamente la verdad del dominio.

## Idea central

En un escenario digitalizado, VSlices Method ayuda al equipo a separar tres cosas:

* cómo ocurre realmente el trabajo
* cómo el software actual representa ese trabajo
* cómo las personas han adaptado su trabajo alrededor del software

!!! principle "Principio de continuidad"

    El objetivo no es hacer ingeniería inversa de todo el sistema. Es recuperar suficiente continuidad para tomar la siguiente decisión responsable.


## Cuándo aplica esta guía

Usa esta guía cuando:

* ya existe software
* los flujos de trabajo están parcial o totalmente soportados por un sistema
* las personas dependen de pantallas, reportes, formularios, APIs o automatizaciones actuales
* el equipo necesita mejorar, reemplazar o extender comportamiento existente
* la documentación falta, está desactualizada o está desconectada de la implementación
* el conocimiento de negocio está oculto dentro de código, tickets o hábitos de usuario

Esta guía puede aplicarse aunque el proyecto ya use o no use VSlices Method.

## Riesgo principal

El riesgo principal es tratar el software existente como la verdad del dominio.

Un sistema puede contener:

* reglas reales de negocio
* decisiones obsoletas
* workarounds convertidos en comportamiento
* restricciones accidentales
* compromisos técnicos
* conceptos faltantes
* nombres engañosos
* comportamientos que los usuarios aprendieron a tolerar

!!! risk "Riesgo a evitar"

    Si el equipo copia el sistema existente sin cuestionarlo, puede preservar complejidad accidental como si fuera conocimiento del dominio.


## Modalidad inicial útil

Un escenario digitalizado normalmente comienza con [**Context-First**](../../../design/modalities/context-first/index.md) o [**Problem-First**](../../../design/modalities/problem-first/index.md), porque el equipo necesita entender qué representa el sistema actual y qué problema conviene resolver primero.

| Situación                                                                 | Modalidad útil                                                     | Razón                                                                              |
| ------------------------------------------------------------------------- | ------------------------------------------------------------------ | ---------------------------------------------------------------------------------- |
| El sistema existe, pero el contexto de negocio circundante no está claro. | **Context-First**                                                  | El equipo necesita entender qué está intentando representar el software.           |
| Existe un dolor claro en el sistema actual, pero la causa no está clara.  | **Problem-First**                                                  | El equipo necesita entender el problema antes de cambiar el comportamiento.        |
| Una mejora pequeña y segura puede revelar evidencia útil.                 | [**Slice-First**](../../../design/modalities/slice-first/index.md) | El equipo puede aprender mediante un cambio acotado sin pretender entenderlo todo. |

!!! risk "Riesgo a evitar"

    Slice-First puede ser útil, pero solo cuando el cambio es lo suficientemente pequeño como para evitar propagar supuestos mal entendidos.


## Afinidad con caminos de continuidad

Un escenario digitalizado normalmente tiene mayor afinidad con los caminos que ayudan a recuperar continuidad entre el trabajo real, el software existente y la siguiente decisión de cambio.

No todos los caminos deben recorrerse con la misma profundidad.

| Camino de continuidad | Afinidad típica | Uso en este contexto                                                                                                                     |
| --------------------- | --------------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
| Escenario de negocio  | Alta            | Entender qué trabajo real está representando o asistiendo el software actual.                                                            |
| Contexto de dominio   | Alta            | Separar lenguaje, reglas y significados del dominio de nombres, restricciones o decisiones accidentales del sistema.                     |
| Proyecto de software  | Alta            | Ubicar la iniciativa técnica, los límites del cambio, las dependencias existentes y los riesgos de implementación.                       |
| Producto al cliente   | Media           | Entender comportamiento visible para usuarios cuando el cambio afecta pantallas, formularios, reportes o flujos de uso.                  |
| Servicio consumible   | Media           | Entender capacidades expuestas o consumidas cuando el cambio afecta APIs, integraciones, automatizaciones o dependencias entre sistemas. |

!!! principle "Principio de afinidad"

    Parte desde el camino que mejor explica la continuidad en riesgo. No fuerces todo escenario digitalizado a recorrer todos los caminos.


En un escenario digitalizado, el camino principal suele depender del tipo de cambio.

| Cambio observado                                                         | Camino que conviene priorizar |
| ------------------------------------------------------------------------ | ----------------------------- |
| El sistema no refleja bien cómo ocurre el trabajo actual.                | Escenario de negocio          |
| Los términos del sistema no coinciden con el lenguaje del negocio.       | Contexto de dominio           |
| El equipo necesita modificar una base de código existente con seguridad. | Proyecto de software          |
| El comportamiento visible para usuarios necesita cambiar.                | Producto al cliente           |
| Una API, integración o automatización necesita cambiar.                  | Servicio consumible           |

!!! risk "Riesgo de sobre-recuperación"

    Recuperar continuidad no significa documentar todo el sistema existente. Significa preservar lo necesario para cambiarlo sin perder intención.


## Qué observar primero

Antes de cambiar el sistema, observa cómo el trabajo actual se conecta con el software actual.

| Observa                                                                       | Para entender                                                    |
| ----------------------------------------------------------------------------- | ---------------------------------------------------------------- |
| Qué trabajo real apoya este software                                          | Qué parte del negocio está siendo representada o asistida.       |
| Qué flujos de trabajo dependen de él                                          | Qué procesos podrían verse afectados por un cambio.              |
| Qué actores lo usan directa o indirectamente                                  | Quiénes dependen del comportamiento actual.                      |
| Qué partes del sistema son confiables                                         | Qué comportamiento puede tratarse como evidencia estable.        |
| Qué partes se evitan, se corrigen manualmente o se rodean                     | Qué fricciones revelan límites del sistema actual.               |
| Qué términos de negocio aparecen en la interfaz, el código o la documentación | Qué lenguaje puede revelar intención de dominio.                 |
| Qué comportamientos se esperan pero no son explícitos                         | Qué conocimiento puede estar oculto en uso, soporte u operación. |
| Qué errores o excepciones ocurren repetidamente                               | Qué fragilidades deberían entenderse antes de cambiar.           |
| Qué decisiones son históricas, técnicas o ya no se entienden                  | Qué partes requieren recuperación de contexto antes de avanzar.  |

El objetivo no es hacer un análisis completo. Es encontrar dónde falta continuidad.

## Conocimiento a preservar

Preserva conocimiento cuando afecta el siguiente cambio.

El conocimiento útil puede incluir:

* términos del dominio encontrados en el sistema
* diferencias entre el trabajo real y el comportamiento del software
* flujos de trabajo existentes afectados por el cambio
* reglas ocultas dentro de la implementación
* workarounds de usuarios
* dolores actuales
* restricciones creadas por integraciones o datos
* decisiones que deberían mantenerse, cambiarse o cuestionarse
* señales de validación desde usuarios, soporte u operación

!!! principle "Principio de continuidad"

    No documentes todo el sistema existente por defecto.

    Preserva lo que el trabajo futuro no debería tener que redescubrir.


## Apoyo documental

Los documentos pueden ayudar a recuperar continuidad en un escenario digitalizado.

| Necesidad de conocimiento                                          | Documento útil                                                                                                                                                                             |
| ------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Los términos son ambiguos o inconsistentes.                        | Domain Vocabulary — [Taxonomy](../../../docs-standard/taxonomy/domain-vocabulary.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/domain-vocabulary.md)       |
| El escenario de negocio circundante no está claro.                 | Context Document — [Taxonomy](../../../docs-standard/taxonomy/context-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/context-document.md)          |
| El trabajo actual depende de workflows o handoffs.                 | Process Document — [Taxonomy](../../../docs-standard/taxonomy/process-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/process-document.md)          |
| Un comportamiento específico necesita cambiarse o preservarse.     | Use Case Document — [Taxonomy](../../../docs-standard/taxonomy/use-case-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/use-case-document.md)       |
| Está emergiendo una habilidad estable del negocio.                 | Capability Document — [Taxonomy](../../../docs-standard/taxonomy/capability-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/capability-document.md) |
| Debe elegirse una dirección bajo tradeoffs.                        | Decision Record — [Taxonomy](../../../docs-standard/taxonomy/decision-record.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/decision-record.md)             |
| Evidencia desde uso, operación o revisión cambia el entendimiento. | Validation Note — [Taxonomy](../../../docs-standard/taxonomy/validation-note.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/validation-note.md)             |
| Las observaciones todavía son locales, inciertas o temporales.     | Support Note — [Taxonomy](../../../docs-standard/taxonomy/support-note.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/support-note.md)                      |

Usa el documento más liviano que proteja continuidad.

{% include-markdown "shared/readings/document-stage-affinity-admonition.md" %}

## Enfoque sugerido

Comienza seleccionando un área de cambio. No intentes entender primero todo el sistema.

Un enfoque útil es:

1. Identificar el dolor actual, la oportunidad o la solicitud de cambio
2. Ubicar los flujos de trabajo, actores y comportamiento del sistema alrededor de eso
3. Comparar el comportamiento actual del software con el trabajo real
4. Nombrar lo que se sabe, lo que es incierto y lo que es riesgoso
5. Identificar el camino de continuidad que mejor explica el riesgo del cambio
6. Guardar solo el conocimiento necesario para la siguiente decisión responsable
7. Elegir el cambio pequeño más seguro o la siguiente investigación
8. Usar feedback para actualizar el entendimiento

El equipo debería moverse entre entender y construir a medida que aparece evidencia.

## Errores comunes

Los escenarios digitalizados suelen fallar cuando los equipos asumen que el sistema se explica solo.

Algunos errores comunes incluyen:

* copiar comportamiento existente sin entender por qué existe
* rediseñarlo todo porque el sistema actual se ve desordenado
* tratar nombres del código como lenguaje del dominio
* ignorar workarounds de usuarios
* documentar todo el sistema antes de mejorar algo
* cambiar comportamiento sin saber quién depende de él
* asumir que las decisiones antiguas siguen siendo válidas
* asumir que las decisiones antiguas estaban mal solo porque son antiguas
* recorrer todos los caminos de continuidad como si fueran obligatorios

!!! risk "No confundas evidencia con verdad"

    El software existente debería respetarse como evidencia.

    No debería obedecerse como verdad.


## Principio guía

!!! principle "Principio General"

    Usa el sistema existente como una fuente de pistas.

    No conserves complejidad accidental a menos que el dominio todavía dependa de ella.


Recupera suficiente continuidad de dominio, proceso, comportamiento y decisión para cambiar el sistema con seguridad.
