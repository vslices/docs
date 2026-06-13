# "Introducing Method" Scenario

An "Introducing Method" scenario is a working context where a team or organization does not currently use VSlices Method, but is open to improving how knowledge, decisions, implementation and feedback stay connected.

The goal is not to adopt the whole method at once. It is to introduce one useful continuity seam.

## Core idea

VSlices Method should be introduced through real work. A team should not start by changing its whole process. It should start by preserving one piece of knowledge that current or future work depends on. 

The question is not _How do we adopt VSlices Method?_, it is: __Where is continuity currently being lost?__

## When this guide applies

Use this guide when:

* work is already happening
* the team has its own process
* documentation exists but is disconnected from implementation
* decisions are made but not preserved
* tickets describe tasks without enough intent
* feedback appears but does not change future work
* repeated confusion appears across people or teams
* the team is open to lightweight improvement

This guide is not for replacing how a team works. It is for making existing work more continuous.

## Main risk

The main risk is trying to introduce VSlices Method as a complete process. That may create resistance, ceremony or false maturity.

A team may not need new stages, meetings or templates. It may only need a better way to preserve:

* why a change matters
* what context supports it
* what decision was made
* what remains uncertain
* what feedback changed
* what future work should not rediscover

Method should enter through usefulness, not doctrine.

## Useful starting modality

Introducing Method usually starts with **Problem-First** or **Slice-First**.

| Situation                                                                    | Useful modality   | Reason                                                                            |
| ---------------------------------------------------------------------------- | ----------------- | --------------------------------------------------------------------------------- |
| The team feels repeated pain<br/>but does not know where<br/>continuity is breaking. | [**Context-First**](../../design/modalities/context-first/index.md) | The team needs to understand<br/>the loss of continuity before<br/>changing how it works. |
| One small artifact or practice<br/>can improve ongoing work<br/>immediately.         | [**Problem-First**](../../design/modalities/problem-first/index.md)   | The team can validate Method<br/>through a narrow improvement.                        |
| The surrounding work context<br/>is too unclear to intervene<br/>safely.             | [**Slice-First**](../../design/modalities/slice-first/index.md) | The team needs broader<br/>understanding before introducing<br/>a change.                 |

The selected modality should match the adoption uncertainty, not personal preference.

## What to observe first

Before suggesting Method practices, observe how work currently moves. Useful questions include:

* Where does intent get lost?
* Where do people repeat the same explanations?
* Where are decisions made?
* Where are decisions forgotten?
* Where does documentation stop matching reality?
* Where does implementation lose business context?
* Where does feedback disappear?
* Which handoffs create confusion?
* Which small improvement would help current work immediately?

The objective is not to judge the team's process. Is to find one continuity gap worth improving.

## Continuity seams

A continuity seam is a small place where Method can connect knowledge that is currently disconnected. Useful seams may include:

* adding context to one active work item
* recording one important decision
* clarifying one ambiguous domain term
* preserving one validation result
* connecting one use case to one implementation change
* documenting one workflow exception
* capturing one uncertainty before building
* reviewing one stale assumption after feedback

A seam is useful when it helps real work continue with less guessing.

## Document support

Documents may support the introduction of Method, but only when they solve a current continuity problem.

| Continuity gap                                    | Useful document                                                                                                                                                                         |
| ------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| People use the same term with different meanings. | Domain Vocabulary — [Taxonomy](../../docs-standard/taxonomy/domain-vocabulary.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/domain-vocabulary.md)       |
| A task lacks surrounding context.                 | Context Document — [Taxonomy](../../docs-standard/taxonomy/context-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/context-document.md)          |
| A workflow or handoff is misunderstood.           | Process Document — [Taxonomy](../../docs-standard/taxonomy/process-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/process-document.md)          |
| A behavior needs clearer intent.                  | Use Case Document — [Taxonomy](../../docs-standard/taxonomy/use-case-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/use-case-document.md)       |
| A stable ability needs to be named.               | Capability Document — [Taxonomy](../../docs-standard/taxonomy/capability-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/capability-document.md) |
| A decision may affect future work.                | Decision Record — [Taxonomy](../../docs-standard/taxonomy/decision-record.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/decision-record.md)             |
| Feedback should change what happens next.         | Validation Note — [Taxonomy](../../docs-standard/taxonomy/validation-note.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/validation-note.md)             |
| An observation is useful but still uncertain.     | Support Note — [Taxonomy](../../docs-standard/taxonomy/support-note.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/support-note.md)                      |

Do not introduce documents as a package. Introduce the smallest document that protects the work currently at risk.

> Document affinity by iteration stage is described in the [Document-Stage affinity](../document-stage-affinity.md) page.


## Suggested approach

Start with ongoing work. Do not pause the project to introduce Method. A useful approach is:

1. Choose one active work item, problem or decision.
2. Identify where continuity is weak.
3. Add the smallest useful Method structure.
4. Use it during real work.
5. Observe whether it helps people make better decisions.
6. Preserve the learning.
7. Decide whether another seam is worth introducing.

Method should grow only where it keeps proving useful.

## Common mistakes

Introducing Method can fail when the method becomes more important than the work. Common mistakes include:

* introducing too many documents at once
* asking people to change their whole process immediately
* explaining Method before solving a real problem
* treating templates as the value
* creating documentation nobody uses
* replacing conversation with artifacts
* ignoring existing team practices
* forcing VSlices terminology before it helps
* measuring adoption instead of continuity

The first goal is not adoption, it is usefulness.

## Guiding principle

Introduce VSlices Method through one useful continuity seam. Preserve one piece of knowledge that future work depends on.

If that helps, repeat. If it does not help, reduce the structure until it does.
