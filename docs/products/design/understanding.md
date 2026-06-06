# Understanding VSlices Design

VSlices Design uses modalities to adapt the design process to different kinds of uncertainty.

A modality is not a rigid methodology it is a way to decide how much understanding, context, planning, and implementation feedback a team needs before moving forward.

- Some situations require a broad contextual base before defining software artifacts.
- Some situations require a focused problem analysis.
- Some situations require a small vertical slice to learn from implementation as soon as possible.

VSlices Design uses two complementary metaphors to explain this movement:

- the inverted pyramid: explains how the team understands a business.
- the construction pyramid: explains how the team turns that understanding into value.

Together, both metaphors describe the central idea of VSlices Design:

> Before building software artifacts, the team must understand where their material comes from.

A feature should not appear as an isolated decision, it should be built from grains of domain understanding that were discovered, selected, shaped, and placed with intention.

The pyramid is the initial geometry used by VSlices Design because it represents accumulated understanding. Other geometries may be explored in the future when different domain constraints require different reasoning tools.

## The inverted pyramid

The inverted pyramid represents the business as a wide surface of domain knowledge.

The narrow peak is at the bottom, the wide base is at the top, and there are many grains of sand there:

- concepts
- words
- actors
- areas
- departments
- roles
- flows
- rules
- exceptions
- assumptions
- problems
- opportunities
- business signals

Those grains give shape to the business. But not all of them are equally relevant to the current objective.

To understand the business, the team must remove the grains covering the area being explored, but removing grains does not mean deleting them.

It means understanding them, discovering what they are, how they relate to each other, why they exist, and whether they matter for the current goal.

The deeper the team goes, the more precise the understanding becomes. At the surface, the team may only recognize vocabulary and actors.

Deeper down, the team starts finding flows, responsibilities, rules, pain points, risks, and possible changes.

Even deeper, the team may discover the shape of use cases, processes, capabilities, services, and features.

The inverted pyramid is the metaphor for discovery, it explains where the sand comes from.

## The construction pyramid

Once the team has extracted enough sand from the business context, it can start building.

The construction pyramid represents how domain understanding becomes business value.

The first iteration creates the initial base of the pyramid. This base is important because it gives the team an early sense of:

* how large the domain may be
* how many areas or actors are involved
* how much uncertainty exists
* where the first boundaries may appear
* which parts of the domain may require deeper exploration

A large pyramid needs a strong base.

In the same way, a large or complex system needs enough contextual understanding before the team starts defining precise software artifacts. Each new iteration adds more sand to the construction site.

But each grain has a different meaning depending on where it lands.

- If it lands near the base, it may represent new domain understanding.
- If it lands slightly above the base, it may represent a newly discovered flow or adjacent process.
- If it lands around the middle, it may become a use case, process definition, or responsibility boundary.
- If it lands near the top, it may indicate the need for a formal service, capability, or component.
- If it reaches the peak, it may become a concrete feature ready to be implemented and delivered.

The construction pyramid is the metaphor for composition, it explains how understanding becomes value.

## From extraction to construction

VSlices Design moves between both pyramids.

> First, the team extracts sand from the inverted pyramid.
> 
> Then, the team places that sand in the construction pyramid.

The movement is:

1. Discover domain knowledge.
2. Understand what matters.
3. Organize the discovered knowledge.
4. Shape ideas from that knowledge.
5. Turn ideas into design artifacts.
6. Use those artifacts to guide implementation.
7. Deliver business value.

The team should not build the construction pyramid with random sand.

It should not create features, services, screens, APIs, or components only because they seem plausible. Those artifacts need support.

They should be built from understood business material.

## Why both pyramids matter

A team can try to build only the top of the construction pyramid.

It can start directly from features, services, screens, APIs, or database structures. Sometimes this works, especially in small or well-known domains.

But in unclear, manual, fragmented, legacy-driven, or organizationally complex domains, this creates risk.

Without enough base, artifacts are stacked without support. They may look like progress, but they are unstable or unrelated.

As more knowledge appears, those artifacts may collapse, move, split, or need to be rebuilt elsewhere.

VSlices Design exists to reduce that risk.

It does not reject features, services, screens, APIs, or technical components. It refuses to treat them as the starting point when the domain is still unclear.

## Base and height

The construction pyramid has two useful dimensions: __base__ and __height__

The base represents contextual support, it answers questions like:

- How much of the domain do we understand?
- How much surrounding context do we need?
- Which concepts, actors, flows, and boundaries support the current objective?
- How much uncertainty should be reduced before building?

The height represents movement toward concrete implementations, answering questions like:

- How quickly do we move toward a feature?
- How soon do we validate through implementation?
- How concrete does the output of the iteration need to be?
- How much value can we deliver from the current understanding?

VSlices Design uses modalities, because different situations need different proportions between base and height.

## Modality proportion

A VSlices Design modality defines the proportion between contextual base and implementation height. They do not compete, they just respond to different kinds of uncertainty and contexts.

The stages are similar across modalities, but the emphasis changes. A modality answers: _How much base do we need before moving upward?_

> Context-First prioritizes the base.
> Problem-First seeks balance between base and height.
> Slice-First prioritizes height.

## A simple way to think about modalities

A modality can be understood through the relationship between base and height:

```text
base / height
```

Context-First tends toward a large base:

```text
base / height -> large
```

Problem-First tends toward balance:

```text
base / height -> balanced
```

Slice-First tends toward fast height:

```text
base / height -> small
```

It is a design heuristic, that helps the team reason about how much context is needed before moving toward construction.

And it is a heuristic that also implies that you can switch modalities after each iteration.

## Core principle

VSlices Design follows a simple principle:

> Understand the business material before building the software structure.

The inverted pyramid helps the team understand the business, the construction pyramid helps the team turn that understanding into value.

The modalities help the team decide how much understanding is needed before moving toward implementation.
