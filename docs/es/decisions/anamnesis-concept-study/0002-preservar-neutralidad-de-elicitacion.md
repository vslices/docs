---
id: decision.vslices.consumer-elicitation-neutrality
type: decision-record
status: active
related:
  - docs/es/decisions/anamnesis-concept-study/0001-reconocer-context-first-retrospectivamente.md
---

# Preservar neutralidad de elicitación frente al consumidor

## Decision

Separar la incertidumbre dirigida al consumidor de la incertidumbre interna del proveedor y evitar introducir proveedor, mecanismo, arquitectura o espacio de solución en la pregunta primaria cuando eso pueda contaminar la necesidad expresada.

## Status

Active.

## Context

Durante el primer discovery se formuló inicialmente una pregunta con la forma aproximada: `¿Cuál es la primera necesidad real de Anima que todavía no sabemos cómo satisfacer usando Concept?`. Aunque se aclaró después que Anima no debía traducir la necesidad a `Concept.Core`, la referencia a Concept ya introducía el espacio de solución en la elicitación.

La contaminación fue detectada antes de transportar la pregunta, por lo que no alteró la evidencia primaria de Anima.

## Problem or tension

Una frontier puede modificar la evidencia que pretende obtener si obliga a la autoridad de origen a razonar dentro de categorías que pertenecen al proveedor o a una solución todavía no justificada.

## Options considered

### Mantener proveedor y necesidad en una misma pregunta

Reduce pasos, pero mezcla discovery del problema con interpretación de solución.

### Separar consumer-facing y provider-side uncertainty

Preserva primero la necesidad en lenguaje del consumidor y permite traducirla después desde la responsabilidad del proveedor.

## Selected option

Separar ambas incertidumbres.

## Rationale

La evidencia primaria debe conservar la semántica y autoridad de su origen antes de someterla a mecanismos o vocabularios posteriores.

## Consequences

- Preguntas hacia consumidores deben minimizar contaminación por solución cuando el objetivo es descubrir necesidad, significado o fenómeno.
- La traducción hacia capacidades de Concept ocurre después y conserva procedencia.
- Esta decisión se aplica como criterio de trabajo; no constituye todavía una modificación generalizada del protocolo base más allá de esta evidencia.

## Protocol Execution

### Objective

Obtener necesidades de Anima sin forzarlas a expresarse en el vocabulario de Concept o VSlices.

### Previous state

La frontier inicial mezclaba necesidad del consumidor y capacidad del proveedor en una misma formulación.

### Next state

`Consumer-facing uncertainty` y `provider-side uncertainty` quedan separadas durante discovery.

## Review conditions

Revisar si otros casos muestran que esta separación no reduce sesgo o introduce costes que superen su utilidad.