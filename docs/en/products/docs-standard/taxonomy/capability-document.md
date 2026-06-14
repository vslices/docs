# Capability Document

> You can access the [capability document template here](https://github.com/vslices/docs-standard/blob/main/templates/capability-document.md)

A Capability Document preserves a stable ability required by the business or system.

Its purpose is to describe what must be possible without deciding too early how it must be implemented. A Capability Document answers:

> What must this business or system be able to do?

A capability is not a feature, endpoint, screen, service, or technical component. It is an ability that may support several use cases, workflows, processes, or decisions.

## Purpose

A Capability Document helps the team preserve:

- __stable ability__: what the business or system needs to be able to do.
- __business value__: why this ability matters.
- __supported behavior__: which use cases or workflows depend on the capability.
- __boundaries__: what the capability includes and excludes.
- __rules and constraints__: what shapes or limits the capability.
- __expected outcomes__: what this capability enables.
- __implementation independence__: the capability can be understood before choosing code structure.

The goal is to identify meaningful abilities without turning them into technical components too early.

## When to use it

Use a Capability Document when an ability is stable enough to guide design or implementation. It is especially useful when:

- __several use cases need the same ability__: the capability appears repeatedly across behavior.
- __a process depends on a stable ability__: the process cannot work without this capability.
- __the ability may define a boundary__: ownership, responsibility, or architecture may emerge around it.
- __business value needs to stay visible__: the team must remember why the ability matters.
- __implementation options are still open__: the team needs clarity before choosing a design.
- __future evolution is expected__: the capability may grow, split, or become more formal later.

## When not to use it

A Capability Document may be unnecessary when:

- __the behavior is isolated__: a Use Case Document is enough.
- __the ability is too vague__: the team cannot yet explain what must be possible.
- __the team is naming technical components__: the document is being used to justify architecture too early.
- __the capability is only a feature name__: there is no stable ability behind it.
- __the domain is still unclear__: a Context Document, Process Document, or Support Note may be needed first.

## Minimal version

Use the minimal version when the team needs a lightweight capability definition.

```md id="i55iqq"
# Capability Document

## Capability

What must the business or system be able to do?

## Why it matters

What value does this ability provide?

## Supported behavior

Which use cases, workflows, or processes depend on it?

## Boundaries

What is included and what is outside?

## Rules or constraints

What shapes or limits this capability?

## Related artifacts

Which context, process, use case, decision, or validation supports this capability?
```

## Expanded version

Use the expanded version when the capability is important, reused, risky, or likely to influence architecture.

```md
# Capability Document

## Capability

## Purpose

## Business value

## Related scenario or work line

## Supported processes

## Supported workflows

## Supported use cases

## Boundaries

## Responsibilities

## Inputs

## Outputs

## Rules and constraints

## Expected outcomes

## Expected errors

## Dependencies

## Related decisions

## Validation notes

## Evolution notes
```

## Standard affinity

This document can support alignment with existing standards and documentation practices. It does not make the documentation compliant by itself.

| Standard | Affinity | Supports |
| -------------------- | -------- | -------- |
| ISO/IEC/IEEE 42010 | Medium / High | Architecture concerns, boundaries, rationale, and relationships between capabilities and decisions. |
| ISO/IEC/IEEE 29148 | Medium | Capability-related requirements, constraints, expected outcomes, and traceability. |

| Practice | Affinity | Supports |
| -------------------- | -------- | -------- |
| arc42 | Medium / High | Building block thinking, responsibilities, boundaries, risks, and decisions. |
| C4 Model | Medium | Boundary awareness that may later influence container or component views. |
| 4+1 View Model | Medium | Logical and process-oriented architecture thinking. |
| ADR | Medium | Decisions about capability shape, split, ownership, or implementation direction. |

## Related artifacts

A Capability Document may support or be supported by:

| Artifact                                  | Relationship                                                                             |
| ----------------------------------------- | ---------------------------------------------------------------------------------------- |
| [Context Document](context-document.md)   | Explains the scenario or work line where the capability matters.                         |
| [Process Document](process-document.md)   | Shows which processes require the capability.                                            |
| [Use Case Document](use-case-document.md) | Describes behaviors enabled by the capability.                                           |
| [Domain Vocabulary](domain-vocabulary.md) | Preserves the language used to name and explain the capability.                          |
| [Decision Record](decision-record.md)     | Explains why the capability was shaped, split, merged, or implemented in a specific way. |
| [Validation Note](validation-note.md)     | Captures evidence about whether the capability supports real needs.                      |
| [Support Note](support-note.md)           | Captures early ability ideas before they become stable capabilities.                     |


## Common mistakes

Common mistakes include:

- __confusing capability with feature__: a feature delivers a concrete behavior, while a capability describes a stable ability.
- __confusing capability with component__: the document becomes architecture before the domain need is clear.
- __naming too early__: the team gives formal names to abilities that are still vague.
- __making it too broad__: the capability becomes a container for unrelated behavior.
- __making it too narrow__: the capability only repeats one use case.
- __ignoring boundaries__: readers cannot tell what the capability includes or excludes.
- __forgetting value__: the capability exists, but nobody remembers why it matters.

## Example questions

A Capability Document should help answer:

- What must the business or system be able to do?
- Why does this ability matter?
- Which use cases, workflows, or processes depend on it?
- What is included in this capability?
- What is outside this capability?
- What rules, constraints, or outcomes shape it?
- Could this capability become a boundary?
- Which decisions or validations depend on this capability?

## Continuity

A Capability Document preserves continuity between domain needs and possible implementation structure.

```text
scenario or work line
-> work process and use cases
-> stable ability
-> decisions and implementation options
-> validation and evolution
```

When capabilities remain independent from implementation too early, the team can reason about what the system must provide before deciding how the system should be structured.
