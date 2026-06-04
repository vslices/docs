# Why Aren't Cookies In The Jar Anymore?

## Definition

> A pattern where inexperienced engineers are given responsibilities, permissions or autonomy beyond their current understanding without sufficient supervision, review or safety mechanisms.
>
> When mistakes eventually occur, the focus often shifts toward the individual who made the mistake rather than the environment that made the mistake possible.
>
> The resulting failures are usually treated as surprises despite being entirely predictable.

## Context

This pattern commonly appears when junior engineers begin receiving ownership over production systems, infrastructure, permissions or critical business processes. The intention is often positive:

- Accelerate growth
- Increase autonomy
- Reduce dependency on senior engineers

However, the level of responsibility frequently grows faster than the engineer's understanding of the system.

The organization assumes competence and safety in the actions of the professional. Neither assumption was validated by another engineer with deep knowledge.

## Observed Behavior

Several recurring patterns emerged:

- Access was granted without clear boundaries.
- Operations were executed without understanding their full impact.
- Documentation was incomplete or unavailable.
- Potential risks were not communicated.
- Reviews were skipped for seemingly simple changes.
- Existing safeguards were absent or insufficient.

The engineer knew enough to perform the task successfully. But not to predict its consequences.

## Common Signals

Possible indicators that this pattern is occurring:

- "Just make the change, it will be a 5 minutes work, like half a story-point."
    - "In fact, why is that a jira story? It does not merit that"
- Production access granted early without supervision.
- Lack of review for infrastructure or security changes.
- Critical operations performed by a single inexperienced engineer.
- No rollback strategy.
- No staging environment.
- Unclear ownership boundaries.
- Dependence on tribal knowledge.

## Underlying Tensions

### Autonomy vs Guidance

> Independence without support is not autonomy. It is abandonment.

### Trust vs Verification

> Trust should not eliminate review.

### Responsibility vs Capability

> Responsibility can be assigned faster than competence can be developed.

### Growth vs Safety

> Engineers learn through mistakes. Systems should be designed to survive them.

## Consequences

### Short-Term

- Unexpected incidents.
- Emergency fixes.
- Production instability.
- Senior engineers pulled into recovery efforts.

### Long-Term

- Loss of confidence.
- Fear of making changes.
- Reduced willingness to take ownership.
- Knowledge silos.
- Increased organizational risk.

Ironically, the engineer often learns the lesson, but the organization rarely learns its own.

## Reflection Questions

- Who reviewed this decision?
- What safeguards existed before the change?
- Was the engineer prepared for this responsibility?
- Would a senior engineer have made the same mistake without context?
- What knowledge was assumed but never taught?
- What prevented this mistake from being caught earlier?
- If this failure was predictable, why was the system exposed to it?

---

## Final Reflection

Having you own junior engineer is like having a child, __don't abandon them__. When you aren't seeing them, they are eating cookies... I mean, breaking production.

Then immediate reaction is often:

> "Who made this change?"

A more useful question might be:

> "Why was this change possible in the first place?"

The engineer made a mistake, the environment made that mistake dangerous. 

Junior engineers are supposed to make mistakes. Systems, processes and teams should be designed with that reality in mind.

Because when the cookies disappear from the jar, the real mystery is rarely who ate them. The real mystery is why nobody was watching the kitchen.
