# VSlices

**VSlices** is a progressive software engineering suite focused on preserving continuity between domain discovery, documentation, design reasoning, architecture, implementation, and system evolution.

It is composed of:

* **VSlices Framework**, for implementation support.
* **VSlices Design**, for design reasoning and modeling techniques.
* **VSlices Docs Standard**, for living documentation structures.
* **VSlices Method**, for connecting discovery, documentation, design, architecture, and implementation.

VSlices exists to reduce accidental complexity and preserve architectural intent as a system evolves.

## Current maturity

VSlices is currently in a __beta prerelease__ stage.

This documentation is being shared early to validate whether the suite communicates its ideas clearly, preserves conceptual continuity across its products, and helps people reason about software engineering without adding unnecessary ceremony.

The current version should be read as a foundational snapshot, not as a final product specification.

| Area | Current maturity | What to expect |
| --- | --- | --- |
| VSlices Design | Beta prerelease | The main design ideas, principles, and modeling<br/>modalities are available for early feedback.<br/><br/>Some techniques may still evolve as they are validated<br/>in real projects. |
| VSlices Docs Standard | Beta prerelease | The documentation model, document types, and<br/>continuity principles are available for early feedback.<br/><br/>Templates and examples may become more concrete<br/>over time. |
| VSlices Method | Beta prerelease | The method currently connects design reasoning,<br/>documentation, and implementation intent.<br/><br/>Its collaboration and continuity models are available for<br/>review and refinement. |
| VSlices Framework | Experimental | Framework documentation is intentionally limited<br/>while the concepts from Design, Docs Standard, and<br/>Method are reviewed together.<br/><br/>Its implementation model may change as alignment<br/>improves. |
| Alive Lab | Exploratory | Field notes, project stories, theories, and decisions<br/>preserve learning in progress.<br/><br/>These materials may influence VSlices, but they are not<br/>all official product guidance. |

The goal of this prerelease is not to present VSlices as complete. It is to make the current thinking visible, receive feedback, and improve the suite before expanding the Framework documentation and translating the full documentation into Spanish.

## Start here

If you are new to VSlices, start with these pages:

* [How to start?](start-here/index.md)
* [What is VSlices?](start-here/what-is-vslices.md)
* [Why VSlices exists?](start-here/why-vslices-exists.md)
* [Suite overview](start-here/suite-overview.md)
* [Adoption paths - WIP](start-here/adoption-paths.md)

If you only want to understand the core idea, start with [What is VSlices?](start-here/what-is-vslices.md).

If you want to understand why VSlices exists, read [Why VSlices exists](start-here/why-vslices-exists.md).

If you want to understand how the products relate to each other, read [Suite overview](start-here/suite-overview.md).

## Products

VSlices is documented as a suite of connected products:

* [VSlices Framework](products/framework/index.md) explains the implementation-oriented foundations.
* [VSlices Design](products/design/index.md) explains how we reason about software design.
* [VSlices Docs Standard](products/docs-standard/index.md) explains how we preserve knowledge through documentation.
* [VSlices Method](products/method/index.md) explains how the products connect across the software lifecycle.

Each product can evolve independently, but all of them share the same goal: preserving continuity between understanding, documenting, designing, building, and evolving software.

## Validation

VSlices is being defined and validated through real software design and implementation work.

The [Alive Lab](alive-lab/index.md) preserves theories, project stories, modeling discoveries, and field observations that shape VSlices over time.

## Decisions

Important methodology, product, and documentation decisions are recorded in the [Decisions section](decisions/index.md). These records preserve:

* why a decision was made
* which tradeoffs were accepted
* what remains uncertain
* how VSlices evolves from real design pressure

## Current state

VSlices is currently in an early foundational stage.

The documentation represents the first public structure of the suite, not a finished methodology or complete framework ecosystem.

Some ideas are stable enough to document as part of v0.1. Other ideas remain experimental and are intentionally kept inside the Alive Lab until they are validated further.
