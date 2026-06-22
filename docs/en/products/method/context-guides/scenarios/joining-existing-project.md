# Scenario "Joining an existing project"

A "Joining an existing project" scenario is a work context where a person or team enters work that is already in progress.

The project may use VSlices Method, or it may use another way of working.

The goal is not to restart the project. It is to join the current continuity path before changing the work.

## Core idea

!!! principle "Continuity principle"

    Joining an existing project should not start only from tasks.


Tasks describe what someone should do, but they do not always explain why the work matters, what context supports it, which decisions shaped it, or what feedback changed it.

The question is not *Which tasks should we take?*, but *which continuity path are these tasks part of?*

## When this guide applies

Use this guide when:

* a new person joins a project
* a new team joins an ongoing initiative
* the work is already planned or in progress
* decisions exist that affect the current work
* documentation exists, but needs interpretation
* implementation exists, but the intent is not clear
* the project has active stakeholders, users, or operational constraints
* the team needs to contribute without losing the original context

This guide applies both when one person joins an existing project and when a whole team enters work that has already started.

## Main risk

The main risk is entering through execution without understanding intent.

This can create:

* changes that solve a task, but not the problem
* duplicated discovery
* repeated decisions
* implementation that contradicts previous context
* documentation that ignores existing knowledge
* feedback disconnected from the current work
* local improvements that weaken the whole system

An ongoing project already has history. Part of that history is useful knowledge; another part may be outdated or accidental.

!!! risk "Risk to avoid"

    Before contributing, the team needs to distinguish which continuity should be respected, which decisions should be reviewed, and which complexity should not be inherited.


## Useful initial modality

Introducing Method into an ongoing project should start from the uncertainty that is most affecting the work.

| Situation                                                                 | Useful modality                                                     | Reason                                                                      |
| ------------------------------------------------------------------------- | ------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| The team does not understand where continuity is being lost.              | [**Context-First**](../../../design/modalities/context-first/index.md) | The team needs to understand the context before changing how it works.      |
| There is a clear pain in the current way of working.                      | [**Problem-First**](../../../design/modalities/problem-first/index.md) | The team can introduce Method by solving a concrete friction.               |
| A small practice can improve the work without changing the whole process. | [**Slice-First**](../../../design/modalities/slice-first/index.md)     | The team can validate Method through a bounded and observable intervention. |

!!! risk "Risk to avoid"

    The selected modality should respond to adoption uncertainty, not to the team's personal preference.


## Affinity with continuity paths

Joining an existing project usually has high affinity with the path that explains the active work the person or team is joining.

This is not about walking the entire project.

It is about finding enough continuity to contribute without breaking existing intent, decisions, or behavior.

| Continuity path | Typical affinity | Use in this context |
| --- | --- | --- |
| Business scenario | Medium | Understand what operational reality, need, or workflow sustains the project. |
| Domain context | Medium | Clarify the language, rules, boundaries, and concepts the team needs to understand before contributing. |
| Software project | High | Locate the initiative, current architecture, technical decisions, change boundaries, and state of the work. |
| Client product | Medium if you are a frontend analyst<br/>Low if you are a backend analyst | Understand visible behavior when the contribution affects experience, usage flow, or value delivery. |
| Consumable service | Low if you are a frontend analyst<br/>Medium if you are a backend analyst | Understand capabilities, APIs, integrations, or contracts when the contribution affects dependencies between systems. |

!!! principle "Affinity principle"

    First join the path that explains the intent of the active work. Do not try to reconstruct every path of the project.

In this scenario, the primary path depends on what the person or team needs to understand in order to contribute responsibly.

| Onboarding situation | Path worth prioritizing |
| --- | --- |
| It is not clear why the current work exists. | Business scenario |
| The project language is hard to interpret. | Domain context |
| It is not clear how the task fits into the technical initiative. | Software project |
| The contribution affects visible behavior for users. | Client product |
| The contribution affects APIs, integrations, or shared capabilities. | Consumable service |

!!! risk "Infinite onboarding risk"

    Joining the continuity path does not mean understanding everything before contributing. It means recovering the minimum continuity needed to contribute without breaking intent.
    

## What to observe first

Before suggesting Method practices, observe how work currently moves.

