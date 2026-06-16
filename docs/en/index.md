<div class="vslices-hero">
  <img
    src="https://raw.githubusercontent.com/vslices/icons/refs/heads/main/official/icon.svg"
    alt="VSlices icon"
    class="vslices-hero__icon"
  />

  <div class="vslices-hero__content">
    <h1>VSlices</h1>
    <p>
      A progressive software engineering suite for preserving continuity between
      domain discovery, documentation, design, architecture, implementation,
      validation, and system evolution.
    </p>
  </div>
</div>

VSlices is composed of four connected products:

<div class="grid cards" markdown>

-   **[VSlices Method](products/method/index.md)**

    A continuity method that connects discovery, documentation, design, architecture, implementation, validation, and evolution.

-   **[VSlices Design](products/design/index.md)**

    Design reasoning and modeling techniques for understanding the domain before implementation.

-   **[VSlices Docs Standard](products/docs-standard/index.md)**

    Living documentation structures for preserving system intent as software evolves.

-   **[VSlices Framework](products/framework/index.md)**

    Implementation support for domain-oriented software with low ceremony and progressive architecture.

</div>

## Current maturity

VSlices is currently in a **beta prerelease** stage.

This documentation is being shared early to validate whether the suite communicates its ideas clearly, preserves conceptual continuity across its products, and helps people reason about software engineering without adding unnecessary ceremony.

The current version should be read as a foundational snapshot, not as a final product specification.

| Area | Current maturity | What to expect |
| --- | --- | --- |
| [VSlices Design](./products/design/index.md) | Beta prerelease | The main design ideas, principles, and modeling modalities are available for early feedback.<br/><br/>Some techniques may still evolve as they are validated in real projects. |
| [VSlices Docs Standard](./products/docs-standard/index.md) | Beta prerelease | The documentation model, document types, and continuity principles are available for early feedback.<br/><br/>Templates and examples may become more concrete over time. |
| [VSlices Method](./products/method/index.md) | Beta prerelease | The method currently connects design reasoning, documentation, and implementation intent.<br/><br/>Its collaboration and continuity models are available for review and refinement. |
| [VSlices Framework](./products/framework/index.md) | Experimental | Framework documentation is intentionally limited while the concepts from Design, Docs Standard, and Method are reviewed together.<br/><br/>Its implementation model may change as alignment improves. |
| [Alive Lab](./alive-lab/index.md) | Exploratory | Field notes, project stories, theories, and decisions preserve learning in progress.<br/><br/>These materials may influence VSlices, but they are not all official product guidance. |

The goal of this prerelease is not to present VSlices as complete. It is to make the current thinking visible, receive feedback, and improve the suite before expanding the Framework documentation and translating the full documentation into Spanish.

## Start here

If you are new to VSlices, use this reading path depending on what you need to understand:

| If you want to... | Start with... |
| --- | --- |
| Understand the core idea | [What is VSlices?](start-here/what-is-vslices.md) |
| Understand why VSlices exists | [Why VSlices exists](start-here/why-vslices-exists.md) |
| Understand how the products relate to each other | [Suite overview](start-here/suite-overview.md) |
| Explore possible adoption paths | [Adoption paths - WIP](start-here/adoption-paths.md) |

You can also begin from the general [How to start?](start-here/index.md) page.

## Products

VSlices products can evolve independently, but they are meant to preserve the same continuity from different angles:

| Product | Focus |
| --- | --- |
| [VSlices Method](products/method/index.md) | Connects discovery, documentation, design, architecture, implementation, validation, and evolution. |
| [VSlices Design](products/design/index.md) | Helps reason about the domain and shape the system before implementation. |
| [VSlices Docs Standard](products/docs-standard/index.md) | Preserves system intent through living documentation structures. |
| [VSlices Framework](products/framework/index.md) | Supports implementation through .NET libraries, primitives, and development patterns. |

Together, they help keep understanding, documentation, design, implementation, validation, and evolution aligned as the system grows.

## Validation

VSlices is being defined and validated through real software design and implementation work.

The [Alive Lab](alive-lab/index.md) preserves theories, project stories, modeling discoveries, and field observations that shape VSlices over time.

Alive Lab content should be read as learning in progress. Some ideas may later become official product guidance, while others may remain exploratory.

## Decisions

Important methodology, product, and documentation decisions are recorded in the [Decisions section](decisions/index.md). These records preserve:

* why a decision was made
* which tradeoffs were accepted
* what remains uncertain
* how VSlices evolves from real design pressure

## Current state

VSlices is currently in an early foundational stage.

The documentation represents the first public structure of the suite, not a finished methodology or complete framework ecosystem.

Some ideas are stable enough to document as part of v0.1. Other ideas remain experimental and are intentionally kept inside the [Alive Lab](alive-lab/index.md) until they are validated further.
