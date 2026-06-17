# Document Stage Affinity

Document Stage Affinity explains how VSlices Docs Standard documents may support each stage of a VSlices Design iteration.

It does not make documents mandatory. It helps teams choose useful documentation without turning VSlices Method into a checklist.

The shared iteration flow is:

{% include-markdown "shared/simple-design-iteration-flow.md" %}

## Core idea

Each stage creates or changes a different kind of knowledge. Some documents naturally support some stages better than others.

This affinity is only a guide. A team may create, update, skip, merge or revisit documents whenever the iteration requires it.

The question is not "*Which documents does this stage require?*", it is: "**What knowledge do we need to preserve to make the next responsible decision?**".

## Stage affinity

| Stage                          | Knowledge being handled                                                                   | Useful documents                                                                                                               | Main risk avoided                                                                 |
| ------------------------------ | ----------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------- |
| **Understanding**              | Early domain signals, language, assumptions, risks and open questions.                    | **[Domain Vocabulary](../docs-standard/taxonomy/domain-vocabulary.md)**, **[Support Note](../docs-standard/taxonomy/support-note.md)**, early **[Context Document](../docs-standard/taxonomy/context-document.md)**.                                                           | Designing software artifacts before understanding the world they belong to.       |
| **Contextualizing**            | Scenario, actors, boundaries, work lines, workflows and surrounding context.              | **[Context Document](../docs-standard/taxonomy/context-document.md)**, **[Process Document](../docs-standard/taxonomy/process-document.md)**, **[Domain Vocabulary](../docs-standard/taxonomy/domain-vocabulary.md)**, **[Support Note](../docs-standard/taxonomy/support-note.md)**.                                           | Treating a problem, use case or feature as isolated from its context.             |
| **Planning**                   | Intended improvement, behavior, capabilities, scope, decisions and tradeoffs.             | **[Use Case Document](../docs-standard/taxonomy/use-case-document.md)**, **[Capability Document](../docs-standard/taxonomy/capability-document.md)**, **[Decision Record](../docs-standard/taxonomy/decision-record.md)**, **[Support Note](../docs-standard/taxonomy/support-note.md)**.                                         | Solving an attractive technical problem instead of the relevant business problem. |
| **Building**                   | Implementation behavior, validations, expected errors, constraints and delivery feedback. | **[Use Case Document](../docs-standard/taxonomy/use-case-document.md)**, **[Capability Document](../docs-standard/taxonomy/capability-document.md)**, **[Decision Record](../docs-standard/taxonomy/decision-record.md)**, **[Validation Note](../docs-standard/taxonomy/validation-note.md)**, **[Support Note](../docs-standard/taxonomy/support-note.md)**.                    | Treating implementation as the end of learning.                                   |
| **Returning to Understanding** | Evidence, learning, changed assumptions, updated context and new uncertainty.             | **[Validation Note](../docs-standard/taxonomy/validation-note.md)**, **[Context Document](../docs-standard/taxonomy/context-document.md)**, **[Process Document](../docs-standard/taxonomy/process-document.md)**, **[Use Case Document](../docs-standard/taxonomy/use-case-document.md)**, **[Decision Record](../docs-standard/taxonomy/decision-record.md)**, **[Support Note](../docs-standard/taxonomy/support-note.md)**. | Ignoring what the system taught after being built.                                |

## Affinity by document

The same document may support more than one stage.

| Document                | Strongest affinity                       | Useful when                                                                           |
| ----------------------- | ---------------------------------------- | ------------------------------------------------------------------------------------- |
| [**Domain Vocabulary**](../docs-standard/taxonomy/domain-vocabulary.md)   | Understanding and Contextualizing.       | Language appears, changes, conflicts or becomes important for decisions.              |
| [**Context Document**](../docs-standard/taxonomy/context-document.md)    | Contextualizing.                         | The team needs to preserve the scenario, actors, boundaries or current situation.     |
| [**Process Document**](../docs-standard/taxonomy/process-document.md)    | Contextualizing.                         | Work depends on responsibilities, workflows, handoffs or repeated operations.         |
| [**Use Case Document**](../docs-standard/taxonomy/use-case-document.md)   | Planning and Building.                   | Behavior, consequences, validations or expected errors need to guide implementation.  |
| [**Capability Document**](../docs-standard/taxonomy/capability-document.md) | Planning and Building.                   | A stable business or system ability needs to be named and preserved.                  |
| [**Decision Record**](../docs-standard/taxonomy/decision-record.md)     | Planning and Building.                   | A direction, tradeoff, accepted risk or rejected option may affect future work.       |
| [**Validation Note**](../docs-standard/taxonomy/validation-note.md)     | Building and Returning to Understanding. | Evidence from implementation, review, usage or operation changes what the team knows. |
| [**Support Note**](../docs-standard/taxonomy/support-note.md)        | All stages.                              | Knowledge is useful but still early, local, uncertain or temporary.                   |

## Using affinity

Document affinity should help the team decide what to preserve. It should not decide for the team. Use a document when it helps the team:

* clarify language
* preserve context
* explain behavior
* make a decision visible
* carry intent into implementation
* record evidence
* avoid rediscovering the same knowledge later

Skip a document when it only exists because a stage seems to expect it.

## Method rule

Use the document that preserves the knowledge needed for the next responsible decision.

- If a document helps the team move with more clarity, use it.
- If a document creates ceremony without preserving useful knowledge, skip it.
