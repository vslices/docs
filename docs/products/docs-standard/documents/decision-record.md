# Decision Record

A Decision Record preserves an important decision, the context that shaped it, and the consequences the team accepted.

Its purpose is to explain why a direction was chosen so future work can understand, review, or change that decision deliberately. A Decision Record answers:

> Why did we choose this?

A decision may be about domain language, process design, scope, architecture, implementation, validation, or documentation.

## Purpose

A Decision Record helps the team preserve:

- __decision__: the selected direction.
- __context__: the situation, constraint, risk, or need that made the decision relevant.
- __options__: alternatives the team considered.
- __rationale__: why this option was chosen.
- __tradeoffs__: what the team gained, lost, accepted, or postponed.
- __consequences__: what changes because of the decision.
- __review conditions__: when the decision should be revisited.

The goal is to preserve reasoning, not to justify decisions after the fact.

## When to use it

Use a Decision Record when a decision affects future understanding, implementation, or evolution. It is especially useful when:

- __the decision is hard to reverse__: changing it later may be expensive.
- __the decision affects several artifacts__: contexts, processes, use cases, capabilities, or implementation may depend on it.
- __tradeoffs matter__: the team accepted costs, risks, or constraints.
- __alternatives were plausible__: future readers may wonder why another option was not chosen.
- __the decision shapes boundaries__: ownership, responsibility, architecture, or scope may change.
- __the decision may be challenged later__: preserving context avoids repeating the same discussion.

## When not to use it

A Decision Record may be unnecessary when:

- __the decision is trivial__: the choice has no meaningful future impact.
- __the decision is fully reversible__: changing it later is cheap and obvious.
- __the team is only recording tasks__: implementation work does not always need a decision record.
- __the decision is still unclear__: a Support Note may be better until the options are understood.
- __the record is used as approval theater__: the document exists to look formal, not to preserve reasoning.

## Minimal version

Use the minimal version when the team only needs to preserve the core reasoning.

```md
# Decision Record

## Decision

What did we choose?

## Context

Why was this decision needed?

## Rationale

Why did we choose this direction?

## Consequences

What changes because of this decision?

## Status

Draft, active, superseded, or archived.
```

## Expanded version

Use the expanded version when the decision is risky, disputed, architectural, or likely to affect future evolution.

```md
# Decision Record

## Decision

## Status

## Context

## Problem or tension

## Options considered

## Selected option

## Rationale

## Tradeoffs

## Consequences

## Accepted risks

## Rejected alternatives

## Related artifacts

## Review conditions
```

## Related artifacts

A Decision Record may support or be supported by:

- __Context Document__: explains the scenario or constraint behind the decision.
- __Process Document__: shows process conditions that influenced the decision.
- __Use Case Document__: describes behavior affected by the decision.
- __Capability Document__: explains abilities shaped by the decision.
- __Domain Vocabulary__: preserves language decisions or naming choices.
- __Validation Note__: confirms, challenges, or updates the decision.
- __Support Note__: captures early options, risks, or assumptions before a decision is made.

## Common mistakes

Common mistakes include:

- __recording everything__: the team creates decision records for choices with no real impact.
- __writing only the final answer__: future readers cannot understand why the decision was made.
- __hiding tradeoffs__: the record pretends the chosen option had no cost.
- __ignoring rejected options__: the same alternatives are debated again later.
- __using decisions as authority__: the record becomes a way to stop discussion instead of preserve reasoning.
- __not reviewing old decisions__: changed context invalidates the decision, but the record remains active.

## Example questions

A Decision Record should help answer:

- What did we decide?
- Why was this decision needed?
- What alternatives were considered?
- Why was this option chosen?
- What tradeoffs did we accept?
- What risks did we knowingly keep?
- What artifacts or implementation choices depend on this decision?
- When should this decision be reviewed?

## Continuity

A Decision Record preserves continuity between reasoning and future change.

```text
context or problem
-> options and tradeoffs
-> selected decision
-> affected artifacts
-> implementation consequences
-> validation and evolution
```

When decisions remain explicit, the team can evolve the system without losing the reasoning that shaped it.
