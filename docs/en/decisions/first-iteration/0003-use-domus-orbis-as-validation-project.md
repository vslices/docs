# Use Domus Orbis As Validation Project

## Status

Accepted.

## Context

VSlices is evolving as a software engineering suite composed of:

* VSlices Framework
* VSlices Design
* VSlices Docs Standard
* VSlices Method

The suite aims to preserve continuity between:

* domain discovery
* documentation
* design reasoning
* architecture
* implementation
* validation
* evolution

Because VSlices is still in an early foundational stage, there is a high risk of designing abstractions that are theoretically elegant but not validated against real software work.

This risk is especially important because VSlices is not intended to become a collection of interesting abstractions.

VSlices should grow from recurring problems observed in real systems. Domus Orbis is currently the main real project available for validating VSlices ideas.

It contains enough product, domain, documentation, architecture, and implementation complexity to reveal whether VSlices concepts are useful in practice.

## Decision

Domus Orbis will be used as the primary validation project for VSlices during the v0.1 stage.

New VSlices concepts, abstractions, documentation structures, design techniques, and method guidance should be tested against Domus Orbis before being treated as stable parts of the suite.

This applies especially to:

* domain modeling patterns
* feature organization
* capability modeling
* documentation structures
* design modalities
* method workflows
* architectural boundaries
* implementation primitives
* cross-product traceability

A VSlices idea should not become official only because it is elegant. It should become official when it survives contact with real project needs.

## Rationale

Domus Orbis provides a concrete environment where VSlices can be tested across the lifecycle. It can validate whether VSlices helps preserve continuity between:

* understanding the domain
* documenting the system
* reasoning about design
* defining architecture
* implementing behavior
* evolving the system over time

This matters because VSlices is not only a framework.

If validation happens only through code examples, then VSlices Framework may evolve, but VSlices Design, VSlices Docs Standard, and VSlices Method may remain untested.

Domus Orbis allows the suite to be validated as a connected lifecycle, not only as an implementation library.

## Validation Role

Domus Orbis should be used to answer questions such as:

* Does this abstraction reduce accidental complexity?
* Does this document preserve useful knowledge?
* Does this design technique help clarify the domain?
* Does this method step help move from discovery to implementation?
* Does this pattern remain understandable after some time?
* Does this structure help future evolution?
* Does this idea still work when the domain becomes messy?
* Does this create more ceremony than value?

If Domus Orbis exposes friction, the friction should be treated as design feedback.

The goal is not to force Domus Orbis to fit VSlices. The goal is to let Domus Orbis reveal where VSlices is useful, incomplete, unclear, or overdesigned.

## Consequences

This decision gives VSlices a concrete validation path. It reduces the risk of premature abstraction.

It also creates a healthy constraint: not every interesting idea should be promoted into the suite immediately.

Some ideas may remain as:

* experiments
* field notes
* alive lab entries
* local patterns
* future possibilities

This is acceptable. VSlices should prefer validated usefulness over theoretical completeness.

## Scope Limit

Domus Orbis is the primary validation project, not the only possible future validation project.

A pattern validated in Domus Orbis should still be treated carefully before being generalized.

Some Domus Orbis needs may be specific to that project.

Some VSlices ideas may require validation in other domains before becoming stable recommendations.

Domus Orbis validates that an idea can work in one real project.

It does not automatically prove that the idea is universal.

## Documentation Rule

When a VSlices idea is validated through Domus Orbis, the documentation should preserve:

* what problem appeared
* what solution was tried
* what tradeoff was accepted
* what changed in the design
* what changed in the implementation
* and what remains uncertain

This keeps validation visible and prevents the suite from pretending that decisions appeared fully formed.

## Accepted Tradeoff

Using Domus Orbis as the primary validation project may bias early VSlices decisions toward the needs of one system.

This tradeoff is accepted because validating against one real project is better than validating against none.

The risk will be reduced later by testing VSlices in additional projects, domains, and collaboration contexts.

## Principle

VSlices should not be designed only from theory.

VSlices should be shaped by real project pressure.

Domus Orbis exists as the first place where VSlices ideas must prove that they help.
