# What is VSlices?

**VSlices** is a progressive software engineering suite focused on preserving continuity between domain discovery, documentation, architecture, implementation, and system evolution.

It helps teams keep software structurally close to the domain it represents.

VSlices is not only a framework for organizing code. It is composed of four connected products:

- **VSlices Method**
- **VSlices Design**
- **VSlices Docs Standard**
- **VSlices Framework**

Each product can be used independently, but they are designed to work together.

## Core idea

Software systems often drift away from the domain they represent, and this drift usually appears when discovery, documentation, architecture, and implementation evolve as separate activities.

VSlices proposes a different direction:

> The same domain language, structural boundaries, and behavioral intent should remain visible across documentation, architecture, and code.

The goal is not to make every project follow the same architecture, **but to preserve continuity**.

## What VSlices promotes

VSlices promotes:

- domain-driven design
- vertical slices
- strong domain modeling
- explicit behaviors
- explicit expected errors
- composable capabilities
- progressive architecture
- low ceremony

VSlices does not require teams to start with a large architectural blueprint. Instead, it encourages teams to introduce structure when the domain makes that structure necessary.

## What VSlices is not

VSlices does not enforce:

- CQRS,
- Event Sourcing,
- Clean Architecture,
- microservices,
- or a specific infrastructure style.

It is also not intended to be:

- low-code tooling,
- automatic software generation,
- or architecture enforcement software.

VSlices should support engineering decisions, not replace them.

## The four products

### VSlices Method

The method connects the whole lifecycle: discovery, documentation, architecture, implementation, and evolution, defining how the other products are meant to work together.

### VSlices Design

Design focuses on modeling and architectural reasoning before implementation, providing concepts, techniques, and language for understanding the domain and shaping the system.

### VSlices Docs Standard

Docs Standard defines documentation structures that preserve system intent. The goal is to make documentation part of design, not a disconnected artifact.

### VSlices Framework

Framework provides .NET libraries, primitives, and development patterns for implementing domain-oriented software with low ceremony and progressive architecture.

