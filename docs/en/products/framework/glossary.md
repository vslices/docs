# VSlices Framework glossary

This glossary defines terms used by VSlices Framework.

VSlices Framework focuses on implementing domain-oriented software with explicit behavior, explicit errors, functional composition, progressive architecture, and low ceremony.

These terms help connect domain knowledge, application behavior, runtime requirements, and executable structure.

## Execution concepts

- __Flow__: an executable composition that describes how work, data, behavior, dependencies, and expected errors move through an operation.

- __Feature__: a concrete behavior, action, or vertical slice that delivers value or supports a validated need inside a domain context.

- __Step__: a small unit of executable behavior inside a flow, usually responsible for one meaningful transformation, validation, decision, or side effect.

- __Pipeline__: an ordered composition of steps, behaviors, effects, validations, or transformations that produce a result.

## Domain modeling concepts

- __Domain Type__: a strongly modeled value that represents a domain concept with explicit validation, meaning, and invariants.

- __Invariant__: a rule that must remain true for a domain type, behavior, capability, or state to be considered valid.

- __Runtime Validation__: the act of checking whether a value, behavior, command, request, or state satisfies expected rules before continuing.

- __Expected error__: a known failure condition that belongs to the domain or application flow and should be modeled explicitly instead of treated as an unexpected exception.

- __Unexpected error__: a failure that was not part of the expected domain or application flow, usually caused by infrastructure, defects, unavailable dependencies, or invalid assumptions.

## Composition concepts

- __Capability__: a stable ability required by the business or system. In Framework, a capability may be represented through explicit contracts, implementations, dependencies, or composable behaviors.

- __Trait__: a composable unit of behavior or ability that can be attached, combined, or reused without relying on inheritance-heavy models.

- __Effect__: an explicit representation of work that may require dependencies, produce results, fail, or interact with the outside world.

- __Functional composition__: the practice of building behavior by composing smaller functions, effects, validations, and transformations into larger executable structures.

- __Runtime requirement__: an explicit dependency or environmental requirement needed by a flow, feature, effect, or operation during execution.

## Integration concepts

- __Integrator__: a mechanism that invokes a feature from a specific interaction style, such as an HTTP endpoint, CLI command, background job, UI action, timed job, or event handler.

- __Adapter__: a technology-specific implementation that connects VSlices concepts to external frameworks, libraries, platforms, infrastructure, or providers.

- __Provider__: an external or internal capability source used by an adapter, feature, integration, or runtime behavior.

- __Port__: a contract that describes what a feature, capability, adapter, or external dependency needs without binding the domain behavior to a specific technology.

## Error and result concepts

- __Result__: an explicit outcome of an operation, usually representing either success or failure without requiring exceptions for normal control flow.

- __Error as value__: the practice of representing expected failures as explicit values that can be composed, returned, matched, logged, tested, and documented.

- __Failure path__: the route an operation takes when an expected error, validation failure, dependency issue, or unexpected problem prevents normal completion.

- __Success path__: the route an operation takes when all required validations, dependencies, decisions, and effects complete as expected.

## Relationship between the terms

VSlices Framework attempts to keep executable software close to domain intent.

```text
Domain Type
-> Feature
-> Flow
-> Runtime requirement
-> Expected error
-> Result
```

This does not mean every implementation needs every concept. A small feature may only need a domain type, a simple flow, and an explicit result. More structure should appear only when the domain, behavior, or runtime needs justify it.

The goal is not to add framework ceremony. The goal is to make behavior, dependencies, errors, and domain meaning explicit enough to be composed, tested, and evolved safely.
