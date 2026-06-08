# Digitalized Scenario

A digitalized scenario is a working context where software already represents part of the business, process or organization.

This does not mean the domain is already understood. Existing software is evidence, it is not automatically domain truth.

## Core idea

In a digitalized scenario, VSlices Method helps the team separate three things:

* how work actually happens
* how the current software represents that work
* how people have adapted their work around the software

The goal is not to reverse-engineer the whole system. It is to recover enough continuity to make the next responsible decision.

## When this guide applies

Use this guide when:

* software already exists
* workflows are partially or fully supported by a system
* people depend on current screens, reports, forms, APIs or automations
* the team needs to improve, replace or extend existing behavior
* documentation is missing, outdated or disconnected from implementation
* business knowledge is hidden inside code, tickets or user habits

This guide can apply whether or not the project already uses VSlices Method.

## Main risk

The main risk is treating existing software as the domain truth. A system may contain:

* real business rules
* obsolete decisions
* workaround behavior
* accidental constraints
* technical compromises
* missing concepts
* misleading names
* behaviors users learned to tolerate

If the team copies the existing system without questioning it, it may preserve accidental complexity as if it were domain knowledge.

## Useful starting modality

A digitalized scenario usually starts with **Context-First** or **Problem-First**.

| Situation                                                            | Useful modality   | Reason                                                                                  |
| -------------------------------------------------------------------- | ----------------- | --------------------------------------------------------------------------------------- |
| The system exists, but the surrounding<br/>business context is unclear.  | [**Context-First**](../../design/modalities/context-first/index.md) | The team needs to understand what<br/>the software is trying to represent.                  |
| A clear pain exists in the current system,<br/>but the cause is unclear. | [**Problem-First**](../../design/modalities/problem-first/index.md) | The team needs to understand the<br/>problem before changing behavior.                      |
| A small and safe improvement can<br/>reveal useful evidence.             | [**Slice-First**](../../design/modalities/slice-first/index.md)   | The team can learn through a narrow<br/>change without pretending to<br/>understand everything. |

Slice-First can be useful, but only when the change is small enough to avoid spreading misunderstood assumptions.

## What to observe first

Before changing the system, observe how current work connects to current software. Useful questions include:

* What real work does this software support?
* Which workflows depend on it?
* Which actors use it directly or indirectly?
* Which parts of the system are trusted?
* Which parts are avoided, corrected manually or bypassed?
* Which business terms appear in the interface, code or documentation?
* Which behaviors are expected but not explicit?
* Which errors or exceptions happen repeatedly?
* Which decisions are historical, technical or no longer understood?

The objective is not complete analysis. Is finding where continuity is missing.

## Knowledge to preserve

Preserve knowledge when it affects the next change. Useful knowledge may include:

* domain terms found in the system
* differences between real work and software behavior
* existing workflows affected by the change
* rules hidden inside implementation
* user workarounds
* current pain points
* constraints created by integrations or data
* decisions that should be kept, changed or questioned
* validation signals from users, support or operation

Do not document the whole existing system by default. Preserve what future work should not have to rediscover.

## Document support

Documents may help recover continuity in a digitalized scenario.

| Knowledge need                                                  | Useful document         |
| --------------------------------------------------------------- | ----------------------- |
| Terms are ambiguous or inconsistent.                            | [Domain Vocabulary](../../docs-standard/taxonomy/domain-vocabulary.md)   |
| The surrounding business scenario is unclear.                   | [Context Document](../../docs-standard/taxonomy/context-document.md)    |
| Current work depends on workflows or handoffs.                  | [Process Document](../../docs-standard/taxonomy/process-document.md)    |
| A specific behavior needs to be changed or preserved.           | [Use Case Document](../../docs-standard/taxonomy/use-case-document.md)   |
| A stable business ability is emerging.                          | [Capability Document](../../docs-standard/taxonomy/capability-document.md) |
| A direction must be chosen under tradeoffs.                     | [Decision Record](../../docs-standard/taxonomy/decision-record.md)     |
| Evidence from usage, operation or review changes understanding. | [Validation Note](../../docs-standard/taxonomy/validation-note.md)     |
| Observations are still local, uncertain or temporary.           | [Support Note](../../docs-standard/taxonomy/support-note.md)        |

Use the lightest document that protects continuity.

> Document affinity by iteration stage is described in the [Document-Stage affinity](../document-stage-affinity.md) page.

## Suggested approach

Start by selecting one area of change. Do not try to understand the whole system first.

A useful approach is:

1. Identify the current pain, opportunity or change request.
2. Locate the workflows, actors and system behavior around it.
3. Compare current software behavior with real work.
4. Name what is known, uncertain and risky.
5. Preserve only the knowledge needed for the next responsible decision.
6. Choose the smallest safe change or next investigation.
7. Use feedback to update understanding.

The team should move between understanding and building as evidence appears.

## Common mistakes

Digitalized scenarios commonly fail when teams assume the system explains itself. Common mistakes include:

* copying existing behavior without understanding why it exists
* redesigning everything because the current system looks messy
* treating code names as domain language
* ignoring user workarounds
* documenting the entire system before improving anything
* changing behavior without knowing who depends on it
* assuming old decisions are still valid
* assuming old decisions were wrong only because they are old

Existing software should be respected as evidence. It should not be obeyed as truth.

## Guiding principle

Use the existing system as a source of clues. Recover enough domain, process, behavior and decision continuity to change the system safely.

Do not preserve accidental complexity unless the domain still depends on it.
