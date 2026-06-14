# Escenario "Digitalizado"

Los escenarios ya "digitalizados" (*Digitalized Scenarios* en inglés) son contextos de trabajo donde el _software_ ya representa parte del negocio, proceso u organización.

Esto no significa que el dominio ya se entienda. El _software_ existente es evidencia, no es automáticamente verdad del dominio.

## Idea central

En un escenario digitalizado, *VSlices Method* ayuda al equipo a separar tres cosas:

* cómo ocurre realmente el trabajo
* cómo el _software_ actual representa ese trabajo
* cómo las personas han adaptado su trabajo alrededor del _software_

El objetivo no es hacer ingeniería inversa de todo el sistema. Es recuperar suficiente continuidad para tomar la siguiente decisión responsable.

## Cuándo aplica esta guía

Usa esta guía cuando:

* ya existe _software_
* los _workflows_ están parcial o totalmente soportados por un sistema
* las personas dependen de pantallas, reportes, formularios, *APIs* o automatizaciones actuales
* el equipo necesita mejorar, reemplazar o extender comportamiento existente
* la documentación falta, está desactualizada o está desconectada de la implementación
* el conocimiento de negocio está oculto dentro de código, tickets o hábitos de usuarios

Esta guía puede aplicar aunque el proyecto ya use o no use *VSlices Method*.

## Riesgo principal

El riesgo principal es tratar el software existente como la verdad del dominio. Un sistema puede contener:

* reglas reales de negocio
* decisiones obsoletas
* comportamientos de workaround
* restricciones accidentales
* compromisos técnicos
* conceptos faltantes
* nombres engañosos
* comportamientos que los usuarios aprendieron a tolerar

Si el equipo copia el sistema existente sin cuestionarlo, puede preservar complejidad accidental como si fuera conocimiento de dominio.

## Modalidad inicial útil

Un escenario digitalizado normalmente comienza con *Context-First* o *Problem-First*.

| Situación                                                                 | Modalidad útil                                                        | Razón                                                                              |
| ------------------------------------------------------------------------- | --------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| El sistema existe, pero el<br/>contexto de negocio<br/>circundante no está claro. | [**_Context-First_**](../../design/modalities/context-first/index.md) | El equipo necesita entender qué está intentando<br/>representar el software.           |
| Existe un dolor claro en el<br/>sistema actual, pero la<br/>causa no está clara.  | [**_Problem-First_**](../../design/modalities/problem-first/index.md) | El equipo necesita entender el problema antes de<br/>cambiar comportamiento.           |
| Una mejora pequeña y segura<br/>puede revelar evidencia útil.                 | [**_Slice-First_**](../../design/modalities/slice-first/index.md)     | El equipo puede aprender mediante un cambio<br/>acotado sin pretender entenderlo todo. |

*Slice-First* puede ser útil, pero solo cuando el cambio es lo suficientemente pequeño como para evitar propagar supuestos mal entendidos.

## Qué observar primero

Antes de cambiar el sistema, observa cómo el trabajo actual se conecta con el _software_ actual. Algunas preguntas útiles incluyen:

* ¿Qué trabajo real apoya este _software_?
* ¿Qué _workflows_ dependen de él?
* ¿Qué actores lo usan directa o indirectamente?
* ¿Qué partes del sistema son confiables?
* ¿Qué partes se evitan, se corrigen manualmente o se rodean?
* ¿Qué términos de negocio aparecen en la interfaz, el código o la documentación?
* ¿Qué comportamientos se esperan, pero no están explícitos?
* ¿Qué errores o excepciones ocurren repetidamente?
* ¿Qué decisiones son históricas, técnicas o ya no se entienden?

El objetivo no es un análisis completo. Es encontrar dónde falta continuidad.

## Conocimiento a preservar

Preserva conocimiento cuando afecta el siguiente cambio. El conocimiento útil puede incluir:

