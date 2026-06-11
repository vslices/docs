# 0008 - Use template generation as the first Slice-First sample

## Status

Accepted

## Context

VSlices documentation is growing across multiple products, versions and languages.

This creates a maintenance problem. For example, a single documentation idea may need to exist across:

* English documentation
* Spanish documentation
* product-specific sections
* versioned documentation
* generated markdown files
* public documentation pages

Maintaining these files manually creates duplicated effort and increases the risk of divergence.

At the same time, VSlices needs real examples to validate its own method, documentation standard, design reasoning and framework primitives.

The documentation generator is a small but real problem observed inside VSlices itself. Because of that, it is a strong candidate for the first Slice-First sample.

## Decision

We will use the documentation template generator as the first Slice-First sample for VSlices.

- The objective is not to build a complete documentation platform.
- The objective is to solve the immediate problem of generating consistent documentation artifacts from a smaller source of truth.

This sample should validate how VSlices approaches a concrete slice from:

* observed problem
* documentation need
* design reasoning
* implementation
* feedback
* evolution

## Rationale

The generator is useful immediately. It supports current v0.1 work and reduces manual documentation maintenance. It also creates a realistic but bounded scenario for validating VSlices.

This makes it better than an artificial sample. The slice is small enough to keep scope controlled, but meaningful enough to involve:

* documentation structure
* source content
* transformation rules
* generated markdown
* language variants
* validation feedback
* implementation decisions

## Slice Definition

The initial slice is:

> Generate documentation files from structured template content in order to reduce duplicated manual maintenance across documentation variants.

The first version should focus on the smallest useful workflow:

* define source content
* define output targets
* generate markdown files
* support at least one repeated documentation structure
* keep the generated output readable and editable
* avoid unnecessary platform features

## Explicit Non-Goals

This decision does not commit to building:

* a full documentation CMS
* a visual editor
* a complete localization platform
* a public product
* a complex template language
* a generic static site generator
* a full Surreal Atlas prototype

Those may become future explorations only if the initial slice validates the need.

## Consequences

### Positive consequences

* VSlices gets a real Slice-First example.
* Documentation maintenance becomes easier.
* Framework examples can be derived from actual internal usage.
* Docs Standard can be validated through generation constraints.
* Method can be tested against a concrete implementation path.
* The sample may later inform Surreal Knowledge Manager or Surreal Atlas.

### Negative consequences

* The generator may temporarily distract from finishing v0.1-beta.
* There is a risk of overgeneralizing the tool too early.
* There is a risk of building a platform instead of solving the current documentation problem.
* The first implementation may need to be rewritten after learning from usage.

### Tradeoff

We accept a small implementation effort now because the generator solves a current documentation problem and provides a concrete Slice-First validation case.

We do not accept expanding the generator beyond the current documentation need until it proves useful.

## Validation Strategy

This decision will be validated if the generator helps:

* reduce duplicated documentation work
* keep English and Spanish documentation more consistent
* generate useful markdown outputs
* reveal better Docs Standard structures
* produce examples that can explain VSlices Method and Framework
* support v0.1 documentation without increasing complexity

This decision will be weakened if:

* manual editing remains easier than generation
* generated documents become harder to understand
* the generator requires too much ceremony
* the tool becomes more complex than the documentation problem
* the implementation blocks v0.1-beta progress

## Notes

The generator should follow VSlices principles:

* solve a real problem first
* keep the first slice small
* prefer explicit behavior
* avoid hidden magic
* preserve human-readable documentation
* introduce complexity progressively

The generator is a validation tool before it is a product.
