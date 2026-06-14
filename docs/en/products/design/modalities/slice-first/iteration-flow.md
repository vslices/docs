# Stage emphasis

Slice-First gives more attention to Building and feedback.

| Stage           | Emphasis     | Objective                                                          |
| --------------- | ------------ | ------------------------------------------------------------------ |
| Understanding   | Low / Medium | Understand only enough to avoid blind implementation.              |
| Contextualizing | Low          | Define the minimum context needed for a safe slice.                |
| Planning        | Medium       | Choose a small vertical slice that can produce learning.           |
| Building        | High         | Build, validate, and use feedback as the main discovery mechanism. |

Slice-First does not require the broadest possible base, just the smallest responsible base that can support the slice.

# Understanding in Slice-First

## Objective

The objective of Understanding is to identify the minimum domain knowledge required to avoid blind implementation.

The team does not try to deeply analyze the entire business area. It focuses on what must be understood before building a small slice.

This stage is related to the inverted pyramid, but the excavation is intentionally shallow and narrow. The team removes only the grains that directly cover the slice. Then asks:

- What are we trying to learn?
- What minimum business concept must we understand?
- Who is affected by this slice?
- What language is required to avoid misunderstanding?
- What existing flow does this slice touch?
- What assumption are we testing?
- What could make this slice unsafe?
- What do we intentionally not understand yet?
- What would force us to stop and switch modality?

The goal is not to understand everything, but to know enough to build without being reckless.

## Common supporting artifacts

- learning goal
- minimal glossary
- assumption list
- actor notes
- affected flow notes
- open questions
- slice boundary notes
- stop-condition notes

## Main risk avoided

Building blindly without knowing what the slice is supposed to teach.

## Risk focus

Understanding in Slice-First should explicitly identify what is being ignored or postponed. The team should make visible:

- assumptions accepted for speed
- unknowns that remain unresolved
- business rules not yet explored
- flows intentionally left outside the slice
- actors not yet considered
- risks that would make the slice unsafe
- conditions that require switching to Problem-First or Context-First

The goal is not to eliminate those risks. It is to know which risks are being accepted.

# Contextualizing in Slice-First

## Objective

The objective of Contextualizing is to define the minimum context needed for a safe vertical slice. The team organizes only the context required to build, validate, and learn from the slice. 

This scenario should be intentionally small, and it may describe:

- the actor involved
- the entry point
- the expected outcome
- the minimum flow touched by the slice
- the immediate dependencies
- the surrounding constraints
- the slice boundary
- what is outside the slice

Contextualizing in Slice-First should not expand unless the slice becomes unsafe or meaningless without more context. So, the team asks:

- What is the smallest meaningful context for this slice?
- Where does the slice start?
- Where does the slice end?
- What flow does it touch?
- What responsibility does it test?
- What dependency must be present?
- What adjacent flows are intentionally excluded?
- What context would make the slice too large?
- What context is missing but acceptable for now?

The objective is not to build a full base, the objective is to build enough base for this slice.

## Common supporting artifacts

- slice context notes
- minimal flow sketch
- boundary notes
- dependency notes
- excluded context notes
- actor notes
- expected outcome notes
- validation notes

## Main risk avoided

Letting the slice expand until it stops being small enough to validate quickly.

## Risk focus

Contextualizing in Slice-First should keep scope pressure visible, the team should watch for:

- hidden dependencies
- expanding boundaries
- unclear entry or exit points
- adjacent flows being pulled into the slice
- missing validation context
- stakeholders adding unrelated expectations
- context that is too weak to make the slice meaningful
- context that is too broad to keep the slice fast

If the minimum context becomes too large, Slice-First may no longer be the right modality.

# Planning in Slice-First

## Objective

The objective of Planning is to choose a small vertical slice that can produce useful learning.

The team defines what will be built, what will be validated, and what will remain outside the slice. Planning shifts the mindset:

> What can we learn by building? -> What is the smallest slice that can teach us that?

The team asks:

- What is the learning goal?
- What is the smallest vertical slice that can validate it?
- What must be included end-to-end?
- What can be intentionally excluded?
- What assumptions will this slice test?
- What feedback do we expect?
- What result would invalidate our direction?
- What risks are we accepting?
- What is the cost of throwing this slice away?
- What would make this slice accidentally permanent?

The preferred slice is not the smallest amount of code, it is the smallest meaningful path from intention to feedback.

## Common supporting artifacts

- slice proposal
- learning goal notes
- scope notes
- out-of-scope notes
- tradeoff notes
- risk notes
- assumption notes
- validation criteria
- rollback notes
- throwaway decision notes

## Main risk avoided

Building a slice that is small in code but meaningless for learning.

## Risk focus

Planning in Slice-First should explicitly define risk boundaries.

The team should make visible:

- what the slice is allowed to prove
- what the slice is not allowed to prove
- what assumptions are being tested
- what assumptions remain untested
- what risks are accepted for speed
- what would require rollback
- what would require rework
- what would require switching modality
- what would prevent the slice from becoming production-worthy

The team should avoid treating the slice as a complete architectural decision, a slice is a learning instrument before it is a final structure.

# Building in Slice-First

## Objective

The objective of Building is to implement the slice, validate the learning goal, and feed the result back into the next iteration. Building includes development, integration, validation, delivery, observation, and feedback.

In this stage, the team may define or implement:

- a thin feature
- a minimal flow
- a small capability
- a temporary integration
- a minimal domain model
- a narrow UI path
- a single endpoint
- a small process automation
- a limited deployment path
- expected errors only for the slice

In Slice-First, Building is the main discovery mechanism.

The team uses implementation feedback to discover constraints, risks, missing concepts, and better questions. The team asks:

- Did the slice validate the learning goal?
- What did implementation reveal?
- Which assumptions survived?
- Which assumptions failed?
- What domain concepts became clearer?
- What technical constraints appeared?
- What adjacent flows became relevant?
- What needs to be refactored, discarded, or expanded?
- Should we continue with Slice-First?
- Should we switch to Problem-First or Context-First?

The result of Building produces feedback.

Sometimes that feedback becomes production value, sometimes it becomes learning. Both useful, but they should not be confused.

## Common supporting artifacts

- implementation notes
- validation notes
- feedback notes
- learned constraint notes
- technical decision notes
- throwaway notes
- production-readiness notes
- refactoring notes
- next-iteration notes

## Main risk avoided

Confusing a working slice with a fully understood solution.

## Risk focus

Building in Slice-First should keep the temporary or limited nature of the slice visible. The team should watch for:

- accidental permanence
- unvalidated assumptions becoming architecture
- prototype code becoming production code without review
- missing error handling
- missing operational concerns
- hidden business rules discovered too late
- stakeholder overinterpretation
- local implementation decisions becoming global constraints
- feedback being ignored because the slice already works

If the slice works, the team should still ask what it actually proved, a working slice is not automatically a correct product decision.
