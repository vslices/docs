---
id: decision.vslices.anamnesis-paths-and-petrov-frontier
type: decision-record
status: active
related:
  - docs/es/decisions/anamnesis-concept-study/0003-transicionar-a-slice-first.md
---

# Seleccionar Continuity Paths y frontier para el primer slice

## Decision

Usar `Consumable Service` como Continuity Path principal para la evolución de Concept bajo presión de Anamnesis, con `Domain Context`, `Software Project` y `Evolution` como supporting paths. Definir como frontier inmediata la materialización de una única trayectoria Petrov determinista usando el Concept actual y manteniendo semántica específica en el consumidor.

## Status

Active.

## Context

La ejecución ya cambió a Slice-First. La tensión principal está en preservar continuidad entre necesidad consumer-driven, materialización específica y posible promoción o rechazo de capacidades reusables.

## Problem or tension

Era necesario orientar el slice sin convertir los Continuity Paths en una lista documental ni asumir que Petrov define Concept.

## Options considered

### Domain Context como path principal

Protege significado experimental, pero no enfatiza suficientemente la relación consumidor/proveedor que se está poniendo a prueba.

### Software Project como path principal

Orienta bien hacia código, pero desplaza la pregunta central de reusabilidad y ownership.

### Consumable Service como path principal

Hace visible la continuidad entre presión del consumidor, capacidad ofrecida y decisión de promoción o permanencia local.

## Selected option

`Consumable Service` principal; `Domain Context`, `Software Project` y `Evolution` como supporting paths.

## Rationale

La pregunta metodológica inmediata no es sólo “¿podemos implementar Petrov?”, sino “¿cómo responde Concept a una necesidad concreta sin absorberla automáticamente en Core?”.

## Consequences

- Petrov permanece como vertical de Anamnesis y no como vocabulario de Concept.
- La implementación debe intentar primero expresar el vertical con el Core actual.
- La primera fricción observable puede cambiar la frontier o los paths.

## Protocol Execution

### Objective

Preservar continuidad desde necesidad de Anamnesis hasta evidencia sobre límites reales de Concept.

### Previous state

Slice-First activo, pero sin navegación formalizada para la relación consumidor/proveedor ni una frontier mínima cerrada.

### Next state

- Principal path: Consumable Service.
- Supporting paths: Domain Context, Software Project, Evolution.
- Frontier: ejecutar una trayectoria Petrov determinista con estado causal explícito, observación parcial, acción, transición y traza reconstruible sin extender Core por anticipación.

## Review conditions

Revisar cuando la primera implementación produzca una fricción que cambie ownership, incertidumbre dominante o el tipo de continuidad que debe preservarse.