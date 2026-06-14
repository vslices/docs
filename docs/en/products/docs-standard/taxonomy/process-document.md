# Process Document

> You can access the [process document template here](https://github.com/vslices/docs-standard/blob/main/templates/process-document.md)

A Process Document preserves how a work line operates.

Its purpose is to make responsibilities, roles, coordination rules, workflows, handoffs, and outcomes visible enough to support better design and implementation decisions.

A Process Document answers:

> How do we do it?
> 
> What is done?

A Process Document is not a complete operational manual. It describes the process knowledge that matters for understanding, improving, automating, or preserving how work is performed.

## Purpose

A Process Document helps the team preserve:

* **work process**: how a work line is performed in practice.
* **responsibilities**: who owns, performs, approves, supports, or reacts to work.
* **roles and positions**: which cargos, teams, areas, or systems participate.
* **coordination rules**: how participants organize work between them.
* **workflows**: concrete sequences of steps, decisions, handoffs, and responsible participants.
* **exceptions**: alternative paths, failures, rework, or unusual cases.
* **friction**: delays, ambiguity, duplication, manual work, or fragile coordination.

The goal is to understand how work is organized before changing or automating it.

## When to use it

Use a Process Document when the way work is performed affects understanding, planning, or implementation.

It is especially useful when:

- __the work line needs operational clarity__: the team needs to understand how value is currently produced.
- __responsibilities are important__: roles, ownership, approvals, or reactions affect the process.
- __coordination is fragile__: work depends on handoffs, timing, communication, or implicit agreements.
- __several workflows exist__: the process contains multiple paths, variants, or operational cases.
- __rules shape the process__: business conditions affect what can happen and who must act.
- __automation is being considered__: software may support, replace, or modify existing work.
- __current behavior is inconsistent__: different people describe the process differently.

## When not to use it

A Process Document may be unnecessary when:

- __the process is trivial__: the way work is performed does not affect design decisions.
- __the scenario is still unclear__: a Context Document or Support Note may be needed first.
- __only one interaction matters__: a Use Case Document may be enough.
- __only a sequence of steps matters__: a small workflow note may be enough.
- __the team is documenting every operational detail__: the document becomes an exhaustive procedure manual.
- __the process is too unstable__: a Support Note may be better until the work process becomes clearer.

## Minimal version

Use the minimal version when the team needs a lightweight description of how work is performed.

```md
# Process Document

## Work process

How is this work line performed?

## Purpose

Why does this process exist?

## Participants and responsibilities

Who participates and what are they responsible for?

## Main workflow

- Step 1.
- Step 2.
- Step 3.

## Outcome

What does this process produce?

## Pain points or risks

What makes this process fragile, slow, unclear, or risky?
```

## Expanded version

Use the expanded version when the process is complex, risky, cross-functional, or likely to guide implementation.

```md id="rhx9ii"
# Process Document

## Work process

## Purpose

## Scope

## Related scenario or work line

## Participants, roles, and responsibilities

## Preconditions

## Coordination rules

## Main workflow

## Alternative workflows

## Exceptions and rework

## Business rules

## Handoffs

## Inputs

## Outputs

## Systems or tools involved

## Pain points

## Risks

## Related artifacts
```

## Standard affinity

This document can support alignment with existing standards and documentation practices. It does not make the documentation compliant by itself.

| Standard | Affinity | Supports |
| -------------------- | -------- | -------- |
| ISO/IEC/IEEE 29148 | Medium | Process-related requirements, assumptions, business rules, and validation inputs. |
| ISO/IEC/IEEE 42010 | Medium | Concerns, relationships, and process constraints that may shape architecture. |

| Practice | Affinity | Supports |
| -------------------- | -------- | -------- |
| arc42 | Medium / High | Runtime behavior, process movement, risks, responsibilities, and operational concerns. |
| 4+1 View Model | Medium | Process-oriented view thinking and scenario support. |
| C4 Model | Low / Medium | Boundary and interaction awareness. |
| ADR | Low / Medium | Process constraints that may justify decisions. |

## Related artifacts

A Process Document may support or be supported by:

- __Context Document__: explains the scenario and work line where the process exists.
- __Domain Vocabulary__: preserves terms used inside the process.
- __Use Case Document__: describes the meaning, consequences, and validations of specific behavior.
- __Capability Document__: identifies stable abilities required to perform or improve the process.
- __Decision Record__: explains choices made because of process constraints.
- __Validation Note__: captures what was learned after changing or testing the process.
- __Support Note__: captures uncertain responsibilities, workflow variants, risks, assumptions, or open questions.

## Common mistakes

Common mistakes include:

- __confusing process with workflow__: the document only lists steps and misses responsibilities or coordination.
- __documenting every detail__: the process becomes too large to guide decisions.
- __only writing the happy path__: exceptions and rework remain invisible.
- __ignoring handoffs__: the most fragile parts of the process disappear.
- __mixing current and target behavior__: readers cannot tell what exists today and what is proposed.
- __hiding ownership__: responsibilities remain implicit.
- __jumping to automation__: the team designs software before understanding the work.
- __not updating after change__: the documented process no longer matches reality.

## Example questions

A Process Document should help answer:

- How is this work line performed?
- Why does this process exist?
- Who participates and what are they responsible for?
- How do participants coordinate work?
- What workflows exist inside this process?
- What happens first, next, and last?
- Where does work move between people, areas, systems, or tools?
- What makes the process slow, fragile, risky, or unclear?
- Which use cases, capabilities, or decisions depend on this process?

## Continuity

A Process Document preserves continuity between operational structure and software behavior.

```text 
work line
-> work process
-> responsibilities and workflows
-> use cases and capabilities
-> decisions and implementation
-> validation and evolution
```

When process behavior remains explicit, the team is less likely to build software that works technically but fails operationally.
