# Continuity Paths

VSlices Docs Standard uses continuity paths to explain how knowledge moves between documents.

A continuity path shows how one piece of knowledge can be discovered, documented, shaped into decisions, reflected in implementation, validated, and evolved.

The goal is not to force every document into a fixed sequence, the goal is to keep important knowledge connected.

## Core idea

Documentation loses value when documents become isolated.

- A Context Document may explain where the team is working.
- A Process Document may explain how work is performed.
- A Use Case Document may explain what a behavior means.
- A Capability Document may explain what must be possible.
- A Decision Record may explain why a direction was chosen.
- A Validation Note may explain what was learned.
- A continuity path connects those artifacts so future readers can understand how knowledge evolved.

## General path

A common continuity path may look like this:

```text
scenario
-> work line
-> work process
-> workflow
-> use case
-> capability
-> decision
-> implementation
-> validation
-> updated understanding
```

This path is descriptive, not mandatory. A team may start from a scenario, a problem, a workflow, a use case, a decision, or a small implementation.

What matters is that important knowledge remains traceable.

## Document contribution

Each document preserves a different part of the path:

- __Domain Vocabulary__: preserves the language needed to understand the path.
- __Context Document__: preserves the scenario and work lines where the path begins.
- __Process Document__: preserves how work is organized and performed.
- __Use Case Document__: preserves the meaning, consequence, validations, and expected errors of behavior.
- __Capability Document__: preserves stable abilities required by the business or system.
- __Decision Record__: preserves why a direction was selected and which tradeoffs were accepted.
- __Validation Note__: preserves evidence, learning, and changes after review, implementation, or usage.
- __Support Note__: preserves early or uncertain knowledge before it becomes structured.

## Example path: from scenario to behavior

A team may discover that a company has a fragmented reservation scenario.

The continuity path may become:

```text
Context Document
-> defines the reservation scenario and involved work lines.

Domain Vocabulary
-> clarifies terms like reservation, booking, cancellation, and availability.

Process Document
-> explains how reservations are currently handled.

Use Case Document
-> defines what confirming a booking means.

Capability Document
-> identifies the need to validate availability.

Decision Record
-> explains why availability validation belongs near booking confirmation.

Validation Note
-> captures whether the implemented behavior matched real operational needs.
```

The value is not the number of documents.

The value is that the behavior can be traced back to the knowledge that justified it.

## Example path: from learning to change

Continuity also moves backward.

A feature, slice, review, or production behavior may reveal that previous understanding was incomplete.

The continuity path may become:

```text
Validation Note
-> captures evidence that a rule was misunderstood.

Use Case Document
-> updates the expected behavior.

Process Document
-> updates the workflow affected by the rule.

Decision Record
-> supersedes the previous decision.

Context Document
-> updates the scenario if the learning changes the broader understanding.
```

This is why documentation should support evolution.

Implementation does not end learning.

It often creates better questions.

## Lightweight traceability

Simple references are enough.

```md
Related context:
- context.reservations

Related process:
- process.reservation-management

Related use cases:
- use-case.confirm-booking

Related capability:
- capability.validate-availability

Related decisions:
- decision.booking-validation-boundary

Related validations:
- validation.booking-feedback
```

References should help readers move through knowledge.

They should not become administrative noise.

## When to create references

Add references when they improve clarity. Useful references usually connect:

- __cause to consequence__: why a document or decision exists.
- __behavior to context__: where a use case gets its meaning.
- __decision to evidence__: what supported or challenged a choice.
- __capability to behavior__: which use cases require an ability.
- __validation to change__: what learning affected after evidence appeared.

Do not add references only because a template has a place for them.

## Continuity principle

A continuity path follows one principle: __Important knowledge should remain connected to the artifacts and decisions that depend on it__.

- If a document cannot explain what it connects to, it may be too isolated.
- If an implementation cannot be traced back to context, behavior, capability, or decision, the team may have lost intent.
- If validation does not update future understanding, the team may be ignoring what the system has taught.
