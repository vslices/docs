# Document Modeling

VSlices Docs Standard treats documents as evolving structures that preserve useful knowledge.

A document is not only a file, it is a named container for knowledge that may support future understanding, decisions, implementation, validation, or evolution.

The goal of document modeling is to make documentation explicit enough to preserve continuity without turning it into bureaucracy.

## Documents and notes

VSlices Docs Standard distinguishes between documents and notes.

A **document** has a stable purpose, a recognizable structure, and a clear role inside the documentation system. Examples:

- Domain Vocabulary
- Context Document
- Process Document
- Use Case Document
- Capability Document
- Decision Record
- Validation Note

A __note__ is lighter. It captures useful knowledge before the team knows whether that knowledge deserves a formal document. Examples:

- concept note
- assumption note
- risk note
- open question
- feedback note
- implementation note
- scope note

The rule is simple:

> Everything can start as a note. Only knowledge that proves useful should gain more structure.

## Progressive structure

Documents should grow progressively.

A team should not start with the largest possible version of a document. Each document type should support at least two levels:

- __minimal version__: captures the smallest useful structure
- __expanded version__: when complexity, risk, ambiguity, team size, or system lifetime requires more detail.

A document should become larger because the domain requires it, not because the template allows it.

## Document lifecycle

A document may evolve through different states. Suggested states and meanings are:

- __draft__: still being shaped
- __active__:  currently represents useful shared knowledge
- __superseded__: has been replaced by newer knowledge
- __archived__: is no longer active, but may remain useful as historical context

A document should not be treated as permanent just because it exists. When the system changes, documentation may need to change with it.

## Document identity

Documents should be easy to reference. A document may have a stable identifier when it needs to be connected with other documents. Example:

- _context_._order-fulfillment_
- _process_._order-submission_
- _use-case_._create-reservation_
- _capability_._validate-payment_
- _decision_._order-validation-boundary_
- _validation_._payment-rules-feedback_

The identifier does not need to be complex. It only needs to help readers understand what the document refers to and how it connects with other knowledge.

## Document relationships

Documents should not live as isolated files. They may relate to each other through simple relationships, common relationships include:

- supports
- refines
- depends-on
- validates
- challenges
- supersedes

Examples:

- A Use Case Document refines a Context Document.
- A Capability Document supports several Use Case Documents.
- A Decision Record depends on a Risk Note.
- A Validation Note validates or challenges an Assumption Note.
- A newer Decision Record supersedes an older Decision Record.

## Granularity

A document should preserve one coherent piece of knowledge.

- If a document tries to explain too many things, it may need to be split.
- If several documents repeat the same idea, they may need to be merged.
- A document should be split when doing so improves clarity, reuse, or traceability.
- A document should not be split only because the structure allows it.

## Minimal metadata

A document may include lightweight metadata when useful.

Example:

```md
---
id: context.order-fulfillment
type: context-document
status: active
scope: order-fulfillment
related:
  - process.order-submission
  - decision.order-validation-boundary
---
```

Metadata should support navigation and continuity. It should not become the most important part of the document.

## Modeling principle

Document modeling in VSlices Docs Standard follows one principle: __Use the smallest structure that preserves the knowledge future work depends on__.

- If a note is enough, use a note.
- If a minimal document is enough, use the minimal document.
- If the knowledge becomes stable, risky, reused, or decision-critical, give it more structure.

The purpose is not to model documentation perfectly, but to preserve knowledge deliberately.
