```md
# Built-in components

VSlices Framework provides a set of built-in components intended to support domain-oriented software development with explicit behavior and progressive architecture.

These components are not meant to act as a rigid platform or a closed ecosystem.

Their purpose is to provide reusable primitives and structural foundations for modeling, composing, and executing software behavior.

## The role of built-in components

The Framework includes built-in components because some engineering problems appear repeatedly across many systems.

Examples include:

- representing execution flows
- modeling expected failures
- preserving domain invariants
- describing runtime requirements
- composing behavior safely
- expressing reusable capabilities
- structuring application behavior
- and preserving domain intent during implementation

The built-in components attempt to make these concerns more explicit and composable.

## Design philosophy

The built-in components follow the same foundational ideas as the rest of the Framework:

- composition over inheritance
- explicit behavior
- explicit expected errors
- immutable-first modeling
- low ceremony
- progressive complexity
- compile-time safety whenever possible

The goal is not to hide complexity behind abstractions.

The goal is to expose important behavior in a more understandable and evolvable way.

## Current areas

The current built-in components are organized into two main areas:

### For domain

Components focused on domain modeling and domain structure.

This area currently explores concepts such as:

- algebraic types
- domain types
- capabilities
- domain-oriented composition

These components aim to help preserve domain intent and invariants during modeling and implementation.

### For application

Components focused on application behavior and execution flow.

This area currently explores concepts such as:

- features
- execution flows
- runtime requirements
- application capabilities
- compositional execution

These components aim to make application behavior more explicit and easier to reason about.

## Relationship with design patterns

The built-in components are strongly connected to the Framework design patterns.

Patterns such as:

- errors as values
- traits
- capabilities
- compositional design

directly influence how many built-in components are modeled and composed.

The components should be understood as practical implementations of those ideas, not as isolated utilities.

## Current state

This section is still evolving.

Some built-in components already exist in the current implementation direction, while others are still exploratory and being validated through real software design and implementation work.

The current validation work happens primarily through the Alive Lab and Domus Orbis.
```
