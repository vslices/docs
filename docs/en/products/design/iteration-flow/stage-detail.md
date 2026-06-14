# Design Iteration Flow Detail

## 1. Understanding

Understanding is the stage where the team extracts domain knowledge.

The team explores the business context by listening to domain experts, observing existing work, identifying vocabulary, discovering concepts, and detecting relevant flows.

This stage is related to the inverted pyramid, where business is treated as a wide surface of domain knowledge. And to understand a specific objective, the team must remove the grains of sand that cover it. Removing grains means understanding them.

The team asks:

- What concepts appear repeatedly?
- Who participates in this part of the business?
- What language do domain experts use?
- What flows already exist?
- What problems are visible?
- What assumptions are we making?
- What do we still not understand?

The goal is not to model everything. It is to understand enough to continue with better questions.

### Common supporting artifacts

- glossary
- concept notes
- domain interview notes
- actor list
- open questions
- assumption list
- early flow sketches

### Main risk avoided

Designing artifacts before understanding the world they belong to.

## 2. Contextualizing

Contextualizing is the stage where the team organizes discovered knowledge into a visible base scenario.

This stage is related to the base of the construction pyramid, where the team takes the sand extracted during Understanding and starts placing it on the construction site.

The objective is to make the current context understandable, and it may include:

- relevant areas or departments
- actors and responsibilities
- current flows
- current systems
- current pain points
- current boundaries
- relevant business language
- relationships between concepts

Contextualizing does not define the final solution, its purpose is to make the current situation visible enough to support better decisions.

The team asks:

- What is the current scenario?
- How does work move today?
- Which areas, actors, or systems participate?
- Which flows surround the objective?
- Which concepts are foundational?
- Which boundaries are starting to appear?
- What should be preserved as shared understanding?

A strong base makes later decisions safer. Without enough contextual base, later artifacts may look precise but remain unstable.

### Common supporting artifacts

- current scenario notes
- flow sketches
- swimlane diagrams
- responsibility map
- context map
- concept relationship notes
- pain point list
- boundary notes

### Main risk avoided

Treating a problem, use case, or feature as isolated when it actually belongs to a larger context.

## 3. Planning

Planning is the stage where the team decides how the current situation should improve.

The team uses the contextual base to identify which part of the business should change and why. This stage shifts the mind-set:

> What is happening? -> What should become better?

Planning focuses on:

- business impact
- feasibility
- risk
- scope
- tradeoffs
- affected flows
- possible improvements

The team asks:

- Which problems are worth solving now?
- Which improvement creates meaningful business value?
- Which adjacent flows could be affected?
- What risks or mitigations exist?
- What should remain outside the current iteration?
- What would the improved scenario look like?
- Which use cases, processes, capabilities, or services may be needed?

The output of Planning should be precise enough to guide implementation without pretending that every future detail is already known.

### Common supporting artifacts

- improvement proposal
- target scenario notes
- scope notes
- tradeoff notes
- risk notes
- decision notes
- affected flow list
- use case sketches
- target process sketches

### Main risk avoided

Solving the most attractive technical problem instead of the most relevant business problem.

## 4. Building

Building is the stage where the planned improvement becomes real. This includes development, integration, validation, delivery, and feedback.

In this stage, design artifacts are translated into implementation decisions. The team may define or implement:

- features
- flows
- capabilities
- domain types
- integrations
- services
- expected errors
- deployment changes
- operational adjustments

Building is not separate from understanding. It tests the understanding accumulated so far.

When the team builds, it discovers whether the previous stages were clear enough, incomplete, or wrong.

The result of Building produces business value, but it also produces new knowledge.

That new knowledge becomes material for the next iteration.

The team asks:

- What needs to be implemented now?
- Which assumptions are being tested?
- Which design artifacts are guiding the implementation?
- What new constraints appeared during development?
- What changed after delivery?
- What did the team learn?
- What should be explored next?

### Common supporting artifacts

- feature notes
- implementation notes
- validation notes
- delivery notes
- feedback notes
- technical decision notes
- discovered constraint notes
- next-iteration notes

### Main risk avoided

Treating implementation as the end of learning.

## Returning to Understanding

The iteration does not end after Building, in fact, it returns to Understanding.

Every delivered improvement changes the business context.

- A new feature may create new workflows.
- A new workflow may reveal new responsibilities.
- A new responsibility may expose new risks.
- A new risk may require new planning.
- A new production behavior may challenge previous assumptions.

This is why VSlices Design treats iteration as a loop.

```text
Understanding -> Contextualizing -> Planning -> Building -> Understanding
```

The team does not return to the beginning because it failed. It returns because the domain has evolved.
