# Anti-Bureaucracy Rules

VSlices Docs Standard should help teams preserve useful knowledge without turning documentation into ceremony.

> A document is valuable when it supports understanding, decisions, implementation, validation, or evolution.
> 
> A document is wasteful when it exists only because a process, template, or standard made it feel required.

## Rule 1: No document is mandatory by default

VSlices Docs Standard defines available document structures.

It does not require every team to create every document. A document should be created only when it helps preserve knowledge that current or future work depends on. 

The team should ask:

- What knowledge does this document preserve?
- What decision does it support?
- What risk does it reduce?
- What confusion does it prevent?
- Who will use it later?

If those questions do not reveal enough value, the document may not be needed.

## Rule 2: Use the smallest useful version

The default version of a document should be the smallest version that still helps.

A short document that preserves the right knowledge is better than a long document that repeats obvious information.

The team should prefer:

- __note before document__: capture early knowledge lightly before giving it formal structure.
- __minimal before expanded__: start with the smallest useful document version.
- __specific before generic__: preserve concrete knowledge before writing broad explanations.
- __useful before complete__: fill what matters, not every possible section.

A document should grow because the domain requires it, not because the template allows it.

## Rule 3: Do not confuse volume with understanding

More documentation does not mean better understanding.

> A team can produce many documents and still misunderstand the domain.
> 
> A team can also preserve strong understanding with a small set of focused documents.

The quality of documentation depends on whether it helps the team explain:

- what is happening.
- why it matters.
- what decision was made.
- what knowledge supports that decision.
- what uncertainty remains.
- what changed after implementation.

Documentation should create clarity, not noise.

## Rule 4: Do not document beyond what is known

A document should not pretend that the team knows more than it actually knows.

Unknowns, assumptions, risks, and open questions should remain visible. The team should prefer honest uncertainty over false precision. Examples:

- __known__: this was validated with domain experts or observed in the system.
- __assumed__: this seems true, but still needs validation.
- __unclear__: this is not understood well enough yet.
- __invalidated__: this was believed before, but later evidence disproved it.

False certainty is more dangerous than an incomplete document.

## Rule 5: Avoid false completeness

A complete-looking document is not always useful, it may contain many sections and still fail to preserve the important knowledge.

The team should not fill sections with weak text just to make the document look complete. Use simple marks when needed:

- __unknown__: the team does not know this yet.
- __not applicable__: this section does not matter for this case.
- __deferred__: this may matter later, but not now.
- __superseded__: this was replaced by newer knowledge.

A useful document is not the one with every section filled. It is the one that preserves the knowledge future work depends on.

## Rule 6: Keep documents close to decisions

Documentation should not drift away from the decisions it supports.

- When a document influences a decision, that relationship should be visible.
- When a decision affects implementation, that relationship should be visible.
- When implementation produces learning, that learning should return to the documentation.

Simple references are enough:

```text
Related context:
- context.order-fulfillment

Related decision:
- decision.payment-validation-boundary

Related validation:
- validation.payment-rules-feedback
```

The goal is traceability without heavy process.

## Rule 7: Treat stale documentation as risk

Outdated documentation can create false confidence. A document that no longer reflects reality should not remain silently active.

The team should update it, supersede it, or archive it. Suggested states:

- __draft__: the document is still being shaped.
- __active__: the document currently represents useful shared knowledge.
- __superseded__: the document was replaced by newer knowledge.
- __archived__: the document is no longer active, but remains useful as history.

A document does not need to live forever.

## Rule 8: Split only when it improves clarity

> A document should be split when the split improves clarity, reuse, ownership, or traceability.
> 
> A document should not be split only because the standard has many possible document types.

The team should split when:

- one document is mixing unrelated knowledge.
- different parts evolve at different speeds.
- different people own different parts.
- the document is too large to maintain safely.
- the same section is reused by several other documents.

If splitting makes the documentation harder to understand, keep it together.

## Rule 9: Documentation must justify its cost

Documentation has a cost. It takes time to create, read, review, and maintain.

That cost is acceptable when the document reduces more future cost than it introduces. The team should ask:

- What happens if we do not write this?
- What happens if someone misunderstands this later?
- What happens if this document becomes outdated?
- Is a support note enough for now?
- Is the document helping us move forward?

Documentation should support engineering judgment. It should not replace it.

## Summary

VSlices Docs Standard follows a simple anti-bureaucracy principle:

> Create the smallest useful documentation that preserves the knowledge future work depends on.

Documentation should make software work safer, clearer, and more connected. When documentation stops doing that, it has become ceremony.