* términos de dominio encontrados en el sistema
* diferencias entre el trabajo real y el comportamiento del _software_
* _workflows_ existentes afectados por el cambio
* reglas ocultas dentro de la implementación
* _workarounds_ de usuarios
* dolores actuales
* restricciones creadas por integraciones o datos
* decisiones que deberían mantenerse, cambiarse o cuestionarse
* señales de validación desde usuarios, soporte u operación

No documentes todo el sistema existente por defecto. Preserva lo que el trabajo futuro no debería tener que redescubrir.

## Soporte documental

Los documentos pueden ayudar a recuperar continuidad en un escenario digitalizado.

| Necesidad de conocimiento                                             | Documento útil                                                                                                                                                                                                      |
| --------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Los términos son ambiguos o<br/> inconsistentes.                           | Vocabulario de dominio  — [Taxonomía](../../docs-standard/taxonomy/domain-vocabulary.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/domain-vocabulary.md)       |
| El escenario de negocio<br/>circundante no está claro.                    | Documento de contexto — [Taxonomía](../../docs-standard/taxonomy/context-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/context-document.md)           |
| El trabajo actual depende de<br/>workflows o handoffs.                    | Documento de proceso — [Taxonomía](../../docs-standard/taxonomy/process-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/process-document.md)            |
| Un comportamiento específico<br/>necesita cambiarse o preservarse.        | Documento de caso de uso — [Taxonomía](../../docs-standard/taxonomy/use-case-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/use-case-document.md)     |
| Está emergiendo una<br/>capacidad estable de negocio.                     | Documento de capacidad — [Taxonomía](../../docs-standard/taxonomy/capability-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/capability-document.md) |
| Debe elegirse una dirección<br/>bajo tradeoffs.                           | Registro de decisión — [Taxonomía](../../docs-standard/taxonomy/decision-record.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/decision-record.md)               |
| La evidencia desde uso,<br/>operación o revisión cambia el<br/>entendimiento. | Nota de validación — [Taxonomía](../../docs-standard/taxonomy/validation-note.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/validation-note.md)                 |
| Las observaciones todavía<br/>son locales, inciertas o temporales.        | Nota de soporte — [Taxonomía](../../docs-standard/taxonomy/support-note.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/support-note.md)                             |

Usa el documento más ligero que proteja la continuidad.

> La afinidad documento y etapa (*Document-Stage affinity*) se describe en la página [afinidad documento y etapa](../document-stage-affinity.md).

## Enfoque sugerido

Comienza seleccionando un área de cambio. No intentes entender todo el sistema primero.

Un enfoque útil es:

1. Identificar el dolor, oportunidad o solicitud de cambio actual.
2. Ubicar los _workflows_, actores y comportamiento del sistema alrededor de eso.
3. Comparar el comportamiento actual del _software_ con el trabajo real.
4. Nombrar lo conocido, lo incierto y lo riesgoso.
5. Preservar solo el conocimiento necesario para la siguiente decisión responsable.
6. Elegir el cambio seguro más pequeño o la siguiente investigación.
7. Usar _feedback_ para actualizar el entendimiento.

El equipo debería moverse entre entender y construir a medida que aparece evidencia.

## Errores comunes

Los escenarios digitalizados suelen fallar cuando los equipos asumen que el sistema se explica por sí mismo. Algunos errores comunes incluyen:

* copiar comportamiento existente sin entender por qué existe
* rediseñarlo todo porque el sistema actual parece desordenado
* tratar nombres de código como lenguaje de dominio
* ignorar _workarounds_ de usuarios
* documentar todo el sistema antes de mejorar cualquier cosa
* cambiar comportamiento sin saber quién depende de él
* asumir que las decisiones antiguas todavía son válidas
* asumir que las decisiones antiguas estaban mal solo porque son antiguas

El _software_ existente debería respetarse como evidencia. No debería obedecerse como verdad.

## Principio guía

Usa el sistema existente como fuente de pistas. Recupera suficiente continuidad de dominio, proceso, comportamiento y decisión para cambiar el sistema de forma segura.

No preserves complejidad accidental a menos que el dominio todavía dependa de ella.
