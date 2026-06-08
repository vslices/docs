# Collaboration Model

The Collaboration Model explains how people or teams can work through VSlices Method without losing continuity.

VSlices Method does not require fixed roles. It describes responsibilities that may be held by one person, shared by a small team, or distributed across specialized teams.

The goal is not to define an organization chart. The goal is to preserve intent as work moves between discovery, documentation, design, implementation, validation and evolution.

## Core idea

The stages of a VSlices Design iteration are collaboration responsibilities. They are not mandatory roles. 

- A small team may perform all responsibilities together.
- A larger organization may distribute them across different people or teams.

The important rule is continuity:

> Each responsibility should preserve enough intent for the next responsibility to act without guessing why the work matters.

## Common responsibilities

A VSlices Method iteration may involve several responsibilities.

They do not need to be separated. They only need to be visible enough for continuity to be preserved.

* **Discovery responsibility** identifies domain signals, problems, language, workflows, actors and uncertainty.
* **Context preservation responsibility** organizes discovered knowledge into a shared context.
* **Design reasoning responsibility** chooses how to reason about the current uncertainty.
* **Decision responsibility** selects a direction while making tradeoffs explicit.
* **Building responsibility** turns the selected direction into working behavior.
* **Validation responsibility** gathers evidence from review, usage, delivery or operation.
* **Continuity responsibility** carries new learning back into the shared context.

In a small team, the same people may hold all responsibilities. In a larger organization, different groups may hold different responsibilities.

## Collaboration through the iteration flow

The shared VSlices Design iteration flow is:

```text
Understanding
-> Contextualizing
-> Planning
-> Building
-> Understanding
```

> Collaboration should protect continuity across this flow.
> Understanding should not produce disconnected notes.
> Contextualizing should not produce documents that nobody uses.
> Planning should not produce decisions without context.
> Building should not implement behavior without intent.
> Validation should not become isolated feedback that never changes future work.

Each stage should leave enough knowledge for the next stage to move responsibly.

## Handoffs

A handoff happens when responsibility moves from one person or team to another.

A handoff does not need ceremony, it needs preserved intent. Useful handoffs usually make clear:

* what context supports the current work
* what problem or opportunity is being addressed
* what decision has been made
* what remains uncertain
* what behavior is expected
* what feedback should be observed

The purpose of a handoff is not to transfer documents. The purpose is to transfer enough understanding for work to continue without losing meaning.

## Small teams

In a small team, collaboration may happen through direct conversation. Documentation can remain light. 

The main risk is that knowledge stays implicit because everyone believes the context is shared. Small teams should preserve knowledge when:

* a decision affects future work
* a term may be interpreted in different ways
* a behavior has important consequences
* a workflow has exceptions
* validation changes the understanding of the problem

The smaller the team, the more tempting it is to rely only on memory. VSlices Method should help preserve the few things that future work should not have to rediscover.

## Larger organizations

In a larger organization, responsibilities may be distributed. One group may:

- Discover domain signals.
- Another may organize context.
- Another may plan work.
- Another may build.
- Another may validate.

The main risk is local optimization. Each group may do its part correctly while the original intent disappears between stages.

Larger organizations should preserve continuity by making context, decisions, expected behavior and validation visible enough for other groups to continue the work responsibly.

## Collaboration risks

Several risks commonly appear when collaboration loses continuity.

* **Discovery without preservation** creates knowledge that disappears after conversations.
* **Documentation without use** creates artifacts disconnected from work.
* **Planning without context** creates tasks that hide the reason behind the work.
* **Building without intent** creates implementation that solves the ticket but not the problem.
* **Validation without feedback loops** creates learning that does not change future decisions.
* **Specialization without continuity** creates teams that optimize their stage while weakening the whole system.

The Collaboration Model exists to make these risks visible before they become normal.

## Guiding principle

The structure should adapt to the organization. The organization should not be forced to adapt to the method.

Use the smallest collaboration structure that preserves the intent future work depends on.

- If direct conversation preserves enough continuity, use direct conversation.
- If the work crosses time, people, teams or decisions, preserve the knowledge that should not be lost.
