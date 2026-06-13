# "Joining Existing Project" Scenario

A "Joining existing project" scenario is a working context where a person or team enters work that is already in progress. The project may already use VSlices Method, or it may use another way of working.

The goal is not to restart the project. It is to join the current continuity path before changing the work.

## Core idea

Joining an existing project should not start only from tasks. Tasks describe what someone should do. But, they do not always explain:

- Why the work matters
- What context supports it
- What decisions shaped it
- What feedback changed it

The question is not _What tasks should we take?_, it is: __What continuity path are these tasks part of?__.

## When this guide applies

Use this guide when:

* a new person joins a project
* a new team joins an ongoing initiative
* work is already planned or in progress
* existing decisions affect the current work
* documentation exists but needs interpretation
* implementation exists but intent is unclear
* the project has active stakeholders, users or operational constraints
* the team needs to contribute without losing the original context

This guide applies whether the project is new to the person or new to the whole team.

## Main risk

The main risk is entering through execution without understanding intent. This may create:

* changes that solve a task but not the problem
* duplicated discovery
* repeated decisions
* implementation that violates previous context
* documentation that ignores existing knowledge
* feedback that is disconnected from current work
* local improvements that weaken the whole system

A project in progress already has history, some of that history is useful knowledge, some of it may be outdated or accidental.

The team should understand enough to tell the difference.

## Useful starting modality

Joining an existing project does not always require choosing a new modality. First, identify the current work context.

| Situation                                                                            | Useful modality               | Reason                                                                     |
| ------------------------------------------------------------------------------------ | ----------------------------- | -------------------------------------------------------------------------- |
| The project context, boundaries<br/>or history are unclear.                              | [**Context-First**](../../design/modalities/context-first/index.md)             | The team needs to understand the<br/>surrounding continuity before acting.     |
| The current work is centered<br/>on a known pain or active decision.                     | [**Problem-First**](../../design/modalities/problem-first/index.md)             | The team needs to understand the<br/>problem behind the tasks.                 |
| The project has enough context<br/>and a small contribution can safely<br/>produce feedback. | [**Slice-First**](../../design/modalities/slice-first/index.md)               | The team can learn by contributing<br/>a narrow change.                        |
| The project already has an active<br/> modality.                                          | Continue the<br/> current modality | The team should join the current<br/>continuity path before changing<br/>emphasis. |

The first responsibility is orientation. Changing modality too early may restart work unnecessarily.

## What to observe first

Before contributing, observe how current work is connected. Useful questions include:

* What scenario or work line is active?
* What problem or opportunity is being addressed?
* What decisions already shape the current direction?
* What documents or discussions preserve the current context?
* What implementation already exists?
* What feedback has recently changed the work?
* What remains uncertain?
* Who depends on the current behavior?
* Which constraints are technical, business or operational?
* Which parts of the work are still being validated?

The objective is not to learn the whole project. Is to understand the continuity path of the work being joined.

## Knowledge to preserve

Joining an existing project may reveal missing or fragile continuity. 

Preserve knowledge when it helps new contributors or future work avoid guessing. Useful knowledge may include:

* project vocabulary that is not obvious
* decisions that explain current implementation
* active assumptions
* known constraints
* current workflow or use case boundaries
* validation results that shaped the current direction
* differences between documented intent and actual implementation
* onboarding questions that reveal hidden knowledge
* outdated knowledge that should be reviewed

Newcomers often expose implicit knowledge. Those questions should not be treated as interruptions. They are signals of __where continuity may need support__.

## Document support

| Knowledge need                                      | Useful document                                                                                                                                                                         |
| --------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Terms are unclear to newcomers.                     | Domain Vocabulary — [Taxonomy](../../docs-standard/taxonomy/domain-vocabulary.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/domain-vocabulary.md)       |
| The surrounding scenario needs orientation.         | Context Document — [Taxonomy](../../docs-standard/taxonomy/context-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/context-document.md)          |
| Current work depends on workflows or handoffs.      | Process Document — [Taxonomy](../../docs-standard/taxonomy/process-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/process-document.md)          |
| A behavior needs intent and consequences clarified. | Use Case Document — [Taxonomy](../../docs-standard/taxonomy/use-case-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/use-case-document.md)       |
| A stable ability explains several related changes.  | Capability Document — [Taxonomy](../../docs-standard/taxonomy/capability-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/capability-document.md) |
| Existing direction depends on past tradeoffs.       | Decision Record — [Taxonomy](../../docs-standard/taxonomy/decision-record.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/decision-record.md)             |
| Recent feedback changed current understanding.      | Validation Note — [Taxonomy](../../docs-standard/taxonomy/validation-note.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/validation-note.md)             |
| Questions or observations are still uncertain.      | Support Note — [Taxonomy](../../docs-standard/taxonomy/support-note.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/support-note.md)                      |

Use documents to join the work, not to audit the whole project.

> Document affinity by iteration stage is described in the [Document-Stage affinity](../document-stage-affinity.md) page.

## Suggested approach

Start with the active work. Do not try to understand everything before contributing. A useful approach is:

1. Identify the current work item, use case, capability or work line.
2. Find the context and decisions that explain why it exists.
3. Understand the current stage of the iteration.
4. Clarify what is known, uncertain and already decided.
5. Contribute to a small part of the work.
6. Preserve any missing knowledge discovered while joining.
7. Return feedback to the shared context.

The team should enter through continuity, then contribute through delivery.

## Common mistakes

Joining existing work commonly fails when execution starts before orientation. Common mistakes include:

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

Join the continuity path before joining the task list. Understand enough context, decisions, behavior and feedback to contribute without breaking intent.

Preserve the knowledge that helped you join, so the next person does not need to rediscover it.
