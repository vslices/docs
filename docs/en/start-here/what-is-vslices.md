# What is VSlices?

**VSlices** is a progressive software engineering suite focused on preserving continuity between domain discovery, documentation, design reasoning, architecture, implementation, validation, and system evolution.

It helps teams keep software structurally close to the domain it represents.

VSlices is not only a framework for organizing code. It is composed of four connected products:

- **[VSlices Method](../products/method/index.md)**: connects discovery, documentation, design, architecture, implementation, validation, and evolution.
- **[VSlices Design](../products/design/index.md)**: provides design reasoning and modeling techniques.
- **[VSlices Docs Standard](../products/docs-standard/index.md)**: defines living documentation structures.
- **[VSlices Framework](../products/framework/index.md)**: offers implementation support.

Each product can be used independently, but they are designed to work together.

## Core idea

Software systems often drift away from the domain they represent.

This drift usually appears when discovery, documentation, architecture, and implementation evolve as separate activities.

!!! principle "Principle · Continuity"

    The same domain language, structural boundaries, and behavioral intent should remain visible across documentation, architecture, and code.

The goal is not to make every project follow the same architecture, **but to preserve continuity**.

## What VSlices promotes

VSlices promotes practices that keep domain intent visible as the system grows:

| Area | What VSlices emphasizes |
| --- | --- |
| Domain understanding | domain-driven design and strong domain modeling |
| System structure | vertical slices, composable capabilities, and progressive architecture |
| Behavior clarity | explicit behaviors and explicit expected errors |
| Adoption style | low ceremony and structure introduced only when the domain needs it |

VSlices does not require teams to start with a large architectural blueprint. Instead, it encourages teams to introduce structure when the domain makes that structure necessary.

## What VSlices is not

VSlices does not impose a specific architecture or replace engineering judgment.

| VSlices does not enforce... | What this means |
| --- | --- |
| CQRS | Teams may use it when the domain or complexity justifies it, but VSlices does not require it. |
| Event Sourcing | Event history is not assumed as the default persistence or modeling strategy. |
| Clean Architecture | Layering decisions should emerge from the needs of the system, not from a mandatory template. |
| microservices | Deployment and service boundaries are architectural decisions, not VSlices defaults. |
| a specific infrastructure style | Infrastructure choices should support the domain instead of defining the architecture upfront. |

VSlices is also not:

* low-code tooling
* automatic software generation
* architecture enforcement software

VSlices should support engineering decisions, not replace them.

## The four products

VSlices is composed of four products that preserve continuity from different angles:

| Product | Focus |
| --- | --- |
| [VSlices Method](../products/method/index.md) | Connects discovery, documentation, design, architecture, implementation, validation, and evolution across the software lifecycle. |
| [VSlices Design](../products/design/index.md) | Provides concepts, techniques, and language for reasoning about the domain and shaping the system before implementation. |
| [VSlices Docs Standard](../products/docs-standard/index.md) | Defines living documentation structures that preserve system intent and keep documentation connected to design. |
| [VSlices Framework](../products/framework/index.md) | Provides .NET libraries, primitives, and development patterns for implementing domain-oriented software with low ceremony and progressive architecture. |

!!! experimental "Experimental"

    VSlices Framework is currently experimental, and its public documentation is intentionally limited during v0.1-beta.
