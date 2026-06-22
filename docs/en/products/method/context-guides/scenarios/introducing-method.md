# Scenario "Introducing Method"

An "Introducing Method" scenario is a work context where a team or organization does not currently use VSlices Method, but is open to improving how knowledge, decisions, implementation, and feedback stay connected.

The goal is not to adopt all of Method at once. It is to introduce one useful continuity seam.

## Core idea

!!! principle "Continuity principle"

    VSlices Method should be introduced from work that is already happening.

A team should not start by changing its whole process. It should start by preserving one piece of knowledge that current or future work depends on.

The question is not *How do we adopt VSlices Method?*, but *where is continuity being lost now?*.

## When this guide applies

Use this guide when:

* work is already happening
* the team already has a way of working
* documentation exists, but is disconnected from implementation
* decisions are made, but not preserved
* tickets describe tasks without enough intent
* feedback appears, but does not change future work
* repeated confusion appears across people or teams
* the team is open to a lightweight improvement

This guide does not aim to replace the team's way of working. It aims to make existing work more continuous.

## Main risk

The main risk is trying to introduce VSlices Method as a complete process.

That may create resistance, unnecessary ceremony, or a false sense of maturity.

A team may not need new stages, meetings, or templates. It may need a better way to preserve:

* why a change matters
* what context supports it
* what decision was made
* what remains uncertain
* what feedback changed the work
* what future work should not have to rediscover

!!! risk "Risk to avoid"

    Method should enter through usefulness, not doctrine.

If it does not improve a real decision, a real conversation, or a real change, it is probably being introduced too early or with too much weight.

## Useful initial modality

Introducing Method into an ongoing project should start from the uncertainty that is most affecting the work.

| Situation                                                                     | Useful modality                                                     | Reason                                                                            |
| ----------------------------------------------------------------------------- | ------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| The team feels repeated pain, but does not know where continuity is breaking. | [**Context-First**](../../../design/modalities/context-first/index.md) | The team needs to understand the loss of continuity before changing how it works. |
| A small artifact or practice can improve ongoing work immediately.            | [**Problem-First**](../../../design/modalities/problem-first/index.md) | The team can validate Method through a bounded and useful improvement.            |
| The surrounding work context is too uncertain to intervene safely.            | [**Slice-First**](../../../design/modalities/slice-first/index.md)     | The team needs to learn through a small intervention before expanding the change. |

!!! risk "Risk to avoid"

    The selected modality should respond to adoption uncertainty, not to the team's personal preference.


## Affinity with continuity paths

Introducing Method usually has affinity with the path where continuity is being lost most visibly.

This is not about presenting every continuity path to the team.

It is about finding a small and useful entry point.

| Continuity path | Typical affinity | Use in this context |
| --- | --- | --- |
| Business scenario | Medium | Useful when the team loses context about why the work exists or what operational reality it is trying to improve. |
| Domain context | High | Useful when language, rules, boundaries, or concepts become confused across people, documents, tickets, or code. |
| Software project | High | Useful when decisions, technical changes, or implementation boundaries become disconnected from the context that originated them. |
| Client product | Low | Useful when the team needs to connect current work with visible behavior for users or clients. |
| Consumable service | Low | Useful when continuity loss happens around APIs, integrations, dependencies between systems, or shared capabilities. |

!!! principle "Affinity principle"

    Introduce Method through the path where continuity loss most affects real work.

In this scenario, the primary path should be chosen according to the continuity seam the team needs now.

| Observed loss | Path worth prioritizing |
| --- | --- |
| The team does not understand why the current work matters. | Business scenario |
| The team uses ambiguous or inconsistent terms. | Domain context |
| Technical decisions are made, but not preserved. | Software project |
| Tickets or documents do not explain the expected visible behavior. | Client product |
| Integrations change without clarity about capabilities, contracts, or dependencies. | Consumable service |

!!! risk "Heavy adoption risk"

    If introducing Method requires explaining every path, you are probably introducing too much. Start from the seam that already hurts.
    

## What to observe first

Before suggesting Method practices, observe how work currently moves.

