# Learning Loop

The Learning Loop explains how feedback from real work returns to understanding. In VSlices Method, building something is not the end of an iteration. Building creates evidence.

That evidence may confirm the current direction, refine the context, challenge a decision, or reveal a new work line.

## Core idea

A VSlices Method iteration follows the shared VSlices Design flow:

{% include-markdown "shared/simple-design-iteration-flow.md" %}

The final return to **Understanding** is intentional.

A team does not return to Understanding because the iteration failed. A team returns because building, validating, and using software changes what is known.

The result of an iteration should not only be working software. It should also be better understanding.

## What can create learning

Learning may come from different sources.

* implementation, when technical constraints reveal hidden assumptions
* review, when the expected behavior is questioned
* testing, when expected errors or edge cases become visible
* usage, when people interact with the system differently than expected
* operation, when production behavior exposes new risks
* support, when repeated issues reveal unclear workflows or concepts
* business feedback, when the delivered behavior changes priorities

The important part is not where feedback comes from. The important part is whether it changes what the team should understand, preserve, or do next.

## Learning outcomes

After Building, feedback may produce different outcomes.

| Outcome | Means that... |
| --- | --- |
| **Confirmed** | The evidence supports the current understanding or decision. |
| **Refined** | The direction was useful, but some details need adjustment. |
| **Challenged** | The evidence contradicts an assumption, decision, or model. |
| **Split** | The feedback reveals a separate work line or concern. |
| **Superseded** | Previous knowledge no longer represents the current reality. |

Each outcome should influence what happens next:

* A confirmed result may allow the team to continue.
* A refined result may update a document or implementation detail.
* A challenged result may require returning to Planning or Contextualizing.
* A split result may open a new Work Line.
* A superseded result may require updating or replacing previous knowledge.

## What should be preserved

The Learning Loop does not require every feedback signal to become documentation. Preserve feedback when it affects future work.

Useful knowledge to preserve may include:

* a decision that was confirmed or challenged
* a behavior that worked differently than expected
* a missing expected error
* a workflow exception that became visible
* a domain term whose meaning changed
* a technical constraint that affects design
* a new risk discovered during implementation or operation
* a possible new Work Line

The goal is not to record everything. It is to avoid rediscovering the same learning later.

## Document support

Different documents may support the Learning Loop.

| Document | Can preserve |
| --- | --- |
| [Validation Notes](../../docs-standard/taxonomy/validation-note.md) | Evidence and learning. |
| [Decision Records](../../docs-standard/taxonomy/decision-record.md) | Decisions that were confirmed, challenged, or changed. |
| [Use Case Documents](../../docs-standard/taxonomy/use-case-document.md) | Behavior that became clearer after building. |
| [Capability Documents](../../docs-standard/taxonomy/capability-document.md) | Stable abilities revealed or refined by the iteration. |
| [Context Documents](../../docs-standard/taxonomy/context-document.md) | Changes in the surrounding scenario. |
| [Process Documents](../../docs-standard/taxonomy/process-document.md) | Workflow changes, exceptions, or handoffs. |
| [Support Notes](../../docs-standard/taxonomy/support-note.md) | Uncertain or local observations that are not mature yet. |

Use the lightest document that preserves the learning future work depends on.

## Deciding the next move

After learning is gathered, the team should decide what the next responsible move is. Possible moves include:

* continuing the current direction
* updating existing documentation
* recording a Validation Note
* reviewing a Decision Record
* refining the current Use Case or Capability
* returning to Contextualizing
* returning to Planning
* switching design modality
* opening a new Work Line
* stopping the iteration because enough value was delivered

The next move should be based on what the evidence changed.

## Common risks

Learning loops can break in several ways.

* **Feedback without preservation**: makes teams repeat the same discoveries.
* **Validation without decisions**: creates observations that never affect direction.
* **Implementation without reflection**: treats building as completion instead of learning.
* **Documentation without update**: leaves stale knowledge active.
* **Success without review**: misses what should be reused or strengthened.
* **Failure without learning**: turns evidence into blame instead of understanding.

The Learning Loop exists to make feedback useful before it disappears.

## Guiding principle

!!! principle "Learning principle"

    Reality is part of the method.

Use feedback to improve the shared understanding of the work. Preserve only the learning that future decisions, documentation, design, or implementation may depend on.
