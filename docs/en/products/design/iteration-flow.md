# Design Iteration Flow

VSlices Design uses a recurring iteration flow:

```text
Understanding -> Contextualizing -> Planning -> Building -> Understanding
```

This flow is shared by all VSlices Design modalities, the stages are always the same across modalities, but the emphasis changes.

- Some situations require more understanding before planning.
- Some situations require a stronger contextual base before building.
- Some situations require faster implementation feedback.

That is why VSlices Design uses modalities, they do not replace the iteration flow, they only change how much attention each stage receives.

## Relationship with the pyramids

The iteration flow uses the two metaphors explained in `understanding.md`:

- inverted pyramid
- construction pyramid

Each stage of the iteration flow can be understood through those metaphors.

| Stage           | Main metaphor               | Purpose                                |
| --------------- | --------------------------- | -------------------------------------- |
| Understanding   | Inverted pyramid            | Extract domain knowledge               |
| Contextualizing | Construction pyramid base   | Build the base scenario                |
| Planning        | Construction pyramid middle | Decide the intended improvement        |
| Building        | Construction pyramid height | Implement, validate, and deliver value |

The flow is cyclical.

After Building, the team returns to Understanding because every delivered change modifies the context and creates new knowledge.

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

The goal is not to model everything, it is to understand enough to continue with better questions.

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

Contextualizing does not define the final solution, its purpose to make the current situation visible enough to support better decisions.

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

## Modalities and stage emphasis

All VSlices Design modalities use the same iteration flow, they change the emphasis.

> Context-First gives more weight to Understanding and Contextualizing.
> Problem-First gives more weight to Planning while keeping enough Understanding and Contextualizing around the problem.
> Slice-First gives more weight to Building so the team can learn quickly from a small vertical implementation.

The modality should match the kind of uncertainty and context the team is facing.

| Modality      | Main emphasis                     | Useful when                                                           |
| ------------- | --------------------------------- | --------------------------------------------------------------------- |
| Context-First | Understanding and Contextualizing | The domain is unclear, broad, fragmented, or organizationally complex |
| Problem-First | Planning with enough context      | A clear problem exists, but its surrounding context still matters     |
| Slice-First   | Building and feedback             | The team can learn faster from a small working slice                  |

## Readiness to build

Building can start when the team has enough clarity to make implementation decisions without relying only on assumptions.

This does not mean that every detail must be known, just means that the team can explain:

- what is being improved
- why it matters
- what context supports the decision
- which concepts are involved
- which flows or responsibilities are affected
- what the intended outcome is
- what uncertainty remains

A feature should not appear as an isolated decision. It should be the visible result of a path that started from broader understanding.

## Complexity rule

The iteration flow should remain progressive, the team should not create every possible artifact in every iteration.

The level of detail should grow only when it helps:

- preserve understanding
- reduce risk
- clarify decisions
- guide implementation
- protect business intent

Small domains may need only lightweight notes and simple diagrams. Complex domains may require deeper analysis, modeling, and documentation.

The flow should adapt to the domain. The domain should never be forced to adapt to the flow. VSlices Design is not a bureaucratic funnel.

It is a way to make sure concrete software is supported by enough contextual understanding. The team should move deliberately, it may be slow or fast, but it needs to be deliberately.

## Clarifications

### About artifacts 

Supporting artifacts are optional aids. They are not mandatory documents.

A team should create them only when they help preserve understanding, reduce risk, clarify decisions, or guide implementation.

### About modality switching

A team can switch modalities between iterations.

Starting with Context-First does not force the team to remain Context-First forever.

As uncertainty changes, the modality can change too.
