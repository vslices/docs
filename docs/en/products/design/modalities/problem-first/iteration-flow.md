# Stage emphasis in Problem-First

Problem-First gives more attention to Planning while keeping enough Understanding and Contextualizing around the problem.

| Stage           | Emphasis      | Objective                                                                        |
| --------------- | ------------- | -------------------------------------------------------------------------------- |
| Understanding   | Medium        | Understand the problem and the domain concepts directly around it.               |
| Contextualizing | Medium        | Place the problem inside its surrounding flow and responsibilities.              |
| Planning        | High          | Define the most effective improvement and make risks explicit.                   |
| Building        | Medium / High | Implement the improvement and validate whether the problem was actually reduced. |

Problem-First does not require the broadest possible base.

It requires a base wide enough to support the selected improvement.

# Understanding in Problem-First

## Objective

The objective of Understanding is to clarify the problem before trying to solve it.

The team starts from a known pain point, request, failure, opportunity, or limitation. Then it explores the domain concepts directly surrounding that problem.

This stage is related to the inverted pyramid, but the excavation is focused, the team is not trying to remove every grain of sand around the business. It is removing the grains that cover the problem.

So, the team asks:

- What problem are we trying to solve?
- Who experiences this problem?
- When does the problem appear?
- What language do people use to describe it?
- Which concepts are directly involved?
- What current behavior produces or exposes the problem?
- What assumptions are we making about the cause?
- Is this problem a symptom of something deeper?
- What would happen if we did nothing?

The goal is not to fully model the domain. It is to understand the problem clearly enough to avoid solving the wrong thing.

## Common supporting artifacts

- problem statement
- domain interview notes
- glossary
- concept notes
- actor list
- problem evidence notes
- assumption list
- open questions
- early flow sketches

## Main risk avoided

Solving a vaguely understood problem because it looked obvious at first.

# Contextualizing in Problem-First

## Objective

The objective of Contextualizing is to place the problem inside its surrounding business context.

The team organizes the discovered knowledge into a focused base scenario. This scenario should explain where the problem appears, who is affected, what currently happens, and which surrounding flows may matter. After that, the team may asks:

- Where does the problem appear in the current flow?
- Which actors, areas, systems, or responsibilities are involved?
- What happens before the problem appears?
- What happens after the problem appears?
- Which adjacent flows could be affected by a change?
- Which rules, exceptions, or dependencies shape the problem?
- Which parts of the context are relevant now?
- Which parts can remain outside the current iteration?

Contextualizing in Problem-First should be narrower than in Context-First, The team should avoid expanding the investigation unless the surrounding context changes the decision.

The objective is not to understand everything, but to understand enough around the problem.

## Common supporting artifacts

- current scenario notes
- focused flow sketch
- swimlane diagram
- responsibility map
- pain point list
- affected area notes
- concept relationship notes
- boundary notes
- current behavior notes

## Main risk avoided

Treating the problem as isolated when it is actually caused or constrained by surrounding flows.

# Planning in Problem-First

## Objective

The objective of Planning is to define the most effective improvement for the problem.

This is the most important stage in Problem-First.

The team uses the focused context to decide what should change, why it should change, how much should change, and what risks the change may introduce. Planning shifts the mindset:

> What is the problem? -> What improvement should we make now?

The team asks:

- What is the real problem we are solving?
- What outcome would prove that the problem improved?
- Which improvement creates meaningful business value?
- Which solution is feasible in the current context?
- Which options are available?
- Which option is simplest?
- Which option creates the least accidental complexity?
- Which adjacent flows could be affected?
- Which risks or mitigations exist?
- What should remain outside the current iteration?
- What assumptions still need validation?
- What failure modes should we expect?
- What tradeoffs are we accepting?

Problem-First should not jump from problem to solution too quickly.

The problem may be clear, but the solution still needs design judgment, the preferred improvement is the one that reduces the problem effectively without creating disproportionate complexity elsewhere.

## Common supporting artifacts

- improvement proposal
- target scenario notes
- scope notes
- tradeoff notes
- risk notes
- mitigation notes
- decision notes
- affected flow list
- use case sketches
- target process sketches
- expected outcome notes
- out-of-scope notes

## Main risk avoided

Choosing the first attractive solution instead of the most appropriate improvement.

## Risk focus

Planning in Problem-First should explicitly identify risks.

This is important because the modality intentionally avoids broad domain exploration. So, the team should make visible:

- risks caused by limited context
- risks caused by affected adjacent flows
- risks caused by implicit business rules
- risks caused by unclear ownership
- risks caused by technical constraints
- risks caused by changing user behavior
- risks caused by solving a symptom instead of a cause

The team does not need to eliminate every risk. But it should know which risks it is accepting before Building starts.

# Building in Problem-First

## Objective

The objective of Building is to implement the selected improvement and validate whether it actually reduces the problem. Building includes development, integration, validation, delivery, and feedback.

In this stage, the planned improvement becomes real, the team may define or implement:

- features
- flows
- capabilities
- domain types
- integrations
- services
- expected errors
- deployment changes
- operational adjustments

In Problem-First, Building should remain connected to the original problem.

A feature should be traceable to:

- the problem statement
- the affected actors
- the relevant flow
- the selected improvement
- the expected outcome
- the accepted risks
- or the target behavior

Building also tests whether the team understood the problem correctly.

When the team builds, it discovers whether the planned improvement was clear enough, too narrow, too broad, incomplete, or wrong.

The result of Building produces business value, but it also produces new knowledge. That new knowledge becomes material for the next iteration. After that, the team asks:

- What needs to be implemented now?
- Which problem does this implementation reduce?
- Which assumptions are being tested?
- Which accepted risks need attention?
- Which design artifacts are guiding the implementation?
- Which behavior proves the improvement worked?
- What new constraints appeared during development?
- What changed after delivery?
- Did the problem actually improve?
- What should be explored next?

## Common supporting artifacts

- feature notes
- implementation notes
- validation notes
- delivery notes
- feedback notes
- technical decision notes
- discovered constraint notes
- accepted risk notes
- outcome validation notes
- next-iteration notes

## Main risk avoided

Delivering a technically correct solution without validating whether the problem improved.

## Risk focus

Building in Problem-First should keep risks visible during implementation.

This does not mean slowing down development with unnecessary ceremony. It means making sure the team does not forget the risks accepted during Planning.

The team should watch for:

- implementation drift from the original problem
- new complexity introduced by the solution
- new edge cases discovered during development
- conflicts with adjacent flows
- missing validation of the expected outcome
- hidden rules that appear only during implementation
- technical shortcuts that weaken the improvement
- feedback that reveals the problem was misunderstood

If Building reveals that the problem was misunderstood, the iteration should return to Understanding.

That is not failure, it is learning.
