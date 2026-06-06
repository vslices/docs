# Comparing Design Modalities

VSlices Design provides different modalities for approaching software design depending on the kind of uncertainty the team is facing.

These modalities are not competing methodologies.

They are design strategies.

A team does not need to permanently identify with one of them. The same project may use different modalities at different moments, depending on what is currently unclear.

The purpose of this comparison is to help teams decide where to start.

## Overview

| Modality      | Use when                                                                                              | Main uncertainty                                                                                     | Main risk if skipped                                                                                 |
| ------------- | ----------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- |
| Context-First | The business area is broad, unclear, fragmented, or poorly understood.                                | The team does not yet understand enough of the domain context.                                       | Building software structures based on assumptions, incomplete language, or misunderstood boundaries. |
| Problem-First | There is a visible pain, inefficiency, risk, or opportunity, but its causes are not fully understood. | The team does not yet know what problem should actually be solved.                                   | Solving symptoms instead of causes.                                                                  |
| Slice-First   | The team can safely learn by building a small, narrow, reversible part of the system.                 | The team does not yet know whether a proposed solution, model, or integration will work in practice. | Spending too much time designing before validating reality.                                          |

---

## Context-First

Context-First is useful when the team does not yet understand the business material well enough to define reliable software boundaries.

This modality starts by exploring:

* who participates in the domain,
* what responsibilities exist,
* which processes matter,
* which concepts are used by the business,
* which constraints shape decisions,
* and where boundaries may exist.

Context-First helps avoid premature architecture.

It is especially useful when a team is entering a new domain, replacing a legacy process, or trying to understand how several business areas interact.

### Prefer Context-First when

* the domain language is unclear;
* stakeholders describe the same concept in different ways;
* business processes are not well documented;
* the team does not know where the system boundaries should be;
* the risk of misunderstanding the domain is higher than the risk of delaying implementation.

### Be careful when

Context-First can become too broad if the team keeps exploring without deciding what needs to be built.

The goal is not to understand everything.

The goal is to understand enough to make safer design decisions.

---

## Problem-First

Problem-First is useful when the team already sees a concrete pain, but does not yet understand it deeply enough.

This modality starts from a problem instead of a broad context.

The team investigates:

* what is happening,
* who is affected,
* when the problem appears,
* what causes it,
* what consequences it creates,
* and what would count as improvement.

Problem-First helps avoid solving the wrong thing.

It is especially useful when stakeholders request a feature, but the team suspects that the requested feature may be only one possible solution.

### Prefer Problem-First when

* a business pain is visible;
* users are asking for a specific solution, but the underlying need is unclear;
* the team needs to separate symptoms from causes;
* there are several possible solutions;
* the cost of building the wrong thing is significant.

### Be careful when

Problem-First can become too narrow if the team ignores the surrounding context.

Some problems are symptoms of larger structural issues.

When that happens, the team may need to move temporarily into Context-First.

---

## Slice-First

Slice-First is useful when the team can learn safely by building a small vertical part of the system.

This modality starts from a narrow implementation candidate.

The slice should be small enough to validate assumptions without committing the entire architecture too early.

Slice-First helps teams learn from executable behavior.

It is especially useful when the team already has enough understanding to try something concrete, but still needs feedback from implementation, users, integrations, or technical constraints.

### Prefer Slice-First when

* the domain is sufficiently understood for a small part of the system;
* the team needs technical or product feedback;
* a small experiment can reduce uncertainty;
* the cost of building a narrow slice is acceptable;
* the slice can be changed, removed, or expanded later.

### Be careful when

Slice-First can create accidental architecture if the team treats the first slice as the final structure of the system.

The goal is not to build fast at any cost.

The goal is to learn through a controlled piece of implementation.

---

## Moving between modalities

The modalities are not linear stages.

A team may begin with Context-First, discover a specific problem, move into Problem-First, and later validate a solution through Slice-First.

A team may also begin with Slice-First, discover that the slice exposes misunderstood domain concepts, and return to Context-First.

The important question is:

> What kind of uncertainty are we facing right now?

VSlices Design uses modalities to answer that question without forcing every project into the same design process.

---

## Summary

| Modality      | Use when                                                     | Main risk reduced                   |
| ------------- | ------------------------------------------------------------ | ----------------------------------- |
| Context-First | the business/domain is unclear or fragmented                 | building the wrong abstraction      |
| Problem-First | the domain exists but a specific problem needs clarification | solving symptoms instead of causes  |
| Slice-First   | uncertainty is best reduced through implementation feedback  | over-planning before reality checks |


| If the team says...                                                      | Consider...                    |
| ------------------------------------------------------------------------ | ------------------------------ |
| “We do not understand this business area yet.”                           | Context-First                  |
| “We know something hurts, but we are not sure what the real problem is.” | Problem-First                  |
| “We understand enough to try a small piece and learn from it.”           | Slice-First                    |
| “We keep discovering new business concepts while building.”              | Move back toward Context-First |
| “We are building requested features but the pain remains.”               | Move back toward Problem-First |
| “We are discussing too much and validating too little.”                  | Move toward Slice-First        |
