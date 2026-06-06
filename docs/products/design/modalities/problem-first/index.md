# Problem-First

Problem-First is a VSlices Design modality that starts from a specific business or system problem and builds enough surrounding context to improve it effectively.

It is useful when the team already knows what hurts, but still needs to understand enough context to avoid solving the wrong version of the problem.

Problem-First assumes that not every design iteration needs broad domain discovery.

Sometimes the most responsible starting point is not the whole context, it is a clear problem.

## Definition

Problem-First is a design modality where the team begins with a known problem and progressively understands the context around it.

In the pyramid metaphor, Problem-First seeks balance between base and height.

```text
base / height -> balanced
```

This means the team does not build immediately from the problem statement, but also does not spend too much time exploring the entire domain before moving forward.

The goal is to understand enough of the surrounding context to define a useful, feasible, and safe improvement.

## When to use it

Use Problem-First when there is a clear problem that deserves focused attention.

It is especially useful when:

- a specific pain point is already known
- the problem has business impact
- the surrounding domain is partially understood
- the team needs to improve a concrete area
- the team can identify who is affected by the problem
- the problem is important enough to analyze before building
- the scope should remain focused
- the team needs to avoid broad discovery but still needs context
- the risk is not the entire domain being unknown, but the problem being misunderstood
- solving the problem may affect nearby flows, rules, or responsibilities

Problem-First is useful when the team can say:

> We know where the pain is, but we still need to understand it well enough to improve it safely.

## When not to use it

Problem-First may be insufficient when:

- the domain is too unclear to identify the real problem
- the problem statement is only a symptom
- many areas disagree about what the problem actually is
- the surrounding business context is mostly unknown
- the improvement may affect a large operational chain
- the cost of local optimization is high
- the team needs to discover boundaries before defining the problem

In those cases, Context-First may be more appropriate.

Problem-First may also be excessive when:

- the domain is already well understood
- the change is small and low-risk
- the team needs fast implementation feedback
- the best learning will come from a small working slice

In those cases, Slice-First may be more appropriate.

## Characteristics

Problem-First usually has these characteristics:

- starts from a known pain point
- focuses on a specific improvement area
- avoids broad upfront exploration
- builds enough context around the problem
- emphasizes cause, impact, risk, and scope
- gives strong attention to Planning
- uses implementation to validate the chosen improvement
- balances analysis with delivery
- tries to avoid both premature building and endless discovery

Problem-First does not attempt to understand the entire business before acting.

It attempts to understand the problem well enough to improve it responsibly.

## Advantages

Problem-First helps the team:

- stay focused on a concrete problem
- avoid unnecessary broad discovery
- connect design work to visible business pain
- reduce analysis paralysis
- make progress while still preserving enough context
- distinguish symptoms from causes
- identify affected flows and responsibilities
- define scope more clearly
- evaluate tradeoffs before building
- deliver value faster than a broad Context-First iteration

It is especially valuable when the largest risk is not lack of domain awareness in general, but misunderstanding the problem being solved.

## Disadvantages

Problem-First also has costs. It may:

- underexplore the wider domain
- solve a symptom instead of a cause
- optimize a local process while hurting an adjacent one
- miss hidden dependencies
- assume the problem boundary too early
- produce a solution that works technically but fails operationally
- move to Planning before enough context has been discovered
- move to Building before risks have been made explicit

The main danger of Problem-First is local optimization. The team may solve the visible problem while ignoring the wider system that produced it.
