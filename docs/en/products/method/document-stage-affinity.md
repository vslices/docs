# Document-stage affinity

Document-stage affinity explains how VSlices Docs Standard documents can support each stage of a VSlices Design iteration.

!!! principle "Documentation principle"

    Document-stage affinity helps choose useful documentation according to the stage of work.

    It does not turn documents into mandatory requirements or transform VSlices Method into a checklist.


This page uses the following base iteration flow:

<p class="vslices-diagram-caption">Base iteration flow used to organize document affinity.</p>

{% include-markdown "shared/simple-design-iteration-flow.md" %}

## Core idea

Each stage creates or changes a different kind of knowledge.

Some documents naturally support some stages better than others, but this affinity is only a guide. A team can create, update, omit, merge, or revisit documents when the iteration requires it.

!!! principle "Documentation principle"

    The question is not _which documents does this stage require?_, but _what knowledge do we need to preserve to make the next responsible decision?_


## Affinity by stage

| Stage                          | Knowledge being handled                                                                    | Useful documents                                                                                                                                                                                                                                                                                                                                                                                                                | Main risk it avoids                                                               |
| ------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| **Understanding**              | Early domain signals, language, assumptions, risks, and open questions.                    | **[Domain Vocabulary](../docs-standard/taxonomy/domain-vocabulary.md)**, **[Support Note](../docs-standard/taxonomy/support-note.md)**, early **[Context Document](../docs-standard/taxonomy/context-document.md)**.                                                                                                                                                                                                            | Designing software artifacts before understanding the world they belong to.       |
| **Contextualizing**            | Scenario, actors, boundaries, work lines, workflows, and surrounding context.              | **[Context Document](../docs-standard/taxonomy/context-document.md)**, **[Process Document](../docs-standard/taxonomy/process-document.md)**, **[Domain Vocabulary](../docs-standard/taxonomy/domain-vocabulary.md)**, **[Support Note](../docs-standard/taxonomy/support-note.md)**.                                                                                                                                           | Treating a problem, use case, or feature as if it were isolated from its context. |
| **Planning**                   | Expected improvement, behavior, capabilities, scope, decisions, and tradeoffs.             | **[Use Case Document](../docs-standard/taxonomy/use-case-document.md)**, **[Capability Document](../docs-standard/taxonomy/capability-document.md)**, **[Decision Record](../docs-standard/taxonomy/decision-record.md)**, **[Support Note](../docs-standard/taxonomy/support-note.md)**.                                                                                                                                       | Solving an attractive technical problem instead of the relevant business problem. |
| **Building**                   | Implementation behavior, validations, expected errors, constraints, and delivery feedback. | **[Use Case Document](../docs-standard/taxonomy/use-case-document.md)**, **[Capability Document](../docs-standard/taxonomy/capability-document.md)**, **[Decision Record](../docs-standard/taxonomy/decision-record.md)**, **[Validation Note](../docs-standard/taxonomy/validation-note.md)**, **[Support Note](../docs-standard/taxonomy/support-note.md)**.                                                                  | Treating implementation as the end of learning.                                   |
| **Returning to Understanding** | Evidence, learning, changed assumptions, updated context, and new uncertainty.             | **[Validation Note](../docs-standard/taxonomy/validation-note.md)**, **[Context Document](../docs-standard/taxonomy/context-document.md)**, **[Process Document](../docs-standard/taxonomy/process-document.md)**, **[Use Case Document](../docs-standard/taxonomy/use-case-document.md)**, **[Decision Record](../docs-standard/taxonomy/decision-record.md)**, **[Support Note](../docs-standard/taxonomy/support-note.md)**. | Ignoring what the system taught after being built.                                |

## Affinity by document

The same document can support more than one stage.

| Document                                                                    | Strongest affinity                       | Useful when                                                                          |
| --------------------------------------------------------------------------- | ---------------------------------------- | ------------------------------------------------------------------------------------ |
| [**Domain Vocabulary**](../docs-standard/taxonomy/domain-vocabulary.md)     | Understanding and Contextualizing.       | Language appears, changes, conflicts, or becomes important for decision-making.      |
| [**Context Document**](../docs-standard/taxonomy/context-document.md)       | Contextualizing.                         | The team needs to preserve the scenario, actors, boundaries, or current situation.   |
| [**Process Document**](../docs-standard/taxonomy/process-document.md)       | Contextualizing.                         | The work depends on responsibilities, workflows, handoffs, or repeated operations.   |
| [**Use Case Document**](../docs-standard/taxonomy/use-case-document.md)     | Planning and Building.                   | Behavior, consequences, validations, or expected errors must guide implementation.   |
| [**Capability Document**](../docs-standard/taxonomy/capability-document.md) | Planning and Building.                   | A stable business or system ability needs to be named and preserved.                 |
| [**Decision Record**](../docs-standard/taxonomy/decision-record.md)         | Planning and Building.                   | A direction, tradeoff, accepted risk, or rejected option may affect future work.     |
| [**Validation Note**](../docs-standard/taxonomy/validation-note.md)         | Building and Returning to Understanding. | Evidence from implementation, review, use, or operation changes what the team knows. |
| [**Support Note**](../docs-standard/taxonomy/support-note.md)               | All stages.                              | Knowledge is useful, but still early, local, uncertain, or temporary.                |

## Using the affinity

Document affinity should help the team decide what knowledge to preserve. It should not decide for the team.

Use a document when it helps the team:

* clarify language
* preserve context
* explain behavior
* make a decision visible
* carry intent into implementation
* record evidence
* avoid rediscovering the same knowledge later

!!! risk "Risk to avoid"

    Omit a document when it exists only because a stage seems to expect it.



## Method rule

!!! principle "Use documentation only when it preserves continuity"

    Use the document that preserves the knowledge needed for the next responsible decision.


If a document helps the team move forward with more clarity, use it.

If a document creates ceremony without preserving useful knowledge, omit it.
