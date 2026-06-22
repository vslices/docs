# VSlices Docs Standard

VSlices Docs Standard defines reusable documentation structures for preserving knowledge throughout the lifecycle of a software system.

It does not exist to make teams produce more documents.

It exists to help teams preserve the knowledge that software decisions depend on.

!!! principle "Documentation principle"

    Document to preserve useful knowledge, not to complete a document checklist.


## Purpose

VSlices Docs Standard helps teams keep domain understanding, design reasoning, documentation, decisions, implementation, validation, and evolution connected.

Its purpose is to reduce knowledge loss between what the team understands, decides, documents, builds, validates, and changes.

## Core idea

Documentation should exist when it preserves knowledge needed for present or future decisions.

A document should not be created because it belongs to the standard.

It should be created because it helps keep an important part of the system's context, intent, behavior, decision, validation, or evolution visible.

## What it provides

VSlices Docs Standard provides:

* **principles**: ideas that guide how documentation should be used
* **document modeling**: rules for understanding notes, documents, references, states, and relationships
* **taxonomy**: grouping documents according to the type of knowledge they preserve
* **continuity paths**: ways to understand how knowledge moves between documents, decisions, implementation, and learning
* **anti-bureaucracy rules**: criteria for avoiding turning documentation into ceremony
* **document structures**: reusable formats for common types of engineering knowledge

The standard is intentionally progressive. A team should use the smallest useful structure that preserves the knowledge future work depends on.

## How to use it

Start from the knowledge you need to preserve.

| If you need to preserve...                                                        | Use...                                                       |
| --------------------------------------------------------------------------------- | ------------------------------------------------------------ |
| Early, uncertain, local, or temporary knowledge                                   | **[Support Note](./taxonomy/support-note.md)**               |
| Language that may affect understanding, behavior, naming, or boundaries           | **[Domain Vocabulary](./taxonomy/domain-vocabulary.md)**     |
| Where the work happens                                                            | **[Context Document](./taxonomy/context-document.md)**       |
| Responsibilities, coordination, workflows, or operational rules                   | **[Process Document](./taxonomy/process-document.md)**       |
| The explicit meaning of a behavior, consequences, validations, or expected errors | **[Use Case Document](./taxonomy/use-case-document.md)**     |
| A stable capability that several behaviors or processes depend on                 | **[Capability Document](./taxonomy/capability-document.md)** |
| A choice with significant tradeoffs, consequences, or future impact               | **[Decision Record](./taxonomy/decision-record.md)**         |
| Evidence that changes or confirms knowledge future work will depend on            | **[Validation Note](./taxonomy/validation-note.md)**         |

!!! risk "Risk to avoid"

    Do not create a document because the standard contains it. Create it because it preserves useful knowledge for present or future decisions.


## What it is not

VSlices Docs Standard is not a complete methodology.

* It does not define the full workflow for executing an iteration
* It does not require every document to be created
* It does not define meetings, roles, stage controls, or delivery rituals

Those concerns belong to VSlices Method.

Docs Standard defines the instruments. Method defines how those instruments are used during real work.

## Relationship with the VSlices Suite

VSlices Docs Standard is one of the products within the VSlices Suite.

| Product                                        | Relationship with VSlices Docs Standard                            |
| ---------------------------------------------- | ------------------------------------------------------------------ |
| **[VSlices Design](../design/index.md)**       | Defines how teams reason about design.                             |
| **[VSlices Method](../method/index.md)**       | Defines how teams apply design and documentation during real work. |
| **[VSlices Framework](../framework/index.md)** | May reflect that knowledge in implementation.                      |

Docs Standard is independent from VSlices Framework. A team can use these documents with any technology, architecture, language, or delivery process.
