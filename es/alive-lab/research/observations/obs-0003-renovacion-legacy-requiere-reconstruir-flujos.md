---
type: observation
state: observed
code: OBS-0003
title: La renovación de un sistema legacy puede requerir reconstruir flujos antes de modificar código
related_questions:
* RQ-001

related_studies:
* STU-001

related_observations:
* OBS-0001
* OBS-0002

related_tensions:
* TNS-0002

related_findings:
* FND-0001

affects:
* VSlices Research
* VSlices Method
* VSlices Docs Standard
* VSlices Design
* VSlices Framework

confidentiality:
  level: restricted
  reason: professional-experience
  publishable: anonymized-only

evidence:
  level: restricted-retrospective
  artifacts_available: false
  source: professional experience
---

# OBS-0003 — La renovación de un sistema legacy puede requerir reconstruir flujos antes de modificar código

## Tipo

observation

## Estado

observed

## Pregunta relacionada

[RQ-001 — Problema fundacional de VSlices Research](../questions/rq-001-problema-fundacional-vslices.md)

## Caso o fuente

[STU-001 — Pérdida de continuidad en un ecosistema legacy empresarial](../studies/stu-001-legacy-ecosystem-knowledge-loss.md)

## Observación

Observamos que la renovación de un sistema legacy puede requerir reconstruir flujos de negocio y operación antes de modificar, reemplazar o reimplementar código.

En el caso observado, el sistema existente seguía operando, pero no era suficiente mirar solo el código o las aplicaciones existentes para comprender qué debía renovarse.

Antes de intervenir técnicamente, era necesario levantar y reconstruir conocimiento sobre:

* qué flujos existían realmente
* qué áreas participaban en esos flujos
* qué acciones estaban encadenadas
* qué reglas seguían vigentes
* qué comportamientos eran intencionales
* qué comportamientos eran herencia histórica
* qué partes del sistema representaban el negocio actual
* qué partes estaban desalineadas con la operación real

La observación central es que, en ciertos sistemas legacy, renovar software no empieza necesariamente modificando código. Puede empezar recuperando el flujo que el código ya no explica suficientemente.

## Contexto

Esta observación aparece desde una experiencia profesional retrospectiva y restringida con un ecosistema empresarial legacy de larga evolución.

Durante una iniciativa de renovación, el problema no era únicamente cambiar tecnología o reemplazar aplicaciones antiguas. El problema era que la continuidad entre dominio, flujos, decisiones y software se había debilitado con el tiempo.

El software existente entregaba señales parciales, pero no una comprensión completa del sistema como conjunto.

Por eso, la renovación requería reconstruir primero parte del conocimiento perdido antes de definir cómo intervenir técnicamente.

## Evidencia

La evidencia disponible es retrospectiva y restringida.

Puede formularse solo en términos generales:

* Se observó que el sistema existente no podía tratarse como fuente única de verdad.
* Se observó que distintos flujos debían levantarse antes de renovar.
* Se observó que el conocimiento necesario para renovar estaba distribuido, implícito o incompleto.
* Se observó que la operación actual no siempre coincidía claramente con la estructura del software existente.
* Se observó que modificar código sin reconstruir flujos podía aumentar el riesgo de perder comportamientos necesarios.

No existen artifacts públicos disponibles para esta observación dentro de VSlices Research.

Por razones de confidencialidad, no se documentan nombres, flujos internos, módulos, arquitectura, reglas de negocio, datos operacionales ni detalles identificables de la organización.

## Interpretación inicial

Esta observación sugiere que, cuando se pierde continuidad de conocimiento, la renovación de software puede transformarse en un proceso de redescubrimiento.

El código existente puede mostrar cómo algo está implementado, pero no necesariamente explicar:

* por qué existe
* qué necesidad resolvía
* qué flujo completo sostiene
* qué decisiones históricas lo justifican
* qué partes siguen siendo válidas
* qué partes deberían cambiar
* qué consecuencias tendría modificarlo

Esto refuerza la idea de que una renovación segura puede requerir reconstruir continuidad antes de reconstruir software.

## Observaciones relacionadas

* [OBS-0001 — Un sistema puede seguir funcionando mientras se pierde comprensión compartida sobre su funcionamiento](../observations/obs-0001-sistema-funciona-sin-comprension-compartida.md)
* [OBS-0002 — La evolución del negocio puede separarse de la evolución del software](../observations/obs-0002-evolucion-negocio-separa-software.md)

## Tensión relacionada

[TNS-0002 — Renovar software vs reconstruir conocimiento perdido](../tensions/tns-0002-renovar-software-vs-reconstruir-conocimiento-perdido.md)

La tensión aparece porque una iniciativa de renovación puede parecer un problema técnico, pero en contextos donde la continuidad se perdió, puede requerir primero reconstruir conocimiento de dominio, flujos y decisiones.

## Puede afectar a

* VSlices Research
* VSlices Method
* VSlices Docs Standard
* VSlices Design
* VSlices Framework

## Límite

Esta observación no demuestra que toda renovación de sistemas legacy requiera levantar todos los flujos antes de modificar código.

Tampoco demuestra que el código sea inútil como fuente de conocimiento. El código puede contener información valiosa, pero no siempre expresa de forma suficiente la intención, el flujo completo, las decisiones históricas o la alineación con el dominio actual.

La observación solo registra que, en una experiencia profesional retrospectiva y restringida, renovar un sistema legacy apareció vinculado a la necesidad de reconstruir flujos antes de intervenir técnicamente.

Para fortalecer esta observación, VSlices Research necesita casos documentables donde pueda compararse:

* conocimiento disponible antes de renovar
* flujos reconstruidos durante la renovación
* decisiones técnicas tomadas después del levantamiento
* riesgos evitados por comprender el flujo antes de modificar código
* costo de renovar sin reconstruir conocimiento suficiente

## Próxima evidencia necesaria

* Casos documentables donde una renovación técnica haya requerido levantar flujos antes de modificar código.
* Ejemplos donde el código existente no haya sido suficiente para comprender el comportamiento completo.
* Ejemplos donde reconstruir flujos haya reducido riesgo durante una renovación.
* Casos donde se haya levantado demasiado conocimiento y eso haya generado burocracia.
* Evidencia sobre qué nivel mínimo de reconstrucción de flujo permite intervenir con seguridad.
* Observaciones en Alive Lab sobre cómo VSlices puede preservar continuidad para evitar redescubrimientos tardíos.
