# Use Case Document

> You can access the [use case document template here](https://github.com/vslices/docs-standard/blob/main/templates/use-case-document.md)

A Use Case Document preserves the meaning of a behavior inside a domain context.

Its purpose is to describe what an interaction, operation, or expected behavior means, what consequence it produces, and what must be valid for that behavior to make sense. A Use Case Document answers:

> What does this behavior mean?

A use case is not only a sequence of steps. It explains the expected outcome, business rules, validations, consequences, and relevant errors around a behavior.

## Purpose

A Use Case Document helps the team preserve:

- __domain meaning__: why this behavior matters inside the domain.
- __actor intention__: who needs the behavior and what they are trying to achieve.
- __expected consequence__: what should change after the behavior succeeds.
- __validations__: what must be true before or during the behavior.
- __business rules__: conditions that shape what is allowed or denied.
- __expected errors__: known failure cases that belong to the domain.
- __related context__: scenario, process, workflow, or capability that gives meaning to the behavior.

The goal is to make expected behavior explicit before or during implementation.

## When to use it

Use a Use Case Document when behavior needs enough clarity to guide design, implementation, or validation.

It is especially useful when:

- __the behavior has domain meaning__: the action changes something important in the business.
- __validations matter__: the system must reject or allow behavior based on explicit rules.
- __consequences matter__: success changes state, responsibility, availability, commitment, or visibility.
- __errors are expected__: some failures are part of the domain and should be modeled explicitly.
- __implementation needs guidance__: developers need more than a feature name or short task.
- __validation needs clarity__: the team needs to know what proves the behavior works.

## When not to use it

A Use Case Document may be unnecessary when:

- __the behavior is trivial__: the expected outcome is obvious and low-risk.
- __the context is still unclear__: a Context Document or Process Document may be needed first.
- __only a process needs explanation__: the team is trying to describe how work is performed.
- __only a technical task exists__: the work has no meaningful domain behavior yet.
- __a support note is enough__: the behavior is still early, uncertain, or exploratory.

## Minimal version

Use the minimal version when the team needs a lightweight behavior definition.

```md
# Use Case Document

## Use case

What behavior is being described?

## Meaning

What does this behavior mean in the domain?

## Actor

Who needs or triggers this behavior?

## Expected consequence

What changes if this succeeds?

## Validations

What must be true?

## Expected errors

What can fail in a known domain-relevant way?

## Related artifacts

Which scenario, process, workflow, capability, or decision supports this use case?
```

## Expanded version

Use the expanded version when behavior is complex, risky, rule-heavy, or implementation-critical.

```md
# Use Case Document

## Use case

## Meaning

## Actor or trigger

## Related scenario

## Related process or workflow

## Preconditions

## Expected consequence

## Main behavior

## Alternative behavior

## Validations

## Business rules

## Expected errors

## Postconditions

## Inputs

## Outputs

## Related capabilities

## Related decisions

## Validation notes
```

## Related artifacts

A Use Case Document may support or be supported by:

- __Context Document__: explains the scenario where the behavior matters.
- __Process Document__: explains the process or workflow where the behavior appears.
- __Domain Vocabulary__: preserves terms needed to understand the behavior.
- __Capability Document__: identifies stable abilities required by the use case.
- __Decision Record__: explains choices made because of behavior, rules, or tradeoffs.
- __Validation Note__: captures evidence about whether the behavior worked as expected.
- __Support Note__: captures uncertain rules, examples, errors, or assumptions.

## Common mistakes

Common mistakes include:

- __describing only steps__: the document misses consequence, validation, and meaning.
- __writing technical tasks as use cases__: the behavior has no visible domain purpose.
- __ignoring expected errors__: domain failures become hidden exceptions or ad-hoc logic.
- __hiding validations__: rules remain implicit until implementation.
- __forgetting the actor intention__: the document says what happens, but not why it matters.
- __mixing process with use case__: the document explains the whole way of working instead of one meaningful behavior.
- __treating success as obvious__: the expected consequence is never made explicit.

## Example questions

A Use Case Document should help answer:

- What behavior are we describing?
- What does this behavior mean in the domain?
- Who needs, triggers, or benefits from it?
- What should change when it succeeds?
- What must be valid before or during execution?
- What expected errors can happen?
- Which business rules shape the behavior?
- Which capability, process, or decision depends on this use case?

## Continuity

A Use Case Document preserves continuity between domain behavior and implementation behavior.

```text
scenario or process
-> meaningful behavior
-> validations and consequences
-> capabilities and decisions
-> implementation and tests
-> validation and evolution
```

When use cases remain explicit, the team is less likely to implement actions that work technically but fail to represent the domain correctly.
