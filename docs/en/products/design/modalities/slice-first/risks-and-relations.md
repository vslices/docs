

# Risks and tradeoffs

Slice-First is useful, but it can fail when speed is confused with clarity. Common risks include:

- blind implementation
- weak domain understanding
- accidental architecture
- premature technical commitments
- throwaway code becoming permanent
- shallow validation
- overfitting to one path
- missing adjacent business impact
- prototype bias
- stakeholder misunderstanding
- ignoring feedback because the slice appears to work
- treating implementation as proof of product correctness

To avoid these risks, the team should keep the slice small, explicit, and reversible when possible. They should ask:

- What are we trying to learn?
- What assumptions are we accepting?
- What risks are we postponing?
- What would invalidate this slice?
- What would make this slice unsafe?
- What would make this slice accidentally permanent?
- Is the slice still small enough?
- Is the feedback real enough?
- Should we continue building or switch modality?

Slice-First should create fast learning, it should not become an excuse to skip thinking or do a poor work.

# Relationship with other modalities

Slice-First is not always the best modality, it is best when fast implementation feedback is more valuable than additional upfront analysis. 

A team may start with Context-First to understand a broad domain, move to Problem-First when a concrete problem becomes clear, and then use Slice-First to validate a small implementation quickly.

A team may also start with Slice-First when the domain is already understood enough and the main uncertainty is practical:

- Can this be implemented?
- Will users interact with it as expected?
- Does this integration work?
- Is this workflow viable?
- Does this small feature produce the expected feedback?

After Building, the team may return to Problem-First or Context-First if the slice reveals deeper uncertainty.

The modalities can be combined across iterations, they are not identities, they are strategies.