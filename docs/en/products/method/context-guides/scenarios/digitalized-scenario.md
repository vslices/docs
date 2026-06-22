# Scenario "Digitized"

A "Digitized" scenario is a work context where software already represents part of the business, process, or organization.

This does not mean the domain is already understood. Existing software is evidence, not automatically the truth of the domain.

## Core idea

In a digitized scenario, VSlices Method helps the team separate three things:

* how the work really happens
* how the current software represents that work
* how people have adapted their work around the software

!!! principle "Continuity principle"

    The goal is not to reverse engineer the whole system. It is to recover enough continuity to make the next responsible decision.


## When this guide applies

Use this guide when:

* software already exists
* workflows are partially or fully supported by a system
* people depend on current screens, reports, forms, APIs, or automations
* the team needs to improve, replace, or extend existing behavior
* documentation is missing, outdated, or disconnected from the implementation
* business knowledge is hidden inside code, tickets, or user habits

This guide can apply whether or not the project already uses VSlices Method.

## Main risk

The main risk is treating existing software as the truth of the domain.

A system may contain:

* real business rules
* obsolete decisions
* workarounds turned into behavior
* accidental constraints
* technical compromises
* missing concepts
* misleading names
* behaviors users have learned to tolerate

!!! risk "Risk to avoid"

    If the team copies the existing system without questioning it, it may preserve accidental complexity as if it were domain knowledge.


## Useful initial modality

A digitized scenario usually starts with [**Context-First**](../../../design/modalities/context-first/index.md) or [**Problem-First**](../../../design/modalities/problem-first/index.md), because the team needs to understand what the current system represents and which problem should be solved first.

| Situation                                                              | Useful modality                                                 | Reason                                                                                   |
| ---------------------------------------------------------------------- | --------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| The system exists, but the surrounding business context is unclear.    | **Context-First**                                               | The team needs to understand what the software is trying to represent.                   |
| There is a clear pain in the current system, but the cause is unclear. | **Problem-First**                                               | The team needs to understand the problem before changing the behavior.                   |
| A small and safe improvement can reveal useful evidence.               | [**Slice-First**](../../../design/modalities/slice-first/index.md) | The team can learn through a bounded change without pretending to understand everything. |

!!! risk "Risk to avoid"

    Slice-First can be useful, but only when the change is small enough to avoid spreading misunderstood assumptions.

## Affinity with continuity paths

A digitalized scenario usually has stronger affinity with the paths that help recover continuity between the real work, the existing software, and the next change decision.

Not every path should be walked with the same depth.

| Continuity path    | Typical affinity | Use in this context                                                                                                                   |
| ------------------ | ---------------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| Business scenario  | High             | Understand what real work the current software represents or supports.                                                                |
| Domain context     | High             | Separate domain language, rules, and meanings from accidental system names, constraints, or decisions.                                |
| Software project   | High             | Locate the technical initiative, change boundaries, existing dependencies, and implementation risks.                                  |
| Client product     | Medium           | Understand visible behavior for users when the change affects screens, forms, reports, or usage flows.                                |
| Consumable service | Medium           | Understand exposed or consumed capabilities when the change affects APIs, integrations, automations, or dependencies between systems. |

!!! principle "Affinity principle"

    Start from the path that best explains the continuity at risk. Do not force every digitalized scenario to walk every path.


In a digitalized scenario, the primary path usually depends on the type of change.

| Observed change                                                      | Path worth prioritizing |
| -------------------------------------------------------------------- | ----------------------- |
| The system does not properly reflect how the work currently happens. | Business scenario       |
| The system terms do not match the business language.                 | Domain context          |
| The team needs to safely modify an existing codebase.                | Software project        |
| Visible behavior for users needs to change.                          | Client product          |
| An API, integration, or automation needs to change.                  | Consumable service      |

!!! risk "Over-recovery risk"

    Recovering continuity does not mean documenting the whole existing system. It means preserving what is needed to change it without losing intent.


## What to observe first

Before changing the system, observe how the current work connects with the current software.

