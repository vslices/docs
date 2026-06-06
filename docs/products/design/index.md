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

## When should I use VSlices Design?

Use VSlices Design when the team needs to reason about a software system before deciding how it should be built.

It is especially useful when the team is facing uncertainty around the domain, the problem, the boundaries, or the shape of the solution. VSlices Design can help when:

- the business context is still unclear;
- the team is not sure where the system boundaries are;
- stakeholders describe solutions before the underlying problem is understood;
- different people use different words for the same concept;
- the team needs to decide how much discovery is necessary before building;
- the team wants to avoid designing architecture from screens, tables, endpoints, or tasks too early;
- implementation has started, but the domain model still feels unstable.

VSlices Design is not only useful before implementation. It can also be used during implementation when new domain knowledge appears, when a slice reveals incorrect assumptions, or when the team realizes that the current structure no longer represents the business clearly.

The main question is:

> Do we understand enough of the business material to safely shape the software structure?

If the answer is no, VSlices Design helps the team decide what kind of understanding is missing and which modality may help next.

### A small example

Imagine a team is asked to automate an internal approval process. At first, the request sounds simple:

> “We need a screen where managers can approve requests.”

If the team starts from the screen, the database table, or the endpoint, it may accidentally encode a process it does not yet understand.

Using VSlices Design, the team pauses and asks what kind of uncertainty it is facing.

They discover that the real issue is not the approval screen itself. Different departments use different approval rules, some requests require legal validation, some approvals depend on budget limits, and some delays happen before the manager even receives the request.

In this case, the team may start with Context-First to understand the business area before deciding what software structure should exist.

Later, once the context is clearer, the team may move into Problem-First to investigate why approvals are slow.

Finally, once a small part of the process is understood, the team may use Slice-First to build and validate a narrow approval flow.

The goal is not to delay implementation, but to avoid building software from an incomplete understanding of the business material.

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

### Example: regulated approval flow

Consider a system that manages approval requests in a regulated industry.

At first, the team may think about the domain as a pyramid: they collect business knowledge, identify concepts, define processes, and eventually transform that understanding into software structure.

But the knowledge does not move freely from discovery to implementation.

Legal rules, audit requirements, external contracts, and compliance responsibilities filter what the team is allowed to build.

> Some flows are not valid, even if users want them.
> Some data cannot be exposed, even if it would simplify the interface.
> Some decisions must be recorded, even if the business process would be faster without that traceability.

In this case, a prism may be a better geometry than a simple pyramid.

The prism represents the constraints that reshape domain knowledge before it becomes software. The team is not only asking:

> What does the business need?

It is also asking:

> Which constraints transform, block, or reshape what the software is allowed to do?

This keeps the metaphor practical. A knowledge geometry is not decoration. It is a way to make visible how understanding moves, changes, or gets constrained before becoming architecture and implementation.

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
