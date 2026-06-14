# VSlices Design

VSlices Design helps teams decide how much domain understanding is needed before turning business knowledge into software. 

It provides design modalities, reasoning tools, and modeling heuristics for moving from unclear business material to clearer software decisions without losing continuity. 

VSlices Design is intentionally independent from VSlices Framework. You do not need to use VSlices Framework to apply VSlices Design. 

The Framework can later help implement some of the ideas discovered through Design, but Design itself is a stack-agnostic reasoning product.

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

## What problem does it solve? 

Many teams start software design from the first visible artifact: 

- a screen 
- a user story 
- an endpoint 
- a database table 
- a technical task 
- a requested feature 

Those artifacts are useful, but they often appear after important domain questions have already been skipped.

VSlices Design helps teams pause before committing too early to a structure. 

Its main question is: ``` Do we understand enough of the business material to safely shape the software?```

> Sometimes the answer requires broad contextual discovery. 
> Sometimes it requires focused problem analysis. 
> Sometimes it requires building a small vertical slice to learn from implementation feedback. 

VSlices Design helps teams choose the right starting point for the uncertainty they are actually facing.

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

## What VSlices Design is not

VSlices Design is not a universal methodology. It does not claim that every system should be designed the same way. And it does not assume that:

- Context-First is always correct
- Problem-First is always correct
- Slice-First is always correct
- broad discovery is always required
- fast implementation is always better
- documentation is valuable by default

VSlices Design values documentation only when it preserves intent, reduces ambiguity, or improves continuity across decisions. The right approach depends on the uncertainty, risk, domain maturity, and business urgency of the situation.

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