| Observe                                                              | To understand                                                |
| -------------------------------------------------------------------- | ------------------------------------------------------------ |
| What real work this software supports                                | Which part of the business is being represented or assisted. |
| Which workflows depend on it                                         | Which processes could be affected by a change.               |
| Which actors use it directly or indirectly                           | Who depends on the current behavior.                         |
| Which parts of the system are reliable                               | Which behavior can be treated as stable evidence.            |
| Which parts are avoided, manually corrected, or worked around        | Which frictions reveal limits of the current system.         |
| Which business terms appear in the interface, code, or documentation | Which language may reveal domain intent.                     |
| Which behaviors are expected but not explicit                        | Which knowledge may be hidden in use, support, or operation. |
| Which errors or exceptions happen repeatedly                         | Which fragilities should be understood before changing.      |
| Which decisions are historical, technical, or no longer understood   | Which parts require context recovery before moving forward.  |

The goal is not to perform a complete analysis. It is to find where continuity is missing.

## Knowledge to preserve

Preserve knowledge when it affects the next change.

Useful knowledge may include:

* domain terms found in the system
* differences between real work and software behavior
* existing workflows affected by the change
* rules hidden inside the implementation
* user workarounds
* current pains
* constraints created by integrations or data
* decisions that should be kept, changed, or questioned
* validation signals from users, support, or operation

!!! principle "Continuity principle"

    Do not document the whole existing system by default.

    Preserve what future work should not have to rediscover.


## Documentation support

Documents can help recover continuity in a digitized scenario.

| Knowledge need                                                     | Useful document                                                                                                                                                                         |
| ------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Terms are ambiguous or inconsistent.                               | Domain Vocabulary — [Taxonomy](../../../docs-standard/taxonomy/domain-vocabulary.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/domain-vocabulary.md)       |
| The surrounding business scenario is unclear.                      | Context Document — [Taxonomy](../../../docs-standard/taxonomy/context-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/context-document.md)          |
| The current work depends on workflows or handoffs.                 | Process Document — [Taxonomy](../../../docs-standard/taxonomy/process-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/process-document.md)          |
| A specific behavior needs to be changed or preserved.              | Use Case Document — [Taxonomy](../../../docs-standard/taxonomy/use-case-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/use-case-document.md)       |
| A stable business ability is emerging.                             | Capability Document — [Taxonomy](../../../docs-standard/taxonomy/capability-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/capability-document.md) |
| A direction must be chosen under tradeoffs.                        | Decision Record — [Taxonomy](../../../docs-standard/taxonomy/decision-record.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/decision-record.md)             |
| Evidence from use, operation, or review changes the understanding. | Validation Note — [Taxonomy](../../../docs-standard/taxonomy/validation-note.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/validation-note.md)             |
| Observations are still local, uncertain, or temporary.             | Support Note — [Taxonomy](../../../docs-standard/taxonomy/support-note.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/support-note.md)                      |

Use the lightest document that protects continuity.

{% include-markdown "shared/readings/document-stage-affinity-admonition.md" %}

## Suggested approach

Start by selecting one area of change. Do not try to understand the whole system first.

A useful approach is:

1. Identify the current pain, opportunity, or change request
2. Locate the workflows, actors, and system behavior around it
3. Compare the current software behavior with the real work
4. Name what is known, what is uncertain, and what is risky
5. Keep only the knowledge needed for the next responsible decision
6. Choose the smallest safe change or the next investigation
7. Use feedback to update the understanding

The team should move between understanding and building as evidence appears.

## Common mistakes

Digitized scenarios often fail when teams assume the system explains itself.

Common mistakes include:

* copying existing behavior without understanding why it exists
* redesigning everything because the current system looks messy
* treating code names as domain language
* ignoring user workarounds
* documenting the whole system before improving anything
* changing behavior without knowing who depends on it
* assuming old decisions are still valid
* assuming old decisions were wrong only because they are old

!!! risk "Do not confuse evidence with truth"

    Existing software should be respected as evidence. It should not be obeyed as truth.

## Guiding principle

!!! principle "General principle"

    Use the existing system as a source of clues.

    Do not keep accidental complexity unless the domain still depends on it.

Recover enough domain, process, behavior, and decision continuity to change the system safely.
