# Document modeling

VSlices Docs Standard treats documents as evolving structures that preserve useful knowledge.

A document is not only a file. It is a named container for knowledge that can support future understanding, decisions, implementation, validation, or evolution.

The goal of document modeling is to make documentation explicit enough to preserve continuity without turning it into bureaucracy.

!!! principle "Modeling principle"

	Use the smallest structure that preserves the knowledge future work depends on.


## Progressive structure

Documents should grow progressively.

A team should not start with the largest possible version of a document. Not all knowledge should immediately become a formal document either.

VSlices Docs Standard uses four progression levels:

| Level                          | Name               | Use                                                                                                                  |
| ------------------------------ | ------------------ | -------------------------------------------------------------------------------------------------------------------- |
| [L0](#l0---note)               | Note               | Captures early, local, uncertain, or temporary knowledge before the team knows whether it deserves formal structure. |
| [L1](#l1---minimal-document)   | Minimal document   | Captures the smallest useful structure for a document type.                                                          |
| [L2](#l2---expanded-document)  | Expanded document  | Adds detail when complexity, risk, ambiguity, coordination, or lifespan requires it.                                 |
| [L3](#l3---reference-document) | Reference document | Represents stable and important knowledge that should be maintained as a reference for future work.                  |

The levels describe maturity and usefulness, not bureaucracy.

A document should only advance when the knowledge demonstrates enough value.

## L0 - Note

A note captures knowledge quickly.

It is useful when the team needs to preserve something without deciding yet where it belongs.

Examples:

* **Concept note**: an early concept that may later become part of the Domain Vocabulary
* **Assumption note**: something the team believes, but has not validated yet
* **Risk note**: a possible source of failure, misunderstanding, rework, or accidental complexity
* **Open question**: something the team still needs to understand

A note can be resolved, archived, merged into a document, or promoted to a formal document.

## L1 - Minimal document

A minimal document captures the smallest useful structure for a document type.

It should be enough to support a real iteration without becoming heavy.

Use this level when the team knows the knowledge matters, but does not yet need a complete structure.

Examples:

* **Minimal context document**: enough to explain where the team is working
* **Minimal use case document**: enough to explain behavior, consequence, and validations
* **Minimal decision record**: enough to explain what was chosen and why

## L2 - Expanded document

An expanded document adds more explicit structure.

Use this level when the document needs to support greater complexity, risk, ambiguity, reuse, or coordination.

Examples:

* **Expanded process document**: useful when several roles, workflows, exceptions, and handoffs matter
* **Expanded capability document**: useful when several use cases depend on the same stable capability
* **Expanded decision record**: useful when options, tradeoffs, risks, and review conditions matter

A document should grow because the domain requires it, not because the template allows it.

## L3 - Reference document

A reference document is maintained as a stable source of truth for future work.

L3 is not a separate template. It is a maturity level meaning that the document is important enough to be reviewed, maintained, and used as a reference.

Examples:

* **Reference domain vocabulary**: stable language used across several documents and teams
* **Reference context document**: shared foundation for a long-lived scenario or work line
* **Reference capability document**: stable capability that influences several use cases, decisions, or implementation areas

Not all documents should reach L3.

Most should remain as notes, minimal documents, or expanded documents.

!!! principle "Progression principle"

	Everything can begin as a note. Only knowledge that proves useful should gain more structure.


## Document lifecycle

A document can evolve through different states.

| Status     | Meaning                                                             |
| ---------- | ------------------------------------------------------------------- |
| draft      | Still being shaped.                                                 |
| active     | Currently represents useful shared knowledge.                       |
| superseded | Was replaced by newer knowledge.                                    |
| archived   | Is no longer active, but may still be useful as historical context. |

A document should not be treated as permanent just because it exists.

When the system changes, documentation may need to change with it.

## Identity and metadata

Documents should be easy to reference.

A document may have a stable identifier when it needs to connect with other documents.

Examples:

* context.order-fulfillment
* process.order-submission
* use-case.create-reservation
* capability.validate-payment
* decision.order-validation-boundary
* validation.payment-rules-feedback

The identifier does not need to be complex. It only needs to help readers understand what the document refers to and how it connects with other knowledge.

A document may also include lightweight metadata when useful.

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

## Relationships between documents

Documents should not live as isolated files.

They can relate to each other through simple relationships.

| Relationship | Use                                                            |
| ------------ | -------------------------------------------------------------- |
| supports     | One document supports or gives context to another.             |
| refines      | One document makes another document's knowledge more specific. |
| depends-on   | One document depends on knowledge preserved in another.        |
| validates    | One document confirms previous knowledge.                      |
| challenges   | One document questions or casts doubt on previous knowledge.   |
| supersedes   | One document replaces previous knowledge.                      |

Examples:

* A Use Case Document refines a Context Document.
* A Capability Document supports several Use Case Documents.
* A Decision Record depends on a Risk Note.
* A Validation Note validates or challenges an Assumption Note.
* A newer Decision Record supersedes an earlier Decision Record.

## Granularity

A document should preserve one coherent piece of knowledge.

* If a document tries to explain too many things, it may need to be split.
* If several documents repeat the same idea, they may need to be merged.
* A document should be split when doing so improves clarity, reuse, or traceability.
* A document should not be split only because the structure allows it.

!!! risk "Risk to avoid"

	Splitting documents without a continuity reason can create fragmentation instead of clarity.


## Modeling rule

The purpose is not to model documentation perfectly.

The purpose is to preserve knowledge deliberately.

* If a note is enough, use a note.
* If a minimal document is enough, use the minimal document.
* If knowledge becomes stable, risky, reused, or critical for decisions, give it more structure.

!!! principle "Modeling principle"

    Use the smallest document structure that preserves the knowledge needed for future work.
