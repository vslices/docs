# Context Document

> You can access the [context document template here](https://github.com/vslices/docs-standard/blob/main/templates/context-document.md)

A Context Document preserves the scenario where the team is working.

Its purpose is to make the relevant business, organizational, operational, or system context visible enough to support better decisions. A Context Document answers:

- Where are we working?
- What does this area offer, operate, or maintain?

A Context Document is not a complete map of the business. It captures the context that matters for understanding what may need to be designed, improved, automated, integrated, or preserved.

## Purpose

A Context Document helps the team preserve:

- __scenario__: the business, organizational, operational, or system context being observed.
- __work lines__: the areas, departments, services, business lines, or offerings inside the scenario.
- __actors and areas__: who participates in the context.
- __current situation__: how the scenario behaves today at a high level.
- __pain points and opportunities__: what may justify future work.
- __boundaries__: where the scenario starts, ends, or becomes unclear.
- __uncertainty__: assumptions, risks, and open questions that still need attention.

The goal is to create enough shared understanding to avoid designing from isolated requirements.

## When to use it

Use a Context Document when the surrounding scenario affects understanding, planning, or implementation. It is especially useful when:

- __the scenario is unclear__: the team does not yet understand where the work happens.
- __several work lines exist__: the area includes multiple departments, services, or offerings.
- __many actors participate__: responsibilities, ownership, or collaboration may matter.
- __the current situation is fragmented__: work happens across manual steps, tools, documents, or legacy systems.
- __the change may affect adjacent work__: a local improvement could impact surrounding areas or services.
- __the team needs a shared base__: later documents need a stable contextual reference.
- __the cost of misunderstanding is high__: building from weak context could create accidental complexity.

## When not to use it

A Context Document may be unnecessary when:

- __the change is small and isolated__: surrounding context does not affect the decision.
- __the scenario is already understood__: existing documentation or team knowledge is enough.
- __only the process matters__: a Process Document may be more useful.
- __only behavior matters__: a Use Case Document may be enough.
- __the team needs fast feedback__: a small slice can safely produce better learning.
- __the document would become a full business map__: the team is trying to document everything instead of the relevant context.
- __a support note is enough__: the context is still early, small, or uncertain.

## Minimal version

Use the minimal version when the team needs a lightweight shared base.

```md
# Context Document

## Scenario

Where are we working?

## Why it matters

Why this scenario is relevant now.

## Scope

What is included and what is intentionally outside.

## Work lines

What areas, departments, services, or offerings exist inside this scenario?

## Current situation

How the scenario behaves today at a high level.

## Actors and areas

Who participates in this scenario?

## Pain points or opportunities

What may justify future work?

## Open questions

What still needs to be understood?
```

## Expanded version

Use the expanded version when the scenario is broad, risky, fragmented, or likely to guide several future documents.

```md 
# Context Document

## Scenario

## Purpose

## Scope

## Out of scope

## Business background

## Work lines

## Actors, areas, and responsibilities

## Current situation

## Current systems or tools

## Pain points and opportunities

## Boundaries

## Relevant vocabulary

## Assumptions

## Risks

## Open questions

## Related artifacts
```

## Standard affinity

This document can support alignment with existing standards and documentation practices. It does not make the documentation compliant by itself.

| Standard | Affinity | Supports |
| -------------------- | -------- | -------- |
| ISO/IEC/IEEE 29148 | Medium | Context for:<ul><li>Requirements</li><li>Assumptions</li><li>Risks</li><li>Traceability</li></ul> |
| ISO/IEC/IEEE 42010 | High | <ul><li>Context</li><li>Concerns</li><li>Stakeholders</li><li>Boundaries</li><li>Relationships</li><li>Rationale inputs</li></ul> |

| Practice | Affinity | Supports |
| -------------------- | -------- | -------- |
| C4 Model | High | <ul><li>System context thinking</li><li>Actors</li><li>Systems</li><li>Boundary awareness</li></ul> |
| arc42 | High | <ul><li>Context and scope</li><li>External interfaces</li><li>Constraints</li><li>Risks</li><li>Glossary connections</li></ul> |
| 4+1 Model | Medium | Scenario and context grounding for later views. |
| ADR | Low / Medium | Context for decisions and tradeoffs. |

## Related artifacts

A Context Document may support or be supported by:

| Artifact                                      | Relationship                                                             |
| --------------------------------------------- | ------------------------------------------------------------------------ |
| [Domain Vocabulary](domain-vocabulary.md)     | Preserves important terms discovered inside the scenario.                |
| [Process Document](process-document.md)       | Describes how work lines operate through responsibilities and workflows. |
| [Use Case Document](use-case-document.md)     | Defines expected behavior supported by the scenario.                     |
| [Capability Document](capability-document.md) | Identifies stable abilities needed inside the scenario or work line.     |
| [Decision Record](decision-record.md)         | Explains decisions made because of contextual constraints.               |
| [Validation Note](validation-note.md)         | Captures learning that changes or confirms the scenario.                 |
| [Support Note](support-note.md)               | Captures early findings before they become part of the context.          |

## Common mistakes

Common mistakes include:

- __documenting the whole business__: the document becomes too broad to guide decisions.
- __jumping to solutions__: the document starts describing what to build instead of where the team is working.
- __confusing scenario with process__: the document over-describes how work is done.
- __confusing work line with workflow__: services or areas are described as step-by-step flows.
- __ignoring boundaries__: the team cannot tell where the scenario stops.
- __hiding uncertainty__: assumptions and open questions are written as facts.
- __not updating after learning__: implementation feedback changes the scenario but the document stays frozen.

## Example questions

A Context Document should help answer:

- Where are we working?
- Why does this scenario matter now?
- What work lines exist inside this scenario?
- Who participates in this scenario?
- What currently happens at a high level?
- Which pain points or opportunities are visible?
- Which boundaries are clear or unclear?
- What do we still not understand?
- Which documents or decisions depend on this context?

## Continuity

A Context Document preserves continuity between discovered business reality and later software decisions.

```text
scenario
-> work lines
-> shared understanding
-> processes and use cases
-> capabilities and decisions
-> implementation scope
-> validation and evolution
```

When context remains visible, later artifacts are less likely to become isolated from the scenario that justified them.
