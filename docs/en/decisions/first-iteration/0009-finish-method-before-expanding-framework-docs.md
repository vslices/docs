# Finish Method before expanding Framework documentation

## Status

Accepted

## Context

VSlices v0.1-beta is currently focused on consolidating the conceptual foundation of the suite.

The most relevant pending work is to complete and stabilize:

* VSlices Method
* VSlices Design
* VSlices Docs Standard

These products define the language, structure and continuity model that later guide Framework documentation and implementation examples.

At the same time, VSlices Framework still needs more complete documentation. However, documenting Framework too early may create instability if Method, Design and Docs Standard are still changing.

Framework documentation should be derived from a clearer engineering model, not written independently from it.

## Decision

We will finish the v0.1-beta foundation for Method, Design and Docs Standard before expanding Framework documentation in depth.

Framework documentation may continue progressing in parallel only when it is directly supported by stable concepts already defined by the other products. The immediate priority is:

* complete Method
* align Design with Method
* align Docs Standard with Method and Design
* use the resulting structure to guide Framework documentation

## Rationale

Framework is the implementation-facing product of VSlices, but it should not define the suite alone.

VSlices is intended to preserve continuity between:

* discovery
* documentation
* design reasoning
* architecture
* implementation
* evolution

Because of that, Framework documentation should explain not only APIs or abstractions, but also the reasoning that makes those abstractions useful.

- Completing Method first gives Framework documentation a clearer base.
- Completing Design first gives Framework documentation better modeling language.
- Completing Docs Standard first gives Framework documentation better continuity with living documentation.

## Consequences

### Positive consequences

* Framework documentation will be more coherent with the rest of the suite.
* VSlices v0.1-beta will have a stronger conceptual foundation.
* Documentation work will avoid duplicating or contradicting unfinished Method ideas.
* Future Framework examples can reference Method, Design and Docs Standard consistently.
* Adoption paths can emerge from validated scenarios instead of being invented too early.

### Negative consequences

* Framework documentation will remain incomplete for a little longer.
* Some implementation concepts may need to wait for clearer Method language.
* Users looking only for Framework usage may not have complete guidance immediately.

### Tradeoff

We accept slower Framework documentation in the short term to preserve stronger suite coherence in the medium term.

## Validation Strategy

This decision will be validated through the next Alive Lab projects:

* Slice-First documentation generator
* Problem-First analysis without Framework
* Context-First Surreal Knowledge Manager / Surreal Atlas exploration
* Problem-First development using Framework in Domus Orbis

Each project should provide feedback into:

* Method
* Design
* Docs Standard
* Framework documentation
* future Adoption Paths

## Notes

This decision does not block all Framework work.

It only prevents Framework documentation from becoming the primary driver before the conceptual foundation of v0.1-beta is stable.

Framework documentation should continue when it helps explain or validate already defined concepts.
