# Slice-First

Slice-First is a VSlices Design modality that starts from a small vertical slice to learn from implementation feedback as early as possible.

It is useful when the team can safely learn more by building a thin working piece of the system than by extending upfront analysis.

Slice-First assumes that not every design iteration needs a broad contextual base before implementation, sometimes the most responsible starting point is a small, concrete, end-to-end slice.

## Definition

Slice-First is a design modality where the team intentionally keeps the initial contextual base small and moves quickly toward a working vertical slice.

In the pyramid metaphor, Slice-First gives more weight to height than to base.

```text
base / height -> small
```

This means the team invests only enough effort in Understanding and Contextualizing to avoid blind implementation, then moves quickly into Planning and Building.

The goal is not to skip understanding, is to learn through implementation while keeping the slice small enough to limit risk.

## When to use it

Use Slice-First when implementation feedback is more valuable than extended upfront analysis. It is especially useful when:

- the domain is already reasonably understood
- the team needs fast validation
- the proposed change can be tested through a small vertical slice
- the cost of being wrong is low or contained
- the team needs to validate technical direction
- the team needs to validate product direction
- the team needs to reduce uncertainty through working software
- the slice can be delivered without destabilizing adjacent flows
- the team can observe feedback soon after delivery
- the work can be scoped narrowly enough to avoid accidental expansion

Slice-First is useful when the team can say:

> We know enough to build a small slice, and building it will teach us what we need next.

## When not to use it

Slice-First may be risky when:

- the domain is mostly unknown
- the business process is fragmented or unclear
- the cost of building the wrong thing is high
- the slice affects critical workflows
- the slice may create irreversible architectural commitments
- the team cannot validate the result after delivery
- the surrounding context is too weak to define a safe slice
- stakeholders may treat the slice as a final solution
- the slice depends on unresolved business rules
- the slice would touch many adjacent flows or responsibilities

In those cases, Context-First or Problem-First may be more appropriate. 

Slice-First may also be unnecessary when the problem is already well understood and the team can implement the improvement directly without needing a learning slice.

## Characteristics

Slice-First usually has these characteristics:

- small initial contextual base
- fast movement toward implementation
- learning through working software
- narrow scope
- strong feedback orientation
- explicit risk awareness
- low ceremony
- high sensitivity to implementation constraints
- preference for vertical integration over broad modeling
- willingness to refine understanding after delivery

Slice-First does not mean building randomly, it means building a small, intentional slice with enough understanding to make learning safe.

## Advantages

Slice-First helps the team:

- learn from real implementation quickly
- avoid overanalyzing before feedback
- validate technical direction early
- validate product direction early
- expose integration constraints
- reveal unknowns that only appear during development
- reduce uncertainty through working software
- create visible progress
- keep scope small
- avoid designing a large solution from untested assumptions

It is especially valuable when the largest risk is spending too much time analyzing something that could be learned from a small implementation.

## Disadvantages

Slice-First also has costs. It may:

- underexplore the surrounding domain
- build from weak assumptions
- produce throwaway implementation
- create premature architectural shape
- hide domain complexity behind a working demo
- confuse prototype feedback with domain understanding
- create local solutions that do not scale conceptually
- miss adjacent business impact
- make stakeholders believe the slice is more complete than it is
- require rework after new understanding appears

The main danger of Slice-First is treating fast learning as proof of complete understanding.

A slice can validate something, rarely validates everything.
