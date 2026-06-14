# Iteration flow in Context-First

Context-First gives more attention to Understanding and Contextualizing.

| Stage           | Emphasis       | Objective                                                                        |
| --------------- | -------------- | -------------------------------------------------------------------------------- |
| Understanding   | High           | Discover enough domain knowledge to understand the business area.                |
| Contextualizing | High           | Build a broad base scenario of current flows, actors, concepts, and<br/>boundaries.  |
| Planning        | Medium         | Select the most valuable improvement supported by the contextual<br/>base.           |
| Building        | Medium<br/>(_later_) | Implement the improvement without losing traceability to the<br/>discovered context. |

The early stages are intentionally stronger because Context-First assumes that weak context creates unstable implementation decisions.

# Understanding in Context-First

## Objective

The objective of Understanding is to excavate enough domain knowledge to know what the business area is made of.

The team listens to domain experts, observes existing work, identifies recurring vocabulary, discovers concepts, detects actors, and captures assumptions.

This stage is related to the inverted pyramid, the team removes the grains of sand that cover the area being explored and removing grains means understanding them.

So, the team asks:

- What concepts appear repeatedly?
- Who participates in this business area?
- What language do domain experts use?
- Which flows already exist?
- What problems are visible?
- Which assumptions are we making?
- What parts of the domain are still unclear?
- Which concepts seem foundational?
- Which stories are repeated by different people?

The goal is not to model the whole business. It is to understand enough to continue with better questions.

## Common supporting artifacts

- glossary
- concept notes
- domain interview notes
- actor list
- area or department list
- open questions
- assumption list
- early flow sketches
- recurring story notes

## Main risk avoided

Designing software artifacts before understanding the world they belong to.

# Contextualizing in Context-First

## Objective

The objective of Contextualizing is to organize discovered knowledge into a broad base scenario.

The team takes the sand extracted during Understanding and starts placing it in the construction pyramid. This stage makes the current context visible, it may describe:

- relevant areas or departments
- actors and responsibilities
- current flows
- current systems
- current pain points
- current boundaries
- important concepts
- relationships between concepts
- handoffs between participants
- adjacent flows

Contextualizing does not define the final solution. Its purpose is to make the current situation visible enough to support better decisions. So then, the team asks:

- What is the current scenario?
- How does work move today?
- Which areas, actors, systems, or external participants are involved?
- Which flows surround the objective?
- Which responsibilities are explicit?
- Which responsibilities are implicit?
- Which boundaries are starting to appear?
- Which adjacent flows could be affected?
- What should be preserved as shared understanding?

A strong contextual base makes later decisions safer, without enough base, later artifacts may look precise but remain unstable.

## Common supporting artifacts

- current scenario notes
- flow sketches
- swimlane diagrams
- responsibility map
- context map
- concept relationship notes
- pain point list
- boundary notes
- affected area notes
- current process notes

## Main risk avoided

Treating a problem, use case, or feature as isolated when it actually belongs to a larger operational context.

# Planning in Context-First

## Objective

The objective of Planning is to decide which improvement should be pursued from the contextual base.

The team uses the discovered context to evaluate what should change, why it should change, and what impact that change may have. Planning shifts the mindset:

> What is happening? -> What should become better?

In Context-First, Planning should be supported by enough surrounding understanding to avoid local optimization.

The team asks:

- Which problems are worth solving now?
- Which improvement creates meaningful business value?
- Which improvement is feasible in the current context?
- Which adjacent flows could be affected?
- Which risks or mitigations exist?
- Which parts should remain outside the current iteration?
- What would the improved scenario look like?
- Which use cases, processes, capabilities, or services may be needed?
- What assumptions still need validation?

The preferred improvement is not always the most technically interesting one. It is the improvement that provides meaningful business value without introducing disproportionate complexity.

## Common supporting artifacts

- improvement proposal
- target scenario notes
- scope notes
- tradeoff notes
- risk notes
- decision notes
- affected flow list
- use case sketches
- target process sketches
- mitigation notes
- out-of-scope notes

## Main risk avoided

Solving the most attractive technical problem instead of the most relevant business problem.

# Building in Context-First

## Objective

The objective of Building is to implement the planned improvement while preserving continuity with the discovered context. Building includes development, integration, validation, delivery, and feedback.

In this stage, design artifacts become implementation decisions, the team may define or implement:

- features
- flows
- capabilities
- domain types
- integrations
- services
- expected errors
- deployment changes
- operational adjustments

In Context-First, Building should remain connected to the base built in previous stages.

A feature should not appear as an isolated implementation decision. It should be traceable to:

- business concept
- flow
- responsibility
- pain point
- target improvement
- discovered boundary

Building also tests the understanding accumulated so far. When the team builds, it discovers whether the previous stages were clear enough, incomplete, or wrong.

The result of Building produces business value, but it also produces new knowledge. That new knowledge becomes material for the next iteration.

The team asks:

- What needs to be implemented now?
- Which assumptions are being tested?
- Which design artifacts are guiding the implementation?
- Which concepts or flows support this feature?
- What new constraints appeared during development?
- What changed after delivery?
- What did the team learn?
- What should be explored next?

## Common supporting artifacts

- feature notes
- implementation notes
- validation notes
- delivery notes
- feedback notes
- technical decision notes
- discovered constraint notes
- next-iteration notes
- traceability notes
- production learning notes

## Main risk avoided

Treating implementation as the end of learning.
