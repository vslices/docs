# VSlices Design

VSlices Design helps teams decide how much domain understanding they need before turning business knowledge into software.

It provides design modalities, reasoning tools, and modeling heuristics.

It helps teams move from unclear business material toward clearer software decisions without losing continuity.

VSlices Design is intentionally independent from VSlices Framework. You do not need to use VSlices Framework to apply VSlices Design.

!!! principle "Design principle"

```
Understand the business material before building the software structure.

The right modality is not the most sophisticated one. It is the one that matches the uncertainty the team is actually facing.
```

## Purpose

Many software projects begin from artifacts that appear late in design reasoning:

* user stories
* screens
* APIs
* database tables
* technical components
* implementation tasks

These artifacts are useful, but they are not always the right starting point.

!!! risk "Risk to avoid"

```
When the domain is unclear, fragmented, manual, shaped by legacy, or organizationally complex, starting directly from implementation can create accidental complexity.
```

VSlices Design exists to reduce that risk.

Its purpose is to help teams choose how much understanding, context, planning, and feedback they need before moving forward.

## Relationship with the VSlices Suite

VSlices Design is a product within the VSlices Suite.

It connects with the other products, but remains independent.

| Product               | Relationship with VSlices Design                                                                               |
| --------------------- | -------------------------------------------------------------------------------------------------------------- |
| [VSlices Docs Standard](../docs-standard/index.md) | Provides documentation structures to preserve discovered intent.                                               |
| [VSlices Method](../design/index.md)        | Defines how to apply Design within an engineering workflow.                                                    |
| [VSlices Framework](../framework/index.md)     | May later reflect the resulting concepts as contexts, capabilities, features, flows, errors, and integrations. |

!!! principle "Continuity principle"

    Domain understanding should remain connected to documentation, architecture, and implementation.

    Implementation should remain traceable to the business intent that justified it.


## Core principle

!!! principle "Design principle"

    Choose the modality that responds to the team's real uncertainty.

What matters is not choosing the most sophisticated modality.

Sometimes it is better to:

* explore broadly
* focus on a specific problem
* learn from a small vertical slice
