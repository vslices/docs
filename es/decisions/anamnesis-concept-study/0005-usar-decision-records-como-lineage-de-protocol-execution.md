---
id: decision.vslices.protocol-execution-decision-lineage
type: decision-record
status: active
related:
  - es/decisions/anamnesis-concept-study/0001-reconocer-context-first-retrospectivamente.md
  - es/decisions/anamnesis-concept-study/0003-transicionar-a-slice-first.md
---

# Usar Decision Records como lineage de Protocol Execution

## Decision

Representar la ejecución del protocolo como una secuencia tail-append de `Decision Record` estándar, complementados cuando sea necesario por una sección `Protocol Execution` que preserve `Objective`, `Previous state` y `Next state`.

## Status

Active.

## Context

Inicialmente se propuso una superficie propia con la estructura `Objetivo → Estado actual → Decisiones → Nuevo estado`. Al revisar el `Decision Record` de VSlices Docs Standard se observó que ya cubre contexto, tensión, alternativas, rationale, tradeoffs, consecuencias y condiciones de revisión.

## Problem or tension

Crear un nuevo tipo documental duplicaría semántica existente antes de demostrar que el Decision Record es insuficiente. Al mismo tiempo, una ejecución del protocolo necesita preservar una secuencia ordenada de cambios de estado, no sólo decisiones aisladas.

## Options considered

### Crear un nuevo tipo `Protocol Execution Record`

Expresa directamente la transición de estado, pero duplica responsabilidades del Decision Record.

### Usar sólo Decision Records sin extensión

Reutiliza el estándar, pero puede hacer menos visible la transición de estado de la ejecución.

### Usar Decision Records con extensión local de Protocol Execution

Mantiene la taxonomía existente y agrega sólo el contexto de estado que esta ejecución necesita.

## Selected option

Decision Records estándar + extensión `Protocol Execution` cuando aporte continuidad.

## Rationale

Antes de ampliar la taxonomía documental, VSlices debe comprobar si el vocabulario extensible actual puede representar honestamente el caso. La carpeta o secuencia de protocol execution funciona como navegación histórica, no como una taxonomía documental independiente.

## Consequences

- Cada entrada material de la ejecución puede seguir siendo un `Decision Record` válido.
- `Protocol Execution` añade únicamente estado de ejecución, no reemplaza rationale, consecuencias o tradeoffs.
- Los registros históricos se agregan como tail-append y no se reescriben para hacer inevitable el estado actual.
- Decisiones externas de Anamnesis o Concept deben referenciarse por su efecto sobre la ejecución, no reapropiarse como decisiones de VSlices Development.

## Protocol Execution

### Objective

Preservar la trayectoria metodológica de una ejecución real de VSlices sin introducir una taxonomía nueva antes de contar con evidencia de necesidad.

### Previous state

Se había creado una superficie `protocol-execution` con una estructura propia de transición y se había considerado su relación por composición con Decision Record.

### Next state

La unidad documental primaria de decisiones será `Decision Record`; la ejecución será una secuencia ordenada de esos records, con extensión de estado cuando sea útil.

## Review conditions

Revisar si varias ejecuciones muestran que `Decision Record + Protocol Execution` resulta forzado, pierde información esencial o requiere campos suficientemente estables como para justificar una construcción nueva.