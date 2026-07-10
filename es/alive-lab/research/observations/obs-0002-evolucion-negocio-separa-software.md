---
type: observation
state: observed
code: OBS-0002
title: La evolución del negocio puede separarse de la evolución del software

related_questions:
* RQ-001

related_studies:
* STU-001

related_findings:
* FND-0001

related_tensions:
* TNS-0002

affects:
* VSlices Research
* VSlices Method
* VSlices Docs Standard
* VSlices Design

confidentiality:
  level: restricted
  reason: professional-experience
  publishable: anonymized-only

evidence:
  level: restricted-retrospective
  artifacts_available: false
  source: professional experience

---

# OBS-0002 — La evolución del negocio puede separarse de la evolución del software

## Tipo

observation

## Estado

observed

## Pregunta relacionada

[RQ-001 — Problema fundacional de VSlices Research](../questions/rq-001-problema-fundacional-vslices.md)

## Caso o fuente

[STU-001 — Pérdida de continuidad en un ecosistema legacy empresarial](../studies/stu-001-legacy-ecosystem-knowledge-loss.md)

## Observación

Observamos que la evolución de un negocio puede separarse progresivamente de la evolución del software que originalmente intentaba representarlo o sostenerlo.

En el caso observado, distintas áreas, líneas de negocio o prácticas operacionales habían seguido evolucionando con el tiempo. Sin embargo, esa evolución no necesariamente quedó reflejada de forma clara, completa o actualizada en el software existente.

Esto produjo una brecha entre:

* cómo la organización operaba actualmente
* cómo el software representaba el negocio
* qué conocimiento histórico explicaba esa representación
* qué decisiones seguían siendo válidas
* qué partes del sistema correspondían al dominio actual
* qué partes reflejaban necesidades antiguas, adaptaciones locales o deuda acumulada

La observación central es que el software puede seguir siendo usado aunque su modelo implícito del negocio deje de coincidir plenamente con la realidad operacional actual.

## Contexto

Esta observación aparece desde una experiencia profesional retrospectiva y restringida con un ecosistema empresarial legacy de larga evolución.

Durante una iniciativa de renovación o modernización, no bastaba con mirar el software existente como fuente única de verdad. Era necesario levantar flujos, prácticas y necesidades actuales del negocio para entender qué seguía vigente, qué había cambiado y qué partes del sistema ya no representaban correctamente la operación real.

El problema no era solamente que el software tuviera años de existencia.

El problema era que el negocio había seguido vivo, cambiando y adaptándose, mientras la continuidad entre dominio, decisiones y software se había debilitado.

## Evidencia

La evidencia disponible es retrospectiva y restringida.

Puede formularse solo en términos generales:

* Se observó que el sistema existente seguía sosteniendo operaciones reales.
* Se observó que algunas áreas o líneas de negocio habían evolucionado con el tiempo.
* Se observó que no toda evolución del negocio estaba reflejada claramente en el software.
* Se observó que antes de renovar el sistema era necesario reconstruir flujos actuales del negocio.
* Se observó que el software existente no podía tratarse automáticamente como representación completa del dominio actual.

No existen artifacts públicos disponibles para esta observación dentro de VSlices Research.

Por razones de confidencialidad, no se documentan nombres, flujos internos, módulos, arquitectura, reglas de negocio, datos operacionales ni detalles identificables de la organización.

## Interpretación inicial

Esta observación sugiere que la continuidad entre negocio y software no se preserva automáticamente por el solo hecho de que el sistema siga funcionando.

Un sistema puede permanecer operativo mientras el negocio cambia alrededor de él. En ese escenario, el software puede convertirse en una mezcla de:

* necesidades actuales
* decisiones históricas
* reglas parcialmente vigentes
* adaptaciones manuales
* conocimiento local
* comportamiento heredado
* automatizaciones que ya no explican completamente el dominio

Esto refuerza la idea de que renovar un sistema no debería comenzar solo desde el código existente.

También requiere reconstruir el dominio actual y comparar qué tan bien el software todavía lo representa.

## Tensión relacionada

TNS-0002 — Renovar software vs reconstruir conocimiento perdido

La tensión aparece porque una renovación técnica puede parecer, inicialmente, un problema de reemplazo o modernización de software.

Sin embargo, si el negocio evolucionó de forma distinta al sistema, renovar el software requiere primero recuperar conocimiento sobre el dominio actual, sus flujos reales y sus necesidades vigentes.

## Puede afectar a

* VSlices Research
* VSlices Method
* VSlices Docs Standard
* VSlices Design
* VSlices Framework

## Límite

Esta observación no demuestra que todo sistema legacy esté desalineado con el negocio.

Tampoco demuestra que la separación entre negocio y software sea siempre negativa. En algunos casos, el software puede permanecer estable mientras el negocio cambia solo en prácticas externas, acuerdos humanos o procesos complementarios.

La observación solo registra que, en una experiencia profesional retrospectiva y restringida, se observó una separación progresiva entre evolución del negocio y evolución del software.

Para fortalecer esta observación, VSlices Research necesita casos documentables donde pueda compararse:

* dominio esperado
* operación real actual
* comportamiento del software
* documentación existente
* decisiones históricas
* cambios de negocio posteriores
* esfuerzo necesario para realinear software y dominio

## Próxima evidencia necesaria

* Casos documentables donde el negocio haya cambiado más rápido o de forma distinta al software.
* Ejemplos donde el software siga funcionando, pero represente parcialmente el dominio actual.
* Evidencia de decisiones históricas que dejaron de estar alineadas con necesidades actuales.
* Casos donde documentación viva permita detectar desalineación más temprano.
* Casos donde continuity paths ayuden a conectar evolución del dominio con evolución del software.
* Casos donde VSlices Method ayude a distinguir entre renovar código y redescubrir dominio.
