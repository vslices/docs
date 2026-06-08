# Modality Selection

Modality Selection explains how to choose a VSlices Design modality for the current iteration.

The goal is not to choose the best modality in general. It is to choose the modality that helps the team reduce the uncertainty that currently threatens continuity.

## Core idea

Choose the modality by the uncertainty that matters most right now. The question is not:

```text
Which modality do we prefer?
```

The better question is:

```text
What kind of uncertainty would make the next decision unsafe?
```

VSlices Method uses the modalities defined by VSlices Design:

* **Context-First**, when the team needs broader understanding before deciding what to build.
* **Problem-First**, when a clear problem exists, but its causes, impact or boundaries need clarification.
* **Slice-First**, when the team can learn faster by building a small and reversible vertical slice.

Method does not redefine these modalities. It helps decide which one should guide the current work.

## Context-First

Use Context-First when the team cannot yet explain the scenario safely. This may happen when:

* the domain is new or poorly understood
* the work is mostly manual or implicit
* several actors interpret the same process differently
* the language is unstable or ambiguous
* the workflow boundaries are unclear
* the team does not know which problem matters most yet

Context-First helps avoid building software around a misunderstood reality.

The main risk is analysis without movement. Use Context-First only until the team has enough context to make a safer next decision.

## Problem-First

Use Problem-First when there is a visible problem, but the team does not yet understand it well enough to solve it responsibly. This may happen when:

* users report a repeated pain
* a workflow has a known bottleneck
* an existing feature fails to support real work
* the business impact is visible but the cause is unclear
* multiple solutions are being proposed before the problem is understood
* the problem may cross several workflows or responsibilities

Problem-First helps avoid solving symptoms. The main risk is local optimization.

Use Problem-First until the team can explain the problem, its context and the intended improvement.

## Slice-First

Use Slice-First when the team can learn more safely by building a small piece of behavior. This may happen when:

* the context is understood enough to act
* the risk is narrow and reversible
* the team needs feedback from real use
* implementation will reveal useful constraints
* a small vertical slice can validate an assumption
* more analysis would not significantly improve the next decision

Slice-First helps avoid designing too much before reality can teach the team. The main risk is implementation without understanding.

Use Slice-First only when the slice is small enough to learn from without hiding important uncertainty.

## Selection signals

A useful selection usually starts by naming the dominant uncertainty.

| Current signal | Start with | Why |
| --- | --- | --- |
| The team does not understand the surrounding context. | __Context-First__ | The next decision needs broader understanding before choosing what to build. |
| The team understands the area, but not the problem. | __Problem-First__ | The next decision needs problem clarity before choosing a solution. |
| The team understands enough to learn through delivery. | __Slice-First__ | The next decision can be made safer by validating a small vertical slice. |

The selected modality should reduce uncertainty. It should not become the identity of the iteration.

A team may start with one modality and later move to another when the kind of uncertainty changes.

## Common mistakes

Modality selection can fail when the team chooses based on habit instead of uncertainty.

* Choosing Context-First for every situation may create analysis paralysis.
* Choosing Problem-First too early may isolate a symptom from its context.
* Choosing Slice-First too early may produce implementation without intent.
* Choosing the same modality repeatedly may hide that the context has changed.
* Choosing a modality as a process rule may weaken judgement.

The modality is a guide for attention. It is not a fixed process.

## Guiding principle

Choose the smallest modality emphasis that makes the next responsible decision safer.

- If understanding is missing, widen the context.
- If the problem is unclear, clarify the problem.
- If learning requires reality, build a small slice.

The right modality is the one that helps the team preserve continuity while moving forward.
