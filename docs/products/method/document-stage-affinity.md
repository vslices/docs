# Document Stage Affinity

VSlices Method uses document stage affinity to explain which VSlices Docs Standard documents may support each stage of a VSlices Design iteration.

This document does not make documents mandatory. It only explains where each document usually provides the most value inside the shared iteration flow:

```text
Understanding -> Contextualizing -> Planning -> Building -> Understanding
```

The goal is to help teams choose useful documentation without turning the method into a checklist.

## Core idea

Each stage creates, organizes, decides, builds, or validates a different kind of knowledge. Some documents naturally fit better in some stages. 

This affinity is only a guide, because the team may create, update, skip, merge, or revisit documents whenever the iteration requires it.

## Understanding Stage

Understanding is where the team discovers domain knowledge. Useful documents and notes may include:

- __Domain Vocabulary__: preserves important domain language discovered during exploration.
- __Support Note__: captures early concepts, assumptions, risks, open questions, or feedback.
- __Context Document__: may start when the team begins to see where the work is happening.

The main risk avoided is designing software artifacts before understanding the world they belong to.

## Contextualizing Stage

Contextualizing is where the team organizes discovered knowledge into a visible base scenario. Useful documents and notes may include:

- __Context Document__: preserves the scenario, work lines, actors, boundaries, and current situation.
- __Process Document__: explains how a work line operates through responsibilities and workflows.
- __Domain Vocabulary__: clarifies terms that appear inside the scenario or process.
- __Support Note__: captures unclear boundaries, assumptions, risks, or unresolved questions.

The main risk avoided is treating a problem, use case, or feature as isolated when it belongs to a larger context.

## Planning Stage

Planning is where the team decides what should improve and why. Useful documents and notes may include:

- __Use Case Document__: defines the meaning, consequence, validations, and expected errors of behavior.
- __Capability Document__: identifies stable abilities required by the business or system.
- __Decision Record__: preserves selected directions, tradeoffs, accepted risks, and rejected options.
- __Support Note__: captures scope notes, risk notes, improvement notes, and open questions.

The main risk avoided is solving an attractive technical problem instead of the relevant business problem.

## Building Stage

Building is where the planned improvement becomes real through implementation, integration, validation, delivery, and feedback. Useful documents and notes may include:

- __Use Case Document__: guides implementation behavior, validations, expected errors, and tests.
- __Capability Document__: guides implementation boundaries and required abilities.
- __Decision Record__: keeps implementation aligned with selected tradeoffs.
- __Validation Note__: captures what was confirmed, rejected, changed, or learned.
- __Support Note__: captures implementation notes, discovered constraints, feedback, or next-iteration notes.

The main risk avoided is treating implementation as the end of learning.

## Returning to Understanding Stage

After Building, the team returns to Understanding because delivery creates new knowledge. Useful documents and notes may include:

- __Validation Note__: preserves evidence and learning from implementation, review, usage, or production behavior.
- __Context Document__: updates the scenario when real feedback changes understanding.
- __Process Document__: updates the process when work changed or was misunderstood.
- __Use Case Document__: updates behavior when validations, consequences, or errors change.
- __Decision Record__: supersedes or reviews decisions challenged by new evidence.
- __Support Note__: captures new questions, risks, observations, or improvement ideas.

The main risk avoided is ignoring what the system taught after being built.

## Affinity by document

The same document may appear in more than one stage.

- __Domain Vocabulary__: strongest in Understanding and Contextualizing, but useful whenever language changes.
- __Context Document__: strongest in Contextualizing, but may start during Understanding and evolve after Building.
- __Process Document__: strongest in Contextualizing, but may guide Planning and be updated after validation.
- __Use Case Document__: strongest in Planning and Building, but depends on enough context to have meaning.
- __Capability Document__: strongest in Planning, but may guide Building and future architecture.
- __Decision Record__: strongest in Planning and Building, but may be reviewed after validation.
- __Validation Note__: strongest in Building and the return to Understanding.
- __Support Note__: useful across all stages because early knowledge can appear anywhere.

## Method rule

Document stage affinity follows one rule: __Use the document that preserves the knowledge needed for the next responsible decision__.

- If a document helps the team move with more clarity, use it.
- If a document only exists because a stage seems to require it, skip it.

VSlices Method should guide documentation choices. It should not turn them into ceremony.
