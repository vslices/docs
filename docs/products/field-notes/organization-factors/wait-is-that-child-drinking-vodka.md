# Wait... Is That Child Drinking Vodka?

> What do you mean by "_again_"?!

_When responsibility grows faster than mentorship_

## Definition

> A pattern where inexperienced engineers are expected to make decisions, operate systems, solve problems and assume responsibilities beyond their current level of understanding without the guidance required to safely develop those capabilities.
> 
> When mistakes eventually occur, the focus often shifts toward the individual rather than the environment that created the conditions for the mistake.
> 
> The resulting failures are frequently treated as unexpected despite being entirely predictable.

## Context

This pattern commonly appears in organizations where delivery pressure consistently takes priority over mentorship.

The organization often believes that knowledge transfer, onboarding and coaching can happen organically while normal work continues uninterrupted. Unlike any investor dream, this does not happen.

Senior engineers become increasingly busy maintaining delivery commitments while junior engineers receive progressively more responsibility with progressively less guidance.

The intention is rarely malicious. Common motivations may include:

- accelerating delivery
- reducing dependency on key individuals
- increasing autonomy
- reducing bottlenecks
- scaling team capacity

Unfortunately, capability rarely grows at the same speed as responsibility.

## Observed Behavior

Several recurring patterns emerged:

- Junior engineers received responsibilities they were not yet prepared for.
- Important context existed only in the minds of senior engineers.
- Mentorship happened reactively instead of intentionally.
- Questions were postponed because everyone was busy.
- Knowledge transfer became a lower priority than delivery.
- Critical decisions were made without sufficient context.
- Engineers learned through production incidents rather than guidance.

The organization expected growth. The environment provided exposure.

Those are not the same thing.

## Common Signals

Possible indicators that this pattern is occurring:

- "They will figure it out."
- "Just give them access."
- "We don't have time for training right now."
- "It is a simple change."
- "Ask if you have questions."
- Critical knowledge concentrated in a few individuals.
- Onboarding largely dependent on tribal knowledge.
- Junior engineers afraid of asking questions.
- Senior engineers constantly too busy to mentor.
- Learning occurring primarily through mistakes.

## Underlying Tensions

### Delivery vs Mentorship

> Every hour invested in teaching appears to reduce short-term delivery. Until the lack of teaching begins reducing delivery far more.

### Responsibility vs Capability

> Responsibility can be assigned immediately. Capability requires time.

### Autonomy vs Abandonment

> Independence without support is not empowerment. It is neglect.

### Exposure vs Development

> Exposure creates opportunities to learn. Development requires guidance.

## Consequences

### Short-Term

- Faster task delegation.
- Reduced immediate dependency on senior engineers.
- Increased perception of team scalability.

### Long-Term

- Repeated mistakes.
- Fragile systems.
- Fear of taking ownership.
- Slow onboarding.
- Knowledge silos.
- Senior engineer overload.
- Organizational dependency on tribal knowledge.

Ironically, the organization often saves time by avoiding mentorship. It later spends significantly more time recovering from the consequences.

## Engineering Impact

- Critical changes become riskier because the people executing them may not understand the surrounding context.
- Mistakes become more likely when responsibility is assigned without matching knowledge, review or support.
- Production incidents may be treated as individual failures even though the system made them predictable.
- Senior engineers remain overloaded because mentorship was postponed until problems became urgent.
- Junior engineers may become afraid of ownership after being exposed to consequences they were not prepared to handle.
- Knowledge silos become stronger when senior engineers are too busy to teach and junior engineers are expected to infer context.
- Code reviews become insufficient if reviewers assume knowledge that was never taught.
- Delivery speed becomes fragile because short-term delegation creates long-term rework.
- Architecture becomes harder to evolve when only a few people understand why the system works the way it does.
- Team capacity appears to increase, but actual capability remains underdeveloped.
- Onboarding becomes inconsistent because growth depends on luck, proximity and informal conversations.
- The organization may confuse exposure to responsibility with development of competence.

When mentorship is absent, the system does not stop teaching. It simply teaches through mistakes, incidents, fear and rework. That kind of learning is expensive, uneven and often damaging.

## Possible interventions

- Define which responsibilities are safe for the engineer to take independently.
- Identify which responsibilities require pairing, review or supervision.
- Make mentorship an explicit responsibility, not an accidental side effect of delivery.
- Create progressive responsibility levels instead of assigning critical ownership all at once.
- Pair junior engineers with experienced engineers on high-context or high-risk work.
- Document the context needed to make safe decisions in critical areas.
- Encourage questions before mistakes become the only source of feedback.
- Replace "ask if you have questions" with scheduled guidance, checkpoints and review moments.
- Treat repeated mistakes as signals of missing support, not only individual performance issues.
- Give access progressively and connect access with understanding, recoverability and review.
- Use checklists for dangerous operations, deployments, migrations or production changes.
- Make senior engineers' mentoring load visible when planning capacity.
- Protect time for teaching before lack of teaching becomes rework.
- After an incident, ask what knowledge, guardrail or guidance would have made the mistake less likely.
- Measure growth by increasing judgment, not only by increasing task assignment.

A useful intervention is to ask: "What would this person need to understand before this responsibility becomes safe?"
That question shifts the focus from blame to capability development.

## Reflection Questions

- Who is responsible for teaching this engineer?
- When was the last intentional mentoring session?
- What knowledge is assumed but never explained?
- What critical decisions can this engineer make safely?
- Would a mistake in this area be recoverable?
- Is autonomy being developed or merely assigned?
- What would happen if the most knowledgeable person left tomorrow?
- Are we creating future seniors or consuming the current ones?

## Final Reflection

When people see a child drinking vodka, the immediate reaction is often:

> "Why is that child drinking vodka?"

A more useful question might be:

> "Why was vodka available to the child in the first place?"

Junior engineers are supposed to:
- Make mistakes. 
- Ask questions.
- Not know things.
- Ask for vodka
  - Even if we are in work hours

None of those are failures.

The failure occurs when an organization expects competence to emerge without creating the conditions required to develop it.

Children do not become adults by accident. Engineers do not become seniors by accident either.

> If nobody had time to teach, someone eventually will have time to fix.