| Observe                                                     | To understand                                               |
| ----------------------------------------------------------- | ----------------------------------------------------------- |
| Where intent is lost                                        | Which part of the work stops explaining why it matters.     |
| Where people repeat the same explanations                   | Which knowledge depends too much on memory or conversation. |
| Where decisions are made                                    | Which moments need to preserve context.                     |
| Where decisions are forgotten                               | Which continuity is lost between decision and future work.  |
| Where documentation stops matching reality                  | Which documents need to be updated, reduced, or replaced.   |
| Where implementation loses business context                 | Which behavior needs to recover intent.                     |
| Where feedback disappears                                   | Which learning is not changing future decisions.            |
| Which handoffs create confusion                             | Where continuity breaks between people, teams, or stages.   |
| Which small improvement would help current work immediately | Where Method can enter with real usefulness and low weight. |

The goal is not to judge the team's process. It is to find a continuity gap worth improving.

## Knowledge to preserve

Joining an existing project can reveal missing or fragile continuity.

Preserve knowledge when it helps newcomers or future work avoid assumptions.

Useful knowledge may include:

* project vocabulary that is not obvious
* decisions that explain the current implementation
* active assumptions
* known constraints
* current workflow or use case boundaries
* validation results that shaped the current direction
* differences between documented intent and real implementation
* onboarding questions that reveal hidden knowledge
* outdated knowledge that should be reviewed

!!! principle "Continuity principle"

    New people often expose implicit knowledge.

    Their questions should not be treated as interruptions. They are signals of where continuity may need support.

## Documentation support

| Knowledge need                                       | Useful document                                                                                                                                                                         |
| ---------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Terms are not clear to newcomers.                    | Domain Vocabulary — [Taxonomy](../../../docs-standard/taxonomy/domain-vocabulary.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/domain-vocabulary.md)       |
| The surrounding scenario needs orientation.          | Context Document — [Taxonomy](../../../docs-standard/taxonomy/context-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/context-document.md)          |
| The current work depends on workflows or handoffs.   | Process Document — [Taxonomy](../../../docs-standard/taxonomy/process-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/process-document.md)          |
| A behavior needs to clarify intent and consequences. | Use Case Document — [Taxonomy](../../../docs-standard/taxonomy/use-case-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/use-case-document.md)       |
| A stable ability explains several related changes.   | Capability Document — [Taxonomy](../../../docs-standard/taxonomy/capability-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/capability-document.md) |
| The existing direction depends on past tradeoffs.    | Decision Record — [Taxonomy](../../../docs-standard/taxonomy/decision-record.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/decision-record.md)             |
| Recent feedback changed the current understanding.   | Validation Note — [Taxonomy](../../../docs-standard/taxonomy/validation-note.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/validation-note.md)             |
| Questions or observations are still uncertain.       | Support Note — [Taxonomy](../../../docs-standard/taxonomy/support-note.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/support-note.md)                      |

Use documents to join the work, not to audit the whole project.

{% include-markdown "shared/readings/document-stage-affinity-admonition.md" %}

## Suggested approach

Start with the active work. Do not try to understand everything before contributing.

A useful approach is:

1. Identify the current work item, use case, capability, or work line.
2. Find the context and decisions that explain why it exists.
3. Understand the current stage of the iteration.
4. Clarify what is known, what is uncertain, and what has already been decided.
5. Contribute to a small part of the work.
6. Preserve missing knowledge discovered during onboarding.
7. Return feedback to the shared context.

The team should enter through continuity and then contribute through delivery.

## Common mistakes

Joining existing work often fails when execution starts before orientation.

Common mistakes include:

* starting from tickets without understanding intent
* rewriting context that already exists
* ignoring previous decisions
* treating old decisions as always correct
* treating old decisions as always wrong
* changing implementation without knowing who depends on it
* asking for complete documentation before contributing
* keeping onboarding questions private
* creating new documents that duplicate existing knowledge

Existing projects need respect and curiosity. Not blind obedience. Not heroic replacement.

## Guiding principle

!!! principle "Continuity principle"

    Join the continuity path before joining the task list.


Understand enough context, decisions, behavior, and feedback to contribute without breaking intent.

Preserve the knowledge that helped you onboard, so the next person does not have to rediscover it.
