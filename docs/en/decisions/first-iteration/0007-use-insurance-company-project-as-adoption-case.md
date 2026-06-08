# Use Existing Insurance Company Project As Adoption Case

## Status

Accepted.

## Context

VSlices is being developed as a suite composed of:

* VSlices Method
* VSlices Design
* VSlices Docs Standard
* VSlices Framework

Domus Orbis is currently the primary validation project for validating VSlices ideas in a project where we can shape the process, documentation, architecture, and implementation with high control.

However, this does not cover another important scenario:

> Joining an existing project that was not created using VSlices Method, but where there is openness to apply some VSlices practices progressively.

The current work context inside an insurance company provides this scenario. The project already exists.

Its current documentation, architecture, development practices, domain understanding, and team habits were not created using VSlices.

This makes it a valuable adoption case for VSlices Method, VSlices Design, and VSlices Docs Standard.

## Decision

The insurance company project context will be used as an adoption case for validating how VSlices can be introduced into an existing project. This case will focus on:

* understanding an existing domain
* documenting knowledge progressively
* identifying missing context
* preserving discovered intent
* improving continuity between conversations and documentation
* applying design reasoning without forcing framework adoption
* validating whether VSlices Method can help in a project that did not start with VSlices

This case is not intended to validate VSlices Framework first. The primary validation target is:

```text
VSlices Method
VSlices Design
VSlices Docs Standard
```

VSlices Framework may be referenced only when implementation patterns become relevant.

## Rationale

Most real teams do not start from a blank canvas. Many useful engineering methods must work in projects that already have existing:

* code
* architecture
* documentation gaps
* delivery pressure
* team habits
* business language
* accidental complexity

If VSlices only works when applied from the beginning, its practical value would be limited. This adoption case helps validate whether VSlices can provide value incrementally. The key question is:

> Can VSlices help recover continuity in a project where continuity was not intentionally preserved from the start?

## Scope

This adoption case should validate lightweight use of VSlices practices. The focus should be on activities such as:

* creating context documents from existing knowledge
* extracting vocabulary from conversations and systems
* documenting discovered capabilities
* identifying unclear boundaries
* recording decisions
* mapping current processes
* separating domain concepts from implementation details
* using VSlices Design modalities to reason about the existing system

The work should avoid introducing unnecessary ceremony.

The goal is not to convert the project into a VSlices project. It is to observe where VSlices helps.

## Non-goals

This decision does not mean:

* forcing VSlices Framework into the insurance company project
* requiring the team to adopt all VSlices products
* rewriting existing documentation
* replacing existing architecture
* imposing VSlices terminology too early
* or treating the project as a controlled laboratory

This is an adoption case, not a migration project.

## Validation Questions

This case should help answer:

* Can VSlices Method be useful when introduced late?
* Which documents provide value first in an existing project?
* Which VSlices Design techniques help understand legacy or inherited context?
* How much documentation is useful before it becomes ceremony?
* Can VSlices Docs Standard help recover missing intent?
* Can VSlices terminology coexist with existing team language?
* What should be introduced first when a team has limited context?
* Which practices are too heavy for early adoption?

## Expected Outputs

Useful outputs may include:

* context documents
* vocabulary notes
* capability documents
* process notes
* decision records
* boundary observations
* field notes
* adoption lessons

These outputs should be small and practical. They should preserve knowledge that would otherwise remain scattered across meetings, conversations, tickets, code, or personal memory.

## Accepted Tradeoff

This case may not allow full validation of VSlices because the project context is external and already constrained. Some limitations may include:

* limited influence over architecture
* limited access to historical decisions
* existing organizational constraints
* incomplete domain visibility
* delivery pressure

This tradeoff is accepted because these constraints are exactly what make the case useful. Real adoption rarely happens in ideal conditions.

## Relationship With Domus Orbis

Domus Orbis remains the primary validation project for building and refining VSlices under high control.

The insurance company project becomes a complementary validation case for progressive adoption.

```text
Domus Orbis
  validates VSlices as a designed lifecycle.

Insurance company project
  validates VSlices as an adoption aid in an existing lifecycle.
```

Both cases are useful, but they answer different questions.

## Principle

VSlices should not only help when a project starts correctly.

VSlices should also help recover clarity when a project already exists.

Progressive adoption is part of progressive architecture.
