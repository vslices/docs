# Support Note

> > You can access the [support note template here](https://github.com/vslices/docs-standard/blob/main/templates/support-note.md)

A Support Note preserves useful knowledge that is not ready or important enough to become a formal document.

Its purpose is to capture concepts, assumptions, risks, questions, feedback, implementation details, or improvement ideas without adding unnecessary structure. A Support Note answers:

> What should we not lose yet?

A support note is intentionally lightweight. It can later be merged into a document, linked from another artifact, superseded, or archived.

## Purpose

A Support Note helps the team preserve:

- __early knowledge__: ideas, observations, or findings that are still forming.
- __uncertainty__: assumptions, risks, open questions, and unclear concepts.
- __local detail__: information useful in a specific context but not broad enough for a full document.
- __temporary learning__: feedback, implementation notes, or discoveries that may matter later.
- __future candidates__: knowledge that may become part of a Context Document, Process Document, Use Case Document, Capability Document, Decision Record, or Validation Note.

The goal is to preserve useful knowledge without forcing premature structure.

## Common types

Support Notes may include:

| Type                | When to use it                                                                        | Use                                                                                                       |
| ------------------- | ------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- |
| Concept Note        | When an idea appears but is still<br/>immature.                                       | Captures an early concept before it<br/>becomes part of the Domain Vocabulary<br/>or another document.    |
| Assumption Note     | When something seems true, but<br/>has not been validated yet.                        | Captures something the team believes<br/>to be true, but has not validated yet.                           |
| Risk Note           | When something could fail, cause<br/>delay, or introduce accidental complexity.       | Captures a possible source of failure,<br/>misunderstanding, delay, rework, or<br/>accidental complexity. |
| Open Question       | When the team still needs to<br/>understand something.                                | Captures something the team still needs<br/>to understand.                                                |
| Feature Note        | When a *feature* idea appears before<br/>the use case, capability, or scope is clear. | Captures an early *feature* idea before<br/>its use case, capability, or scope is clear.                  |
| Feedback Note       | When someone provides input that<br/>may change understanding or direction.           | Captures input from users, domain experts,<br/>stakeholders, implementation, or operation.                |
| Implementation Note | When useful technical detail appears,<br/>but there is no decision yet.               | Captures useful technical detail that is<br/>not yet a Decision Record.                                   |
| Scope Note          | When something may be included,<br/>excluded, postponed, or intentionally ignored.    | Captures what may be included, excluded,<br/>postponed, or intentionally ignored.                         |
| Improvement Note    | When a possible improvement appears,<br/>but is not yet a planned change.             | Captures a possible improvement before<br/>it becomes a planned change.                                   |


## When to use it

Use a Support Note when knowledge should be preserved, but a formal document would be too much. It is especially useful when:

- __the idea is early__: the team does not yet know where it belongs.
- __the knowledge is uncertain__: the team needs to track an assumption, risk, or question.
- __the detail is local__: the information matters, but only in a narrow context.
- __the team needs speed__: writing a full document would slow learning without adding value.
- __the knowledge may evolve__: the note may later become part of a larger document.

## When not to use it

A Support Note may be insufficient when:

- __the knowledge is stable and reused__: a formal document may be better.
- __the note affects major decisions__: a Decision Record may be needed.
- __the note describes expected behavior__: a Use Case Document may be clearer.
- __the note describes a process__: a Process Document may be better.
- __the note validates something important__: a Validation Note may be needed.
- __too many notes repeat the same topic__: the knowledge should probably be consolidated.

## Suggested structure

Use the smallest structure that preserves the note.

```md
# Support Note

## Type

Concept, assumption, risk, question, feedback, implementation, scope, or improvement.

## Note

What should be preserved?

## Context

Where did this appear?

## Why it matters

Why could this matter later?

## Status

Open, active, resolved, superseded, or archived.

## Related artifacts

Which documents, decisions, or notes are connected?
```

## Standard affinity

This document can support alignment with existing standards and documentation practices. It does not make the documentation compliant by itself.

| Standard or practice | Affinity | Supports |
| -------------------- | -------- | -------- |
| ISO/IEC/IEEE 29148 | Medium | Assumptions, risks, open questions, feedback, and early requirement inputs. |
| ISO/IEC/IEEE 42010 | Medium | Early concerns, stakeholder notes, rationale inputs, and relationships. |

| Standard or practice | Affinity | Supports |
| -------------------- | -------- | -------- |
| arc42 | Medium | Risks, constraints, open questions, glossary candidates, and decision inputs. |
| ADR | Medium | Early decision inputs, options, assumptions, and risks. |
| C4 Model | Low | Early notes about boundaries, systems, and responsibilities. |
| 4+1 View Model | Low | Early scenario, behavior, or view-related notes. |

## Common mistakes

Common mistakes include:

- __using notes forever__: stable knowledge never becomes formal documentation.
- __creating too many disconnected notes__: useful knowledge becomes hard to find.
- __hiding important decisions__: a note is used when a Decision Record is needed.
- __treating assumptions as facts__: uncertainty disappears from the documentation.
- __not resolving questions__: open questions remain open after the team learns the answer.
- __not consolidating repeated notes__: related knowledge stays fragmented.

## Example questions

A Support Note should help answer:

- What useful knowledge should not be lost?
- Is this a concept, assumption, risk, question, feedback, implementation detail, scope note, or improvement idea?
- Where did this knowledge appear?
- Why might it matter later?
- Is it still open, active, resolved, superseded, or archived?
- Should this note become part of a formal document?

## Continuity

A Support Note preserves continuity between early discovery and structured documentation.

```text
observation or idea
-> support note
-> related document or decision
-> validation or archive
-> future learning
```

When notes remain lightweight, the team can preserve emerging knowledge without turning every observation into a formal document.
