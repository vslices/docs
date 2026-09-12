---
type: finding
state: candidate
code: FND-0001
role: foundational
evidence_level: restricted-retrospective
title: La pérdida de continuidad de conocimiento dificulta mantener, evolucionar y validar sistemas de software

related_questions:
* RQ-001

related_studies:
* stu-001-legacy-ecosystem

related_observations:
* OBS-0001
* OBS-0002
* OBS-0003
* OBS-0004

related_tensions:
* TNS-0001
* TNS-0002

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

# FND-0001 — La pérdida de continuidad de conocimiento dificulta mantener, evolucionar y validar sistemas de software

## Tipo

finding

## Rol

foundational

## Estado

candidate

## Pregunta relacionada

[RQ-001 — Problema fundacional de VSlices Research](../questions/rq-001-problema-fundacional-vslices.md)

## Caso o fuente principal

[Study — Pérdida de continuidad en un ecosistema legacy empresarial](../studies/stu-001-legacy-ecosystem.md)

## Formulación

Esta evidencia sugiere que, en sistemas de software longevos, la pérdida de continuidad de conocimiento entre dominio, flujos, decisiones, comportamiento y software puede dificultar su mantenimiento, evolución, auditoría, validación y modernización.

El finding no plantea que todo sistema antiguo tenga este problema.

Tampoco plantea que la solución sea simplemente producir más documentación.

La formulación central es que un sistema puede seguir funcionando operativamente mientras pierde parte del conocimiento necesario para comprenderlo, modificarlo, justificarlo o renovarlo con seguridad.

## Observaciones que lo sostienen

* [OBS-0001 — Un sistema puede seguir funcionando mientras se pierde comprensión compartida sobre su funcionamiento](../observations/obs-0001-sistema-funciona-sin-comprension-compartida.md)
* [OBS-0002 — La evolución del negocio puede separarse de la evolución del software](../observations/obs-0002-evolucion-negocio-separa-software.md)
* [OBS-0003 — La renovación de un sistema legacy puede requerir reconstruir flujos antes de modificar código](../observations/obs-0003-renovacion-legacy-requiere-reconstruir-flujos.md)
* [OBS-0004 — La falta de continuidad entre dominio, decisiones y software puede convertir la modernización en un proceso de redescubrimiento](../observations/obs-0004-modernizacion-como-redescubrimiento.md)

## Tensiones relacionadas

* [TNS-0001 — Operación funcional vs comprensión insuficiente del sistema](../tensions/tns-0001-operacion-funcional-vs-comprension-insuficiente.md)
* [TNS-0002 — Renovar software vs reconstruir conocimiento perdido](../tensions/tns-0002-renovar-software-vs-reconstruir-conocimiento-perdido.md)

## Evidencia

La evidencia disponible proviene de experiencia profesional retrospectiva y restringida en un ecosistema empresarial legacy.

Por razones de confidencialidad, esta evidencia no incluye artifacts públicos, flujos internos, nombres de sistemas, arquitectura concreta, reglas propietarias, datos operacionales ni detalles identificables de la organización.

La evidencia puede formularse solo en términos generales:

* Se observó que un ecosistema de software podía seguir operando mientras se perdía comprensión compartida sobre su funcionamiento global.
* Se observó que distintas áreas, prácticas o líneas de negocio podían evolucionar de forma distinta al software existente.
* Se observó que una renovación segura requería reconstruir flujos y conocimiento antes de intervenir técnicamente.
* Se observó que la falta de continuidad entre dominio, decisiones y software podía transformar la modernización en un proceso de redescubrimiento.
* Se observó que el conocimiento necesario para evolucionar el sistema podía estar distribuido, implícito, incompleto o desactualizado.

Esta evidencia permite formular un finding fundacional, pero no constituye validación fuerte ni generalizable.

## Interpretación

El problema observado no es únicamente falta de documentación.

La interpretación inicial es que el problema aparece cuando se pierde continuidad entre:

* conocimiento de dominio
* flujos operacionales
* comportamiento esperado
* decisiones históricas
* estructura del software
* implementación existente
* necesidades actuales de evolución
* necesidades de auditoría o validación

Cuando esa continuidad se degrada, el sistema puede conservar continuidad operacional, pero perder continuidad de conocimiento.

