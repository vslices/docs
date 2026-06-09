# Validation Note

> You can access the [validation note template here](https://github.com/vslices/docs-standard/blob/main/templates/validation-note.md)

A Validation Note preserves evidence gathered after testing, building, reviewing, observing, or using something.

Its purpose is to capture what was confirmed, rejected, changed, or learned so future work can start from better understanding. A Validation Note answers:

> What did we learn?

Validation is not only testing. It may come from implementation feedback, user feedback, domain expert review, production behavior, experiments, prototypes, or operational observation.

## Purpose

A Validation Note helps the team preserve:

- __validation target__: what was being validated.
- __evidence__: what was observed, tested, reviewed, or measured.
- __result__: what was confirmed, rejected, or changed.
- __learning__: what the team understands better now.
- __impact__: which documents, decisions, behaviors, or implementations should change.
- __remaining uncertainty__: what still needs more evidence.
- __next action__: what should happen after the validation.

The goal is to prevent learning from disappearing after implementation or review.

## When to use it

Use a Validation Note when evidence changes or confirms knowledge that future work depends on. It is especially useful when:

- __an assumption was tested__: the team needs to record whether it survived.
- __a behavior was validated__: a use case, feature, or workflow was checked against reality.
- __implementation revealed constraints__: building exposed technical, operational, or domain limits.
- __feedback changed understanding__: users, stakeholders, or domain experts clarified something important.
- __a decision needs review__: evidence confirms, challenges, or invalidates a previous decision.
- __production behavior teaches something__: real usage reveals patterns, problems, or opportunities.

## When not to use it

A Validation Note may be unnecessary when:

- __nothing meaningful changed__: the result does not affect future understanding or decisions.
- __the evidence is too weak__: a Support Note may be better until more evidence exists.
- __the result is only task completion__: finishing work is not the same as learning from it.
- __the validation belongs elsewhere__: detailed test cases, metrics, or incidents may need their own format.
- __the note would repeat existing documentation__: update the related document instead.

## Minimal version

Use the minimal version when the team needs to preserve a small but useful learning result.

```md
# Validation Note

## Validation target

What was being validated?

## Evidence

What was observed, tested, reviewed, or measured?

## Result

What was confirmed, rejected, or changed?

## Learning

What do we understand better now?

## Impact

Which documents, decisions, behaviors, or implementations are affected?

## Next action

What should happen next?
```

## Expanded version

Use the expanded version when validation affects important decisions, risky assumptions, or future evolution.

```md 
# Validation Note

## Validation target

## Related assumption, decision, use case, or capability

## Validation method

## Evidence

## Result

## Learning

## Impact on documentation

## Impact on implementation

## Impact on decisions

## Remaining uncertainty

## Risks discovered

## Next action

## Related artifacts
```

## Standard affinity

This document can support alignment with existing standards and documentation practices. It does not make the documentation compliant by itself.

| Standard or practice | Affinity | Supports | Missing for stricter alignment |
| -------------------- | -------- | -------- | ------------------------------ |
| ISO/IEC/IEEE 29148 | High | Validation, evidence, assumptions, feedback, impact, and traceability. | Formal verification plan, requirement verification method, audit-grade evidence controls, and requirements management workflow. |
| ADR | Medium | Reviewing whether previous decisions were confirmed, challenged, or superseded. | Formal architecture decision lifecycle and governance process. |
| ISO/IEC/IEEE 42010 | Medium | Rationale updates, architecture learning, and relationships between evidence and decisions. | Formal architecture description, viewpoints, views, and correspondence rules. |
| arc42 | Medium | Risks, decisions, quality feedback, and evolution notes. | Complete arc42 structure and formal quality scenario integration. |
| 4+1 View Model | Low / Medium | Scenario feedback and behavior validation. | Complete architecture view model and view-specific validation structure. |
| C4 Model | Low | Feedback that may affect boundaries or architecture diagrams. | Diagram notation and visual hierarchy. |

## Related artifacts

A Validation Note may support or be supported by:

- __Context Document__: updates the scenario after new evidence appears.
- __Process Document__: confirms or challenges how work is actually performed.
- __Use Case Document__: validates expected behavior, consequence, errors, or rules.
- __Capability Document__: confirms whether an ability supports real needs.
- __Decision Record__: validates, challenges, or supersedes a decision.
- __Domain Vocabulary__: updates terms when evidence clarifies language.
- __Support Note__: captures early feedback before it becomes validated learning.

## Common mistakes

Common mistakes include:

- __treating delivery as validation__: something working technically does not prove it solved the right problem.
- __recording conclusions without evidence__: future readers cannot understand why the result is trusted.
- __ignoring negative results__: failed assumptions are valuable learning.
- __not updating related artifacts__: the note captures learning, but documentation and implementation stay unchanged.
- __hiding uncertainty__: the team treats partial evidence as final truth.
- __over-documenting routine tests__: not every test result needs a validation note.

## Example questions

A Validation Note should help answer:

- What was validated?
- What evidence was gathered?
- What was confirmed, rejected, or changed?
- What did we learn?
- Which assumption, decision, behavior, or capability is affected?
- What remains uncertain?
- What should change next?
- Should the next iteration continue, adjust, or switch direction?

## Continuity

A Validation Note preserves continuity between delivery and renewed understanding.

```text
implementation or review
-> evidence
-> learning
-> updated documents and decisions
-> next implementation
-> evolution
```

When validation remains explicit, the team is less likely to repeat wrong assumptions or ignore what the system taught after being built.
