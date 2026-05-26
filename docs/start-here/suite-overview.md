# Suite overview

VSlices is composed of four connected products:

- **VSlices Method**
- **VSlices Design**
- **VSlices Docs Standard**
- **VSlices Framework**

Each product can be used independently, but they are designed to work together as part of the same continuity model.

The purpose of the suite is to reduce the distance between what a team discovers, documents, designs, implements, and evolves.

## The continuity model

VSlices is organized around a simple idea:

> Domain understanding should remain visible across documentation, architecture, and code.

The suite attempts to preserve continuity between:

- discovery
- design
- documentation
- architecture
- implementation
- evolution

The four products support different parts of that continuity.

## VSlices Method

**VSlices Method** is the overarching engineering method.

It defines how the other products are meant to work together across the software lifecycle. Its role is to help teams preserve continuity between:

- what they discover
- what they decide
- what they document
- what they design
- what they implement
- what they evolve

Method is not meant to be a rigid process. It should provide guidance for making engineering work more coherent without forcing every team to follow the same workflow.

## VSlices Design

**VSlices Design** is the product focused on software design and domain understanding. It provides concepts, techniques, and language for reasoning about:

- business processes
- service capabilities
- domain boundaries
- use cases
- problems
- slices
- system responsibilities

Design is intentionally independent from Framework.

A team should be able to use VSlices Design even if they never use VSlices Framework. Its purpose is to help teams understand what they are building before deciding how to implement it.

## VSlices Docs Standard

**VSlices Docs Standard** is the product focused on documentation structure.

It defines how to document important software concepts in a way that remains connected to design and implementation. It may include documents for:

- contexts
- use cases
- capabilities
- decisions
- processes
- views
- invariants
- expected errors

Docs Standard exists because documentation should not be a disconnected artifact. Its purpose is to preserve system intent and make important reasoning easier to find, review, and evolve.

## VSlices Framework

**VSlices Framework** is the .NET implementation product.

It provides libraries, primitives, patterns, and eventually batteries for building domain-oriented software with low ceremony and progressive architecture. The Framework currently focuses on concepts such as:

- flows
- features
- explicit errors
- runtime requirements
- domain types
- traits
- capabilities
- functional composition

The Framework is not meant to hide engineering concepts. It is meant to make useful patterns easier to compose, standardize, and evolve.

## How they work together

The products are connected, but they do not depend on each other in the same way. A simplified flow looks like this:

```txt
Method
  guides how we move through the lifecycle

Design
  helps us understand and model the domain

Docs Standard
  preserves the intent and structure of that understanding

Framework
  helps implement that intent in executable software
```

Another way to visualize it:

```txt
Discovery -> Design -> Documentation -> Implementation -> Evolution
     |          |             |                 |             |
   Method     Design     Docs Standard      Framework      Method
```

> This does not mean every project must follow a strict sequence.

In practice, teams may move back and forth between these activities. VSlices only tries to make those movements explicit and easier to preserve.

## Independent adoption

Each product can be adopted independently. A team may use:

* **Design** to improve modeling and discovery work
* **Docs Standard** to improve documentation structure
* **Framework** to build .NET applications with VSlices primitives
* **Method** to guide how the pieces fit together

Adopting VSlices does not require adopting the entire suite at once. The suite is intended to be progressive and composable.

## Current state

VSlices is still being defined and validated.

Some products are more concrete than others.

The Framework already has foundational abstractions and implementation direction.

Design, Docs Standard, and Method are being formalized through real work, especially through the Alive Lab and Domus Orbis.

This overview describes the intended shape of the suite, not a claim that every part is complete.
