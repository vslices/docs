# Treat PResolver As An Abstraction From VSlices

## Status

Accepted

## Context

VSlices is being developed as a software engineering suite focused on preserving continuity between:

* domain discovery
* documentation
* design reasoning
* architecture
* implementation
* validation
* evolution

During the development of VSlices, a broader pattern appeared. Several VSlices ideas seem useful beyond software engineering:

* reasoning modalities
* progressive documentation
* explicit decisions
* explicit tradeoffs
* bounded interventions
* safeguards
* validation loops
* continuity between understanding, action and evolution

This created the possibility of defining a broader methodology tentatively called PResolver.

However, PResolver should not be introduced as a fully independent methodology before VSlices is validated.

Domus Orbis and other software projects validate VSlices as a software engineering specialization. They do not directly validate PResolver as a general problem-resolution methodology.

## Decision

We will treat PResolver as an abstraction extracted from VSlices.

VSlices remains the concrete software engineering suite. PResolver represents the broader problem-resolution structure that may be abstracted from VSlices if its reasoning, documentation and method patterns prove useful.

The practical direction is:

```text
Build VSlices
-> validate VSlices in software
-> observe recurring patterns
-> remove software-specific assumptions
-> define PResolver v0.1
-> test PResolver in other domains
```

> We will not treat PResolver as the primary product at this stage.
> 
> We will not create a PResolver Framework.
> 
> We will not move VSlices Framework concepts into PResolver unless they survive abstraction outside software.

## Rationale

This preserves focus.

VSlices is concrete, technical and currently actionable. PResolver is broader, more abstract and less validated.

By extracting PResolver from VSlices instead of inventing it upfront, we avoid creating a generic methodology disconnected from practice.

This also gives PResolver a healthier validation path. The question is not:

> Can Domus Orbis validate PResolver?

The question is:

> If VSlices works in software, which parts of its reasoning, documentation and method structure remain useful outside software?

This keeps PResolver experimental without denying its potential.

## Consequences

VSlices documentation should continue to focus on software engineering.

PResolver may appear inside Alive Lab as an exploratory theory.

PResolver v0.1 may later document the reusable abstraction behind:

* PResolver Method
* PResolver Design
* PResolver Docs Standard

These should be treated as possible future products, not current commitments.

The relationship should be expressed as:

```text
VSlices validates a software specialization.
PResolver abstracts the reusable structure.
Other domains test the abstraction.
```

## Tradeoffs

This decision delays public positioning for PResolver.

That is acceptable because premature productization could weaken VSlices.

This decision also means PResolver will not receive full documentation immediately.

That is acceptable because the first priority is still VSlices.

The benefit is that PResolver can grow from observed patterns instead of speculation.

## Risks

PResolver may become too generic if we abstract too aggressively.

VSlices may become harder to explain if PResolver is introduced too early.

The abstraction may fail outside software.

Some VSlices patterns may not generalize well.

There is also a risk of creating a second documentation universe before the first one is stable.

## Guardrails

PResolver must remain exploratory until enough examples exist outside software.

VSlices remains the main product focus.

PResolver should not introduce concepts back into VSlices unless they clarify existing software engineering work.

No PResolver Framework should be created in the current stage.

PResolver should be documented first as an Alive Lab theory, not as a product section.

## Validation

This decision is considered valid while:

* VSlices remains easier to explain as a software engineering suite
* PResolver helps explain broader patterns without stealing focus
* PResolver concepts can be extracted from real VSlices work
* no premature framework or product structure is introduced
* future experiments can test PResolver outside software

This decision should be revisited if:

* PResolver gains repeated validation outside software
* VSlices documentation becomes constrained by software-specific language
* service offerings require a broader problem-resolution framing
* PResolver starts requiring its own stable documentation structure
