# Modality Switching

Modality Switching explains when and why a team may move from one VSlices Design modality to another.

A modality is not a permanent label for an iteration. It is an emphasis that helps the team reduce the uncertainty that matters most right now.

When the uncertainty changes, the modality may need to change too.

## Core idea

Switch modality when the current modality is no longer reducing the dominant uncertainty. 

The question is not: _Are we allowed to change modality?_, it is _Has the kind of uncertainty changed?_.

VSlices Method uses modality switching to keep the team aligned with reality instead of forcing work to continue under the wrong emphasis.

## Why switching matters

Each modality protects the team from a different risk.

| Modality          | Helps avoid                                      | Can become risky when                                                         |
| ----------------- | ------------------------------------------------ | ----------------------------------------------------------------------------- |
| __[Context-First](../../design/modalities/context-first/index.md)__ | Building from misunderstood<br/>context.             | The team keeps expanding understanding without<br/>deciding what to validate.     |
| __[Problem-First](../../design/modalities/problem-first/index.md)__ | Solving symptoms instead of<br/>problems.            | The team isolates the problem from the wider<br/>context that gives it meaning.   |
| __[Slice-First](../../design/modalities/slice-first/index.md)__   | Designing too much before<br/>learning from reality. | The team builds without enough understanding of<br/>intent, risk or consequences. |

Switching modality helps avoid turning a useful emphasis into accidental complexity.

## Common switches

A switch does not mean the previous modality was wrong. It means the previous modality produced enough learning for the work to need a different emphasis.

| Switch                             | Use when                                                                                               | Purpose                                                   |
| ---------------------------------- | ------------------------------------------------------------------------------------------------------ | --------------------------------------------------------- |
| __[Context-First](../../design/modalities/context-first/index.md)__ -> __[Problem-First](../../design/modalities/problem-first/index.md)__ | The team understands enough<br/>of the scenario to focus on a<br/>concrete pain, opportunity or<br/>decision.      | Narrow broad context into a<br/>problem worth solving.        |
| __[Context-First](../../design/modalities/context-first/index.md)__ -> __[Slice-First](../../design/modalities/slice-first/index.md)__   | The team understands enough<br/>to validate a small and reversible<br/>part of the system.                     | Turn contextual learning into<br/>practical evidence.         |
| __[Problem-First](../../design/modalities/problem-first/index.md)__ -> __[Context-First](../../design/modalities/context-first/index.md)__ | The problem depends on<br/>surrounding workflows, actors,<br/>language or constraints that<br/>are still unclear.  | Recover the context needed to<br/>avoid local optimization.   |
| __[Problem-First](../../design/modalities/problem-first/index.md)__ -> __[Slice-First](../../design/modalities/slice-first/index.md)__   | The problem is clear enough<br/>that a small delivery can test<br/>theintended improvement.                   | Validate whether the proposed<br/>direction works in reality. |
| __[Slice-First](../../design/modalities/slice-first/index.md)__ -> __[Problem-First](../../design/modalities/problem-first/index.md)__   | A built slice reveals that the<br/>original problem was<br/>incomplete, misplaced or<br/>poorly framed.            | Reframe the problem using<br/>evidence from delivery.         |
| __[Slice-First](../../design/modalities/slice-first/index.md)__ -> __[Context-First](../../design/modalities/context-first/index.md)__   | Building reveals missing<br/>domain context, hidden actors,<br/>unclear boundaries or<br/>unexpected consequences. | Rebuild understanding before<br/>continuing implementation.   |

## Signals that switching may be needed

A team should consider switching modality when the current mode stops helping. Common signals include:

* new domain concepts appear during implementation
* the team keeps debating without learning anything new
* a small slice works technically but does not improve the real situation
* a problem seems clear but depends on workflows nobody understands
* documentation keeps expanding but no decision becomes safer
* delivery feedback contradicts an assumption
* the same question keeps returning across stages
* the team cannot explain why the current work matters

These signals do not automatically require a switch. They indicate that the team should re-evaluate the dominant uncertainty.

## Switching without ceremony

Modality switching should be lightweight.

- A team does not need to restart the iteration.
- A team only needs to acknowledge what changed.

Useful questions include:

* What did we learn?
* What uncertainty is now dominant?
* Is our current modality still helping?
* What is the smallest next move that reduces this uncertainty?
* What knowledge should be preserved before moving on?

The switch may be as simple as changing the next conversation, updating a document, narrowing the next slice or reopening a decision.

## Document support

Documents may help preserve why a modality changed. Use documentation only when the switch affects future work.

* **[Support Notes](../../docs-standard/taxonomy/support-note.md)** can preserve early observations or uncertainty.
* **[Validation Notes](../../docs-standard/taxonomy/validation-note.md)** can preserve evidence that caused the switch.
* **[Decision Records](../../docs-standard/taxonomy/decision-record.md)** can preserve important direction changes.
* **[Context Documents](../../docs-standard/taxonomy/context-document.md)** can preserve newly discovered surrounding context.
* **[Use Case Documents](../../docs-standard/taxonomy/use-case-document.md)** can preserve behavior clarified after switching.
* **[Process Documents](../../docs-standard/taxonomy/process-document.md)** can preserve workflow knowledge revealed by the switch.

The goal is not to document every switch. It is to avoid losing the learning that made the switch necessary.

## Common mistakes

Modality switching can fail when the team treats modalities as process stages.

* Switching too often may prevent useful depth.
* Refusing to switch may keep the team solving the wrong uncertainty.
* Switching without preserving learning may make the team repeat the same confusion.
* Treating switches as failure may discourage feedback.
* Treating switches as mandatory stages may create unnecessary ceremony.

A switch is useful when it makes the next decision safer.

## Guiding principle

Let the current uncertainty choose the modality. When the uncertainty changes, change the emphasis. 

The method should follow the learning. It should not be forced to fit the method.
