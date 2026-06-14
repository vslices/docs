# Domain Vocabulary

> You can access the [domain vocabulary template here](https://github.com/vslices/docs-standard/blob/main/templates/domain-vocabulary.md)

A Domain Vocabulary preserves the language used inside a business area, system, process, or capability.

Its purpose is to make important terms explicit so that discovery, documentation, design, implementation, and validation do not drift into different meanings.

A vocabulary is not a dictionary of every word used by the business. It is a curated set of terms that matter for understanding and building the system.

## Purpose

A Domain Vocabulary helps the team preserve:

- __shared language__: terms used by domain experts, users, analysts, engineers, and stakeholders.
- __meaning__: what a term means in the current domain context.
- __boundaries__: where a term is valid and where it may mean something else.
- __ambiguity__: terms that are used differently by different people or areas.
- __implementation alignment__: names that may later appear in use cases, capabilities, code, tests, or documentation.

The goal is not to force language too early. It is to make important language visible before it silently becomes system behavior.

## When to use it

Use a Domain Vocabulary when language affects understanding, decisions, or implementation. It is especially useful when:

- __the domain has recurring terms__: people keep using the same words during discovery or planning.
- __terms are ambiguous__: the same word means different things depending on the team, process, area, or system.
- __terms are business-critical__: a wrong interpretation could change behavior, rules, scope, or architecture.
- __the team is new to the domain__: engineers or analysts need a stable reference for domain language.
- __implementation names matter__: terms are likely to appear in code, tests, APIs, screens, or documentation.
- __multiple areas collaborate__: different roles need shared meaning to avoid accidental confusion.

## When not to use it

A Domain Vocabulary may be unnecessary when:

- __the change is small and isolated__: the work does not depend on new or ambiguous terms.
- __the terms are generic__: documenting them would not reduce confusion or risk.
- __the vocabulary would become exhaustive__: the team is trying to document every word instead of the terms that matter.
- __the language is still too unstable__: a Support Note may be enough until the term proves useful.

## Minimal version

Use the minimal version when the team only needs a lightweight shared reference.

```md
# Domain Vocabulary

## Terms

- __Term__: short meaning, example usage, related terms.
```

Example:

```md
- __Reservation__: temporary hold on a resource before confirmation. Related terms: booking, availability.
- __Booking__: confirmed reservation that creates a customer commitment. Related terms: reservation, cancellation.
```

## Expanded version

Use the expanded version when terms are ambiguous, reused, business-critical, or likely to influence implementation.

```md
# Domain Vocabulary

## Terms

### Term name

- __Meaning__: what the term means in this context.
- __Used by__: people, teams, roles, systems, or documents that use this term.
- __Examples__: situations where the term applies.
- __Counterexamples__: situations where the term does not apply.
- __Aliases__: alternative words used for the same or similar concept.
- __Conflicting meanings__: meanings used elsewhere that may cause confusion.
- __Related terms__: nearby concepts.
- __Implementation notes__: possible naming or modeling implications.
- __Status__: draft, active, superseded, or archived.
```

## Standard affinity

This document can support alignment with existing standards and documentation practices. It does not make the documentation compliant by itself.

| Standard | Affinity | Supports |
| -------------------- | -------- | -------- |
| ISO/IEC/IEEE 29148 | Medium | <ul><li>Requirement terminology</li><li>Definitions</li><li>Ambiguity reduction</li><li>Traceability</li></ul> |
| ISO/IEC/IEEE 42010 | Medium | Consistent terms for:<ul><li>Stakeholders</li><li>Concerns</li><li>Views</li><li>Decisions</li><li>Architecture descriptions</li></ul> |

| Practice | Affinity | Supports |
| -------------------- | -------- | -------- |
| arc42 | High | <ul><li>Glossary</li><li>Terminology</li><li>Aliases</li><li>Examples</li><li>Shared language</li></ul> |
| C4 Model | Low / Medium | Naming consistency for:<ul><li>Systems</li><li>Containers</li><li>Components</li><li>Boundaries</li></ul> |
| 4+1 Model | Low / Medium | Shared language across scenarios and<br/>architecture views. |
| ADR | Low / Medium | Naming choices that may influence decisions. |

## Related artifacts

A Domain Vocabulary may support or be supported by:

| Artifact                                      | Relationship                                                                           |
| --------------------------------------------- | -------------------------------------------------------------------------------------- |
| [Context Document](context-document.md)       | Explains where the language appears.                                                   |
| [Process Document](process-document.md)       | Shows how terms are used inside business flows.                                        |
| [Use Case Document](use-case-document.md)     | Depends on clear terms to define expected behavior.                                    |
| [Capability Document](capability-document.md) | May reuse vocabulary to name stable business abilities.                                |
| [Decision Record](decision-record.md)         | May explain why one term or interpretation was chosen.                                 |
| [Support Note](support-note.md)               | May capture early, uncertain, or disputed terms before they<br/>become vocabulary entries. |


## Common mistakes

Common mistakes include:

- __documenting every word__: the vocabulary becomes noise instead of a useful reference.
- __forcing final names too early__: the team treats unstable language as settled.
- __ignoring conflicting meanings__: the same term keeps causing confusion across areas.
- __rewriting business language too soon__: implementation names replace domain language before the team understands it.
- __forgetting examples__: definitions remain abstract and hard to validate.
- __not updating terms__: old meanings remain active after the business or system changes.

## Example questions

A Domain Vocabulary should help answer:

- What does this term mean in this context?
- Who uses this term?
- Is this term used differently elsewhere?
- What examples prove the meaning?
- What should this term not mean?
- Which terms are related or easily confused?
- Could this term influence implementation names or boundaries?

## Continuity

A Domain Vocabulary preserves continuity between business language and system structure.

```text
domain language
-> documented meaning
-> use cases and processes
-> capabilities and decisions
-> implementation names
-> validation and evolution
```

When language remains explicit, the system is less likely to drift away from the domain it represents.