| Observe                                                     | To understand                                               |
| ----------------------------------------------------------- | ----------------------------------------------------------- |
| Where intent is lost                                        | Which part of the work stops explaining why it matters.     |
| Where people repeat the same explanations                   | Which knowledge depends too much on memory or conversation. |
| Where decisions are made                                    | Which moments need to preserve context.                     |
| Where decisions are forgotten                               | Which continuity is lost between decision and future work.  |
| Where documentation stops matching reality                  | Which documents need to be updated, reduced, or replaced.   |
| Where implementation loses business context                 | Which behavior needs to recover intent.                     |
| Where feedback disappears                                   | Which learning is not changing future decisions.            |
| Which handoffs create confusion                             | Where continuity breaks between people, teams, or stages.   |
| Which small improvement would help current work immediately | Where Method can enter with real usefulness and low weight. |

The goal is not to judge the team's process. It is to find a continuity gap worth improving.

## Continuity seams

A continuity seam is a small point where Method can connect knowledge that is currently disconnected.

A useful seam may consist of:

* adding context to an active work item
* recording an important decision
* clarifying an ambiguous domain term
* preserving a validation result
* connecting a use case to an implementation change
* documenting a workflow exception
* capturing uncertainty before building
* reviewing an outdated assumption after receiving feedback

!!! principle "Continuity principle"

    A seam is useful when it helps real work continue with fewer assumptions.

    It does not need to change the whole process to improve continuity.


## Documentation support

Documents can help recover continuity in a digitized scenario.

| Knowledge need                                                     | Useful document                                                                                                                                                                         |
| ------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Terms are ambiguous or inconsistent.                               | Domain Vocabulary — [Taxonomy](../../../docs-standard/taxonomy/domain-vocabulary.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/domain-vocabulary.md)       |
| The surrounding business scenario is unclear.                      | Context Document — [Taxonomy](../../../docs-standard/taxonomy/context-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/context-document.md)          |
| The current work depends on workflows or handoffs.                 | Process Document — [Taxonomy](../../../docs-standard/taxonomy/process-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/process-document.md)          |
| A specific behavior needs to be changed or preserved.              | Use Case Document — [Taxonomy](../../../docs-standard/taxonomy/use-case-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/use-case-document.md)       |
| A stable business ability is emerging.                             | Capability Document — [Taxonomy](../../../docs-standard/taxonomy/capability-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/capability-document.md) |
| A direction must be chosen under tradeoffs.                        | Decision Record — [Taxonomy](../../../docs-standard/taxonomy/decision-record.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/decision-record.md)             |
| Evidence from use, operation, or review changes the understanding. | Validation Note — [Taxonomy](../../../docs-standard/taxonomy/validation-note.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/validation-note.md)             |
| Observations are still local, uncertain, or temporary.             | Support Note — [Taxonomy](../../../docs-standard/taxonomy/support-note.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/support-note.md)                      |

Use the lightest document that protects continuity.

{% include-markdown "shared/readings/document-stage-affinity-admonition.md" %}

## Suggested approach

Start with work that is already happening. Do not stop the project to introduce Method.

A useful approach is to:

1. Choose an active work item, problem, or decision.
2. Identify where continuity is weak.
3. Add the smallest useful Method structure.
4. Use it during real work.
5. Observe whether it helps people make better decisions.
6. Preserve the learning.
7. Decide whether another continuity seam is worth introducing.

Method should grow only where it keeps proving useful.

## Common mistakes

Introducing Method can fail when the method becomes more important than the work.

Common mistakes include:

* introducing too many documents at once
* asking the team to change its whole process immediately
* explaining Method before solving a real problem
* treating templates as the value
* creating documentation nobody uses
* replacing conversations with artifacts
* ignoring existing team practices
* forcing VSlices terminology before it helps
* measuring adoption instead of continuity

!!! risk "Do not confuse adoption with usefulness"

    The first goal is not for the team to adopt Method.

    It is for the work to gain enough continuity to decide, build, or learn better.

## Guiding principle

!!! principle "Introduce a useful seam"

    Introduce VSlices Method through one useful continuity seam.


Preserve one piece of knowledge that future work depends on.

If it helps, repeat. If it does not help, reduce the structure until it does.
