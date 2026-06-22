# Anti-bureaucracy rules

VSlices Docs Standard should help teams preserve useful knowledge without turning documentation into ceremony.

A document is valuable when it supports understanding, decisions, implementation, validation, or evolution.

A document becomes waste when it exists only because a process, template, or standard made it seem mandatory.

!!! principle "Documentation principle"

    Create the smallest useful documentation that preserves the knowledge future work depends on.


## Rule 1: No document is mandatory by default

VSlices Docs Standard defines available document structures.

It does not require every team to create every document. A document should be created only when it helps preserve knowledge that current or future work depends on.

Before creating a document, the team should ask:

* What knowledge does this document preserve?
* What decision does it support?
* What risk does it reduce?
* What confusion does it prevent?
* Who will use it later?

If those questions do not reveal enough value, the document may not be necessary.

## Rule 2: Use the smallest useful version

The default version of a document should be the smallest version that still helps.

A short document that preserves the right knowledge is better than a long document that repeats obvious information.

| Prefer...          | Before...                            |
| ------------------ | ------------------------------------ |
| Note               | Premature formal document            |
| Minimal document   | Expanded document                    |
| Specific knowledge | Generic explanation                  |
| Useful content     | Complete sections with no real value |

A document should grow because the domain requires it, not because the template allows it.

## Rule 3: Do not confuse volume with understanding

More documentation does not mean better understanding.

A team can produce many documents and still not understand the domain.

It can also preserve strong understanding with a small set of focused documents.

Documentation quality depends on whether it helps the team explain:

* what is happening
* why it matters
* what decision was made
* what knowledge supports that decision
* what uncertainty remains
* what changed after implementation

!!! risk "Risk to avoid"

    Documentation should create clarity, not noise.


## Rule 4: Do not document beyond what is known

A document should not pretend the team knows more than it actually knows.

Unknowns, assumptions, risks, and open questions should remain visible.

| Mark        | Meaning                                                      |
| ----------- | ------------------------------------------------------------ |
| known       | Was validated with domain experts or observed in the system. |
| assumed     | Seems true, but still needs validation.                      |
| unclear     | Is not understood well enough yet.                           |
| invalidated | Was previously believed, but later evidence refuted it.      |

!!! risk "Risk to avoid"

    False certainty is more dangerous than an incomplete document.


## Rule 5: Avoid false completeness

A document that looks complete is not always useful.

It may contain many sections and still fail to preserve important knowledge.

The team should not fill sections with weak text only to make the document look complete.

| Mark           | Meaning                                     |
| -------------- | ------------------------------------------- |
| unknown        | The team does not know this yet.            |
| not applicable | This section does not matter for this case. |
| deferred       | This may matter later, but not now.         |
| superseded     | This was replaced by newer knowledge.       |

A useful document is not the one with every section filled. It is the one that preserves the knowledge future work depends on.

## Rule 6: Keep documents close to decisions

Documentation should not drift away from the decisions it supports.

* When a document influences a decision, that relationship should be visible.
* When a decision affects implementation, that relationship should be visible.
* When implementation produces learning, that learning should return to documentation.

Simple references are enough:

```text
Related context:
- context.order-fulfillment

Related decision:
- decision.payment-validation-boundary

Related validation:
- validation.payment-rules-feedback
```

The goal is traceability without a heavy process.

## Rule 7: Treat outdated documentation as a risk

Outdated documentation can create false confidence.

A document that no longer reflects reality should not remain silently active.

| Status     | Meaning                                                          |
| ---------- | ---------------------------------------------------------------- |
| draft      | The document is still being shaped.                              |
| active     | The document represents useful shared knowledge.                 |
| superseded | The document was replaced by newer knowledge.                    |
| archived   | The document is no longer active, but remains useful as history. |

A document does not need to live forever.

## Rule 8: Split only when it improves clarity

A document should be split when the split improves clarity, reuse, ownership, or traceability.

It should not be split only because the standard has many possible document types.

The team should split when:

* a document mixes unrelated knowledge
* different parts evolve at different speeds
* different people own different parts
* the document is too large to maintain safely
* the same section is reused across several documents

If splitting makes the documentation harder to understand, keep it together.

## Rule 9: Documentation must justify its cost

Documentation has a cost.

It takes time to create, read, review, and maintain.

That cost is acceptable when the document reduces more future cost than it introduces.

The team should ask:

* What happens if we do not write this?
* What happens if someone misunderstands it later?
* What happens if this document becomes outdated?
* Is a support note enough for now?
* Does the document help us move forward?

Documentation should support engineering judgment. It should not replace it.

## Summary

Documentation should make software work safer, clearer, and more connected.

When it stops doing that, it has become ceremony.

!!! principle "Documentation principle"

    Create the smallest useful documentation that preserves the knowledge future work depends on.