Esto produce una forma de fragilidad: el sistema sigue ejecutándose, pero se vuelve más difícil de entender, cambiar, auditar, justificar o renovar.

En ese contexto, mantener o modernizar el sistema puede requerir primero reconstruir conocimiento que no fue preservado de forma explícita, trazable o compartida.

## Alcance

Este finding aplica, de forma inicial y prudente, a sistemas de software longevos donde:

* el dominio ha evolucionado con el tiempo
* el software sostiene múltiples flujos o áreas
* el conocimiento está distribuido entre personas, equipos o prácticas locales
* las decisiones históricas no están suficientemente trazadas
* la documentación existente no explica adecuadamente intención, flujo o comportamiento
* una renovación técnica exige comprender primero el dominio actual
* la operación diaria no garantiza comprensión sistémica

El finding tiene valor principalmente fundacional: ayuda a explicar qué problema práctico motivó a VSlices Research.

## Relación con VSlices

Este finding ayuda a explicar por qué VSlices se enfoca en preservar continuidad entre descubrimiento del dominio, documentación, arquitectura, implementación y evolución.

VSlices no nace solamente para organizar código.

Nace desde la preocupación práctica de que la pérdida de continuidad entre intención, conocimiento, decisiones y artefactos técnicos puede volver difícil la evolución segura de un sistema.

Desde este finding, VSlices Research puede investigar si mecanismos como documentación mínima, continuity paths, estudios vivos, decisiones trazables, artifacts estructurados y tooling progresivo ayudan realmente a preservar continuidad sin introducir burocracia innecesaria.

## Límites

Este finding no demuestra que VSlices resuelva la pérdida de continuidad de conocimiento.

Tampoco demuestra que todos los sistemas legacy pierdan continuidad, ni que toda modernización requiera reconstruir flujos completos antes de modificar código.

No demuestra que la causa principal sea siempre falta de documentación.

No demuestra que más documentación sea la solución suficiente.

La evidencia disponible es retrospectiva, restringida y basada en experiencia profesional previa. Por lo tanto, este finding debe tratarse como fundacional y candidato, no como validado.

## Riesgos de interpretación

* Confundir pérdida de documentación con pérdida de continuidad completa.
* Asumir que documentar más resolvería automáticamente el problema.
* Convertir una experiencia retrospectiva restringida en verdad universal.
* Asumir que todo sistema antiguo está desalineado con el negocio.
* Diseñar mecanismos demasiado pesados para prevenir un problema real pero variable.
* Usar este finding para justificar VSlices sin validar sus mecanismos.
* Confundir continuidad operacional con continuidad de conocimiento.
* Tratar una modernización como problema puramente técnico cuando puede requerir redescubrimiento de dominio.
* Tratar todo redescubrimiento como falla documental, ignorando factores humanos, organizacionales y evolutivos.

## Puede afectar a

* VSlices Research
* VSlices Method
* VSlices Docs Standard
* VSlices Design
* VSlices Framework
* VSlices Tooling

## Próxima evidencia necesaria

Para fortalecer, refinar o descartar este finding, VSlices Research necesita evidencia adicional y documentable.

Evidencia deseable:

* Casos documentables donde la pérdida de continuidad haya producido bloqueos, errores, riesgos, sobrecostos o redescubrimiento.
* Casos donde un sistema siga funcionando, pero no pueda ser explicado suficientemente para evolucionarlo.
* Casos donde la evolución del negocio se haya separado de la evolución del software.
* Casos donde una modernización haya requerido reconstruir dominio, flujos o decisiones.
* Casos donde mecanismos explícitos de continuidad hayan reducido el esfuerzo de redescubrimiento.
* Casos donde documentación existente no haya sido suficiente para preservar continuidad.
* Casos donde mecanismos de VSlices hayan ayudado a preservar continuidad.
* Casos donde mecanismos de VSlices hayan agregado ceremonia sin suficiente valor.

## Estado de madurez

Este finding debe permanecer como `candidate`.

Puede alimentar RQ-001 y orientar estudios futuros, pero no debe convertirse todavía en principio oficial, patrón adoptado o decisión de producto.

Su función actual es fundacional:

> ayuda a explicar el problema práctico que VSlices Research debe investigar, sin demostrar todavía que VSlices sea la solución suficiente o correcta.
