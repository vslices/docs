# Context-First

Context-First is a VSlices Design modality that prioritizes broad domain understanding before defining concrete software artifacts.

It is useful when the team needs to understand the business context before deciding what should be built, improved, automated, integrated, or modernized.

Context-First assumes that software structure should emerge progressively from domain understanding.

It does not start from a preferred architecture, a technical pattern, a database model, a screen, an API, or a feature list. It starts from the context.

## Definition

Context-First is a design modality where the team builds a strong contextual base before moving toward implementation.

In the pyramid metaphor, Context-First gives more weight to the base than to the height.

```text
base / height -> large
```

This means the team invests more effort in Understanding and Contextualizing before Planning and Building.

The goal is not to analyze forever.

The goal is to reduce contextual uncertainty enough to make implementation decisions safer, clearer, and more traceable.

## When to use it

Use Context-First when the domain is not yet clear enough to safely define software structure.

It is especially useful when:

- the business process is unclear or fragmented
- several departments, areas, roles, or external actors participate
- the work currently happens through manual or semi-manual processes
- the system will modernize or replace an existing workflow
- the organization depends on implicit knowledge that is not documented
- different areas understand the same process differently
- the team needs to discover boundaries before designing features
- the cost of building the wrong thing is high
- implementation decisions may affect adjacent flows
- technical work depends on business understanding that is still missing

Context-First is also useful when the team is entering a domain for the first time.

## When not to use it

Context-First may be excessive when:

- the domain is already well understood
- the change is small and isolated
- the problem is already clear and bounded
- the team needs implementation feedback more than additional analysis
- the risk of building the wrong thing is low
- a previous iteration already created enough contextual base
- the work is mostly technical and does not require broad domain discovery

In those cases, Problem-First or Slice-First may be more appropriate.

## Characteristics

Context-First usually has these characteristics:

- broad exploration before narrow planning
- strong focus on domain language
- early identification of actors, areas, roles, and responsibilities
- attention to existing flows before target flows
- discovery of boundaries before implementation structure
- explicit treatment of uncertainty and assumptions
- slower initial movement toward implementation
- stronger traceability between business context and software artifacts
- high sensitivity to adjacent processes and organizational impact

Context-First does not try to model the entire business.

It tries to understand enough of the relevant business context to make better design decisions.

## Advantages

Context-First helps the team:

- reduce premature implementation
- avoid designing features from isolated requirements
- improve shared language
- reveal hidden dependencies
- detect adjacent flows and affected responsibilities
- discover domain boundaries
- understand why current processes behave as they do
- identify risks before they become implementation problems
- produce software artifacts supported by business context
- reduce accidental complexity caused by weak assumptions

It is especially valuable when the largest risk is misunderstanding the business.

## Disadvantages

Context-First also has costs. It may:

- slow down initial delivery
- require more access to domain experts
- feel too broad for small or urgent changes
- create too many artifacts if not kept progressive
- drift into analysis paralysis if the team does not define scope
- delay implementation feedback
- become difficult to manage when exploration has no stopping criteria

The main danger of Context-First is confusing understanding with endless discovery. The team should build enough base to move safely, not attempt to remove every possible uncertainty before building.
