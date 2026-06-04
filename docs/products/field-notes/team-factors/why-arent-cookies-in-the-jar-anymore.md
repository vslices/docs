# Why Aren't Cookies In The Jar Anymore?

_When autonomy is granted without safety boundaries_

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

## Engineering Impact

- Production systems become fragile when critical actions can be performed without adequate review, context or safeguards.
- Incidents become more likely when permissions are granted faster than understanding is developed.
- Seemingly simple changes may produce unexpected consequences because hidden dependencies are not visible.
- Junior engineers may lose confidence when normal learning mistakes create disproportionate damage.
- Senior engineers are pulled into emergency recovery instead of planned mentoring or design work.
- Teams may become more restrictive after incidents, reducing autonomy instead of improving safety.
- Ownership becomes confusing when people are responsible for systems they do not yet understand deeply.
- Reviews lose effectiveness when risky changes are treated as too small to deserve attention.
- Operational knowledge remains tribal because the mistake reveals knowledge that should have been explicit earlier.
- Delivery slows down after avoidable incidents because trust must be rebuilt.
- The organization may blame the person who triggered the failure instead of fixing the system that allowed it to be dangerous.
- Learning becomes associated with fear when mistakes are punished instead of contained.

When autonomy is granted without safety boundaries, the organization is not accelerating growth. It is increasing the blast radius of inexperience. The goal should not be to prevent junior engineers from making mistakes, but to prevent ordinary mistakes from becoming serious incidents.

## Posible intervertion

- Define which actions require supervision, review or approval before execution.
- Grant permissions progressively according to understanding, recoverability and risk.
- Use staging, sandboxes or test environments before allowing production changes.
- Require rollback plans for infrastructure, data, security or production operations.
- Add checklists for recurring risky tasks such as deployments, migrations or configuration changes.
- Pair inexperienced engineers with senior engineers for high-impact changes.
- Document hidden dependencies, operational constraints and known risks close to the affected system.
- Treat "simple changes" as risky when their impact is not fully understood.
- Make ownership boundaries explicit before assigning responsibility.
- Use code review, change review or operational review as safety mechanisms, not as signs of distrust.
- Design systems so common mistakes are recoverable.
- After an incident, ask what guardrail would have reduced the blast radius.
- Avoid granting access merely because someone needs to complete a task quickly.
- Teach the consequences of actions before expecting independent execution.
- Replace blame with system improvement: what made this mistake possible, dangerous or hard to detect?

A useful intervention is to ask: "What is the worst reasonable outcome if this person makes a normal learning mistake here?"
That question helps design autonomy with boundaries instead of autonomy through abandonment.

## Reflection Questions

- Who reviewed this decision?
- What safeguards existed before the change?
- Was the engineer prepared for this responsibility?
- Would a senior engineer have made the same mistake without context?
- What knowledge was assumed but never taught?
- What prevented this mistake from being caught earlier?
- If this failure was predictable, why was the system exposed to it?

## Final Reflection

Having your own junior engineer is like having a child, __don't abandon them__. When you aren't seeing them, they are eating cookies... I mean, breaking production.

Then immediate reaction is often:

> "Who made this change?"

A more useful question might be:

> "Why was this change possible in the first place?"

The engineer made a mistake, the environment made that mistake dangerous. 

Junior engineers are supposed to make mistakes. Systems, processes and teams should be designed with that reality in mind.

Because when the cookies disappear from the jar, the real mystery is rarely who ate them. The real mystery is why nobody was watching the kitchen.
