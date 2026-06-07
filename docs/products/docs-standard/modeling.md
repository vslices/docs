# Document Modeling

VSlices Docs Standard treats documents as evolving structures that preserve useful knowledge.

A document is not only a file, it is a named container for knowledge that may support future understanding, decisions, implementation, validation, or evolution.

The goal of document modeling is to make documentation explicit enough to preserve continuity without turning it into bureaucracy.

## Progressive structure

Documents should grow progressively.

A team should not start with the largest possible version of a document, and not every piece of knowledge should become a formal document immediately. VSlices Docs Standard uses four progression levels:

- __L0 - Note__: captures early, local, uncertain, or temporary knowledge before the team knows whether it deserves formal structure.
- __L1 - Minimal Document__: captures the smallest useful structure for a document type.
- __L2 - Expanded Document__: adds detail when complexity, risk, ambiguity, team size, reuse, or system lifetime requires more explicit documentation.
- __L3 - Reference Document__: represents knowledge stable and important enough to become a maintained reference for future work.

The levels describe maturity and usefulness, not bureaucracy. A document should move forward only when the knowledge proves valuable enough.

### L0 - Note

A note captures knowledge quickly. 

It is useful when the team needs to preserve something without deciding where it belongs yet. Examples:

- __Concept Note__: an early concept that may later become part of the Domain Vocabulary.
- __Assumption Note__: something the team believes but has not validated yet.
- __Risk Note__: a possible source of failure, misunderstanding, rework, or accidental complexity.
- __Open Question__: something the team still needs to understand.

A note may be resolved, archived, merged into a document, or promoted into a formal document.

### L1 - Minimal Document

A minimal document captures the smallest useful structure for a document type. It should be enough to support a real iteration without becoming heavy.

Use this level when the team knows the knowledge matters, but does not need a complete structure yet. Examples:

- __minimal Context Document__: enough to explain where the team is working.
- __minimal Use Case Document__: enough to explain behavior, consequence, and validations.
- __minimal Decision Record__: enough to explain what was chosen and why.

### L2 - Expanded Document

An expanded document adds more explicit structure. 

Use this level when the document must support higher complexity, risk, ambiguity, reuse, or coordination. Examples:

- __expanded Process Document__: useful when several roles, workflows, exceptions, and handoffs matter.
- __expanded Capability Document__: useful when several use cases depend on the same stable ability.
- __expanded Decision Record__: useful when options, tradeoffs, risks, and review conditions matter.

A document should become larger because the domain requires it, not because the template allows it.

### L3 - Reference Document

A reference document is maintained as a stable source of truth for future work.

L3 is not a separate template. It is a maturity level that means the document is important enough to be reviewed, maintained, and trusted as a reference. Examples:

- __reference Domain Vocabulary__: stable language used across several documents and teams.
- __reference Context Document__: shared base for a long-lived scenario or work line.
- __reference Capability Document__: stable ability that influences several use cases, decisions, or implementation areas.

Not every document should reach L3. Most documents should remain notes, minimal documents, or expanded documents. The rule is simple:

> Everything can start as a note. Only knowledge that proves useful should gain more structure.

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
