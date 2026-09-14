---
type: observation
state: observed
code: OBS-0011
title: La salida de una persona puede revelar dependencias de conocimiento ocultas durante la operación normal

related_questions:
* RQ-001

related_studies:
* stu-003-key-person-knowledge-transition

related_observations:
* OBS-0010

related_tensions:
* TNS-0007
* TNS-0008

related_findings:
* FND-0003

affects:
* VSlices Research
* VSlices Method
* VSlices Docs Standard
* VSlices Design
* VSlices Tooling

confidentiality:
  level: restricted
  reason: current-professional-transition
  publishable: anonymized-only

evidence:
  level: restricted-live
  artifacts_available: false
  source: current professional experience
---------------------------------------

# OBS-0011 — La salida de una persona puede revelar dependencias de conocimiento ocultas durante la operación normal

## Tipo

observation

## Estado

observed

## Pregunta relacionada

[RQ-001 — Problema fundacional de VSlices Research](../questions/rq-001-problema-fundacional-vslices.md)

## Caso o fuente

[Study — Riesgo de pérdida de conocimiento por salida de una persona clave](../studies/stu-003-key-person-knowledge-transition.md)

## Observación

Observamos que la posible salida de una persona puede revelar dependencias de conocimiento que estaban ocultas o normalizadas durante la operación cotidiana.

En el caso observado, mientras la persona que concentra conocimiento sigue disponible, el equipo puede resolver dudas, desbloquear decisiones, recuperar contexto o diagnosticar problemas recurriendo a ella de forma informal.

Esa disponibilidad puede hacer que la dependencia no parezca crítica.

La observación central es que una dependencia de conocimiento puede permanecer invisible mientras la persona está presente, y volverse evidente solo cuando aparece una salida, transición, cambio de rol o reducción de disponibilidad.

## Contexto

Esta observación aparece desde una experiencia profesional actual y restringida relacionada con una posible transición laboral o salida de una persona que concentra conocimiento relevante.

Durante la operación normal, el equipo puede apoyarse en una persona para responder preguntas como:

* por qué algo funciona de cierta manera
* qué parte del sistema revisar ante un problema
* qué decisión histórica explica una implementación
* qué riesgo existe al modificar una parte
* qué flujo real sostiene una funcionalidad
* qué integración o dependencia debe considerarse
* qué deuda técnica es conocida
* qué comportamiento es esperado y cuál es accidental
* qué pendiente quedó abierto
* a quién acudir para ciertos temas

Mientras esa persona está disponible, la dependencia puede sentirse como colaboración normal.

El riesgo aparece cuando esa disponibilidad deja de estar garantizada.

## Evidencia

La evidencia disponible es actual, profesional y restringida.

Puede formularse solo en términos generales:

* Se observa que una persona concentra conocimiento relevante sobre partes del sistema, dominio, operación o evolución.
* Se observa que ese conocimiento puede ser usado informalmente para resolver dudas o desbloquear trabajo.
* Se observa que no todo ese conocimiento está distribuido, documentado o convertido en artifacts compartidos.
* Se observa que una posible salida hace más visible la dependencia del equipo respecto de ese conocimiento.
* Se observa que la dependencia puede haber permanecido normalizada mientras la persona estaba disponible.
* Se observa que la transición obliga a distinguir qué conocimiento debe quedar disponible para el equipo y qué conocimiento puede reconstruirse después.

No existen artifacts públicos disponibles para esta observación dentro de VSlices Research.

Por razones de confidencialidad, no se documentan nombres de organizaciones, clientes, proveedores, sistemas, servicios, APIs, repositorios, flujos internos, reglas propietarias, datos operacionales, detalles de arquitectura ni información identificable de equipos o personas.

## Interpretación inicial

Esta observación sugiere que la continuidad de conocimiento puede parecer más estable de lo que realmente es cuando depende de disponibilidad humana informal.

Mientras la persona clave está presente, el equipo puede operar sin sentir una ruptura de continuidad, porque el conocimiento se recupera mediante conversaciones, consultas rápidas, memoria personal o intervención directa.

Sin embargo, esa forma de continuidad puede ser frágil.

La salida de la persona no crea necesariamente toda la dependencia, pero sí puede hacerla visible.

Esto permite distinguir entre:

* continuidad aparente: el equipo funciona porque una persona está disponible
* continuidad transferida: el equipo puede recuperar conocimiento sin depender de esa persona
* continuidad documentada o compartida: el conocimiento existe en artifacts, prácticas o personas alternativas
* continuidad validada: otras personas pueden usar el conocimiento transferido para operar o decidir

Desde VSlices Research, esta observación refuerza la necesidad de estudiar cómo detectar dependencias de conocimiento antes de que se transformen en riesgo de salida.

## Observaciones relacionadas

* [OBS-0010 — El conocimiento crítico puede estar activo pero concentrado en una persona clave](../observations/obs-0010-conocimiento-critico-activo-concentrado-persona-clave.md)

## Tensiones relacionadas

* [TNS-0007 — Transferencia suficiente vs documentación exhaustiva](../tensions/tns-0007-transferencia-suficiente-vs-documentacion-exhaustiva.md)
* [TNS-0008 — Responsabilidad profesional de transferencia vs límite personal de salida](../tensions/tns-0008-responsabilidad-profesional-transferencia-vs-limite-personal-salida.md)

## Puede afectar a

* VSlices Research
* VSlices Method
* VSlices Docs Standard
* VSlices Design
* VSlices Tooling

## Límite

Esta observación no demuestra que toda dependencia de conocimiento sea problemática.

En cualquier equipo existen personas con mayor experiencia, contexto o especialización. Esa diferencia puede ser normal y útil.

Tampoco demuestra que toda dependencia deba eliminarse completamente antes de una salida.

La observación solo registra que, en una experiencia profesional actual y restringida, una posible salida hizo visible que parte del conocimiento relevante no estaba suficientemente distribuido o transferido.

Para fortalecer esta observación, VSlices Research necesita casos documentables donde pueda compararse:

* conocimiento usado durante operación normal
* conocimiento realmente disponible sin la persona clave
* consultas frecuentes hechas a la persona
* artifacts existentes
* capacidad del equipo para resolver problemas sin apoyo directo
* riesgos descubiertos durante una transición
* acciones tomadas para reducir dependencia

## Próxima evidencia necesaria

* Casos documentables donde una salida revele dependencia de conocimiento previamente oculta.
* Casos donde la dependencia ya estaba identificada antes de la salida.
* Ejemplos donde la disponibilidad informal de una persona haya ocultado falta de documentación o transferencia.
* Ejemplos donde el equipo haya podido operar sin la persona gracias a conocimiento previamente distribuido.
* Evidencia sobre cómo detectar dependencias de conocimiento antes de una transición.
* Evidencia sobre cómo validar que una dependencia fue reducida.
* Observaciones sobre qué señales muestran que la continuidad depende demasiado de una persona.
* Observaciones sobre qué artifacts o prácticas permiten convertir continuidad aparente en continuidad transferida.
