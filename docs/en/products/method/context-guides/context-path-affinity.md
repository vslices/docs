# Continuity Paths in VSlices Method

VSlices Method uses continuity paths to help decide how to approach a real context before choosing documents, techniques, or implementation structures.

Continuity paths are defined by VSlices Docs Standard.

VSlices Method does not redefine those paths.

It uses them as a working tool to recognize which continuity needs to be preserved during discovery, documentation, design, implementation, or evolution.

!!! principle "Continuity principle"

    Start from the continuity that needs to be preserved, not from the document that could be written.


## Why Method needs this idea

Without continuity paths, it is easy to treat documentation as a list of documents to complete.

VSlices Method tries to avoid that.

The initial question should not be "*What document is missing?*", but: "**What continuity do we need to understand and preserve?**".

After answering that question, Docs Standard helps identify which documents can support that path.

## Available paths

VSlices Docs Standard defines five main continuity paths:

| Path                                                                                          | Question it helps answer                                             |
| --------------------------------------------------------------------------------------------- | -------------------------------------------------------------------- |
| [Business scenario](../../docs-standard/continuity-paths/perspectives/business-scenario.md)   | Where does the work happen, and why does it matter?                  |
| [Domain context](../../docs-standard/continuity-paths/perspectives/domain-context.md)         | What language, rules, boundaries, and meanings need to be preserved? |
| [Software project](../../docs-standard/continuity-paths/perspectives/software-project.md)     | What technical initiative is addressing the work?                    |
| [Client product](../../docs-standard/continuity-paths/perspectives/client-product.md)         | What visible behavior delivers value to users or clients?            |
| [Consumable service](../../docs-standard/continuity-paths/perspectives/consumable-service.md) | What capabilities does the system offer or consume?                  |

Method does not assume that every path must be walked in every iteration.

A piece of work can have one primary path and one or more secondary paths.

## Context-path affinity

A context has affinity with a path when that path best explains the continuity at risk.

Context-path affinity helps decide where to start.

| Observed context                                                              | Path with strongest affinity |
| ----------------------------------------------------------------------------- | ---------------------------- |
| The team needs to understand how the work happens today                       | Business scenario            |
| The team needs to clarify language, rules, boundaries, or meanings            | Domain context               |
| The team needs to join, modify, or structure a software initiative            | Software project             |
| The team needs to define visible behavior for users or clients                | Client product               |
| The team needs to expose, consume, or coordinate capabilities between systems | Consumable service           |

!!! risk "Checklist risk"

    If every path starts to look mandatory, affinity has been lost. Paths help reduce noise, not add ceremony.


## Primary and secondary paths

The primary path represents the most important continuity for the current work.

Secondary paths provide context, precision, or support.

They should not turn a small iteration into a complete exploration of the system.

| Path type | Use                                                             |
| --------- | --------------------------------------------------------------- |
| Primary   | Explains the continuity we cannot afford to lose                |
| Secondary | Supports understanding of the primary path                      |
| Future    | May become relevant later, but does not need to be deepened now |

## Using paths during an iteration

When starting an iteration, Method can use continuity paths this way:

1. Observe the real context

    Before documenting, understand what situation we are facing.

2. Identify the continuity at risk

    Determine what knowledge would be costly to lose, misunderstand, or separate from the implementation.

3. Recognize the path with the strongest affinity

    Choose the path that best explains the current work.

4. Identify useful documents

    Use Docs Standard to decide which documents can support that path.

5. Apply document-stage affinity

    Decide which documents are worth working on now and which can wait.

6. Implement while preserving continuity

    Keep intent, language, behavior, decisions, and technical structure connected.

## Expected outcome

Using continuity paths inside Method should help answer:

* which continuity matters now
* from which perspective the work should be understood
* which documents can support that path
* which paths can wait
* which complexity we do not need to introduce yet

Method does not use paths to impose a universal route.

It uses them to preserve focus.
