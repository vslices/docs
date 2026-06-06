# VSlices Design

VSlices Design is the design product of the VSlices Suite.

It provides design modalities, reasoning tools, and modeling heuristics to help teams move from domain understanding to software decisions without losing continuity.

VSlices Design is intentionally independent from VSlices Framework, you do not need to use it to apply VSlices Design.

The purpose of VSlices Design is to help teams understand:

- what business context they are working with
- how much uncertainty exists
- what kind of design approach is appropriate
- how domain knowledge becomes software artifacts
- when to explore broadly
- when to focus on a specific problem
- when to learn from a small vertical slice

VSlices Design does not assume that every project needs the same methodology.

Different situations require different ways of moving from discovery to implementation.

## Purpose

Many software projects start from artifacts that appear too late in the reasoning process:

- user stories
- screens
- APIs
- database tables
- technical components
- implementation tasks

These artifacts are useful, but they are not always the right starting point.

When the domain is unclear, fragmented, manual, legacy-driven, or organizationally complex, starting directly from implementation can create accidental complexity.

VSlices Design exists to reduce that risk.

Its purpose is to help teams choose the right amount of understanding, context, planning, and implementation feedback before moving forward.

## Design modalities

VSlices Design uses modalities to adapt the design process to different kinds of uncertainty.

A modality is not a rigid methodology. It is a way to decide how much contextual base is needed before moving toward implementation. The current VSlices Design modalities are:

- Context-First
- Problem-First
- Slice-First

These modalities share the same general iteration flow:

```text
Understanding -> Contextualizing -> Planning -> Building -> Understanding
```

What changes is the emphasis.

## Same flow, different emphasis

The modalities do not compete, they respond to different kinds of uncertainty.

The modality can change between iterations, starting with one modality does not force the team to keep using it forever.

VSlices Design treats modalities as strategies. Not identities.

## Knowledge geometry

VSlices Design uses geometric metaphors intentionally.

The current model uses pyramids because they help explain how domain knowledge is discovered, composed, and transformed into business value.

The inverted pyramid represents discovery, it helps explain how a team extracts understanding from a wide business context.

The construction pyramid represents composition, it helps explain how discovered knowledge becomes ideas, artifacts, implementation, and value.

This does not mean that every domain must always be interpreted as a pyramid. The pyramid is the first useful geometry because it represents accumulated understanding.

Future versions of VSlices Design may explore other geometric metaphors when they help explain different kinds of domain constraints.

For example, a prism may be useful when knowledge does not flow freely because it is constrained by strong boundaries, regulations, legacy systems, organizational silos, external contracts, or fixed responsibilities.

In that sense:

> A pyramid explains how knowledge becomes value.
> A prism explains what prevents knowledge from flowing freely.

These geometries are not decorative metaphors.

They are reasoning tools.

Their purpose is to help teams understand how knowledge behaves before deciding how software should be designed.

## What VSlices Design is not

VSlices Design is not a universal methodology. It does not claim that every system should be designed the same way. And it does not assume that:

- Context-First is always correct
- Problem-First is always correct
- Slice-First is always correct
- broad discovery is always required
- fast implementation is always better
- documentation is valuable by default

The right approach depends on the uncertainty, risk, domain maturity, and business urgency of the situation.

## Relationship with the VSlices Suite

VSlices Design is one product inside the VSlices Suite.

It connects with the other products, but it remains independent.

- VSlices Design provides the design modalities and reasoning tools.
- VSlices Docs Standard can provide formal documentation structures for preserving the discovered intent.
- VSlices Method can define how the design process is applied across an engineering workflow.
- VSlices Framework can later reflect the resulting concepts as contexts, capabilities, features, flows, errors, and integrations.

The goal is continuity.

Domain understanding should not disappear when the team starts documenting.

Documentation should not become disconnected from architecture.

Architecture should not become disconnected from implementation.

Implementation should remain traceable to the business intent that justified it.

## Core principle

VSlices Design follows a simple principle: _Understand the business material before building the software structure_.

> Sometimes that requires broad contextual discovery.
> Sometimes it requires focused problem analysis.
> Sometimes it requires a small vertical slice.

The important part is not choosing the most sophisticated modality, it is choosing the modality that matches the uncertainty the team is actually facing.
