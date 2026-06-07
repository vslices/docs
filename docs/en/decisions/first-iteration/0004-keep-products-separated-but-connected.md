# Keep Products Separated But Connected

## Status

Accepted.

## Context

VSlices is evolving as a software engineering suite composed of multiple products:

* VSlices Framework
* VSlices Design
* VSlices Docs Standard
* VSlices Method

Each product addresses a different part of the software lifecycle. The suite exists to preserve continuity between:

* domain discovery
* documentation
* design reasoning
* architecture
* implementation
* validation
* evolution

A risk appeared while defining the documentation structure: treating all products as if they were only sections of the framework.

That would make the suite easier to describe in the short term, but weaker in the long term. VSlices Framework is only one implementation-oriented product inside the suite.

VSlices Design, VSlices Docs Standard, and VSlices Method must be able to evolve independently from the framework.

## Decision

VSlices products will be documented and evolved as separate but connected products.

Each product must have:

* its own identity,
* its own responsibility,
* its own documentation section,
* its own evolution path,
* and its own validation criteria.

The products should remain connected through shared principles and traceable relationships, but no product should be reduced to a subsection of another product.

The suite will be organized as:

```text
VSlices Suite
  VSlices Framework
  VSlices Design
  VSlices Docs Standard
  VSlices Method
```

The shared connection between products is the continuity model.

The products are not independent because they are unrelated. They are independent because they solve different problems within the same lifecycle.

## Product Boundaries

VSlices Framework is responsible for implementation support.

It provides libraries, primitives, abstractions, adapters, conventions, and development patterns that help implement domain-oriented software with low ceremony and progressive architecture.

VSlices Design is responsible for design reasoning.

It provides modeling techniques, analysis strategies, domain discovery guidance, separation heuristics, and architectural reasoning tools.

VSlices Docs Standard is responsible for documentation structure.

It defines how domain knowledge, architectural decisions, use cases, capabilities, views, processes, expected errors, and invariants are preserved in living documentation.

VSlices Method is responsible for lifecycle continuity.

It explains how Design, Docs Standard, and Framework can work together across discovery, documentation, architecture, implementation, and evolution.

## Rationale

Keeping products separated prevents accidental product coupling.

If everything is treated as part of VSlices Framework, several problems appear:

* design techniques become dependent on framework usage,
* documentation standards become implementation-specific,
* the method becomes hidden behind code examples,
* non-developer users are excluded,
* and the suite becomes harder to explain honestly.

> VSlices Design should be useful even when a team does not use VSlices Framework.
> VSlices Docs Standard should be useful even when the implementation is not written in .NET.
> VSlices Method should guide continuity even before any code exists.
> VSlices Framework should remain an implementation accelerator, not the owner of the entire suite.

At the same time, separating products too much would create another problem: fragmentation.

The products should not drift into unrelated tools.

They must remain connected through shared vocabulary, shared principles, and traceable lifecycle relationships.

## Consequences

This decision gives each product room to mature independently. It also makes documentation clearer because each section can focus on one responsibility.

The tradeoff is that some concepts may appear in more than one product. When this happens, each product should explain the concept from its own perspective. For example:

* VSlices Design may explain a capability as a modeling concept.
* VSlices Docs Standard may explain how to document a capability.
* VSlices Framework may explain how to implement a capability.
* VSlices Method may explain when and why the capability moves across the lifecycle.

This repetition is acceptable when it preserves perspective.

It becomes a problem only when documents duplicate the same explanation without adding product-specific value.

## Documentation Rule

Product documentation should avoid mixing responsibilities.

An index page should explain the purpose and scope of the product.

It should not attempt to explain the entire suite.

Detailed cross-product relationships should live in method-oriented or suite-oriented documentation.

Each product page should answer:

* What is this product responsible for?
* Who is it for?
* What problem does it solve?
* What does it intentionally not solve?
* How does it connect with the rest of VSlices?

## Validation Rule

A product should not absorb responsibilities from another product only because it is convenient.

Before moving a concept into a product, ask:

* Does this responsibility belong here?
* Is this concept implementation-specific?
* Is this concept documentation-specific?
* Is this concept design-specific?
* Is this concept lifecycle-specific?
* Would this still make sense if the framework did not exist?

If the concept still makes sense without the framework, it probably belongs to Design, Docs Standard, or Method before it belongs to Framework.

## Accepted Tradeoff

VSlices accepts slightly more documentation structure in exchange for clearer product boundaries.

The suite should feel connected, but not collapsed into a single product.  This avoids premature coupling and keeps future evolution open.

## Principle

Products should be separated by responsibility. Products should be connected by continuity.

VSlices is a suite because the lifecycle is connected. VSlices is not a single product because each lifecycle problem deserves its own shape.
 