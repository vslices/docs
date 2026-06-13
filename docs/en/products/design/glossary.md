# VSlices Design glossary

This glossary defines terms used by VSlices Design.

VSlices Design focuses on reasoning, modeling, uncertainty, boundaries, and progressive understanding before committing too early to architecture or implementation.

These terms help describe how design work can begin from different kinds of available knowledge.

## Design concepts

- __Design modality__: a way of approaching design work depending on the current uncertainty, available knowledge, and safest next step.

- __Context-First__: a design modality that starts by understanding the surrounding business, operational, organizational, or system context before narrowing into a specific problem or implementation.

- __Problem-First__: a design modality that starts from a concrete tension, need, risk, question, or failure that must be understood before deciding what to build.

- __Slice-First__: a design modality that starts from a small useful slice of work to learn from implementation, validation, or real usage.

## Supporting concepts

- __Modeling heuristic__: a practical reasoning aid used to make domain knowledge, uncertainty, responsibilities, or boundaries easier to observe and discuss.

- __Design reasoning__: the process of understanding why a structure, boundary, behavior, document, or implementation direction may be appropriate for the current context.

- __Uncertainty__: a lack of reliable understanding about the domain, problem, behavior, responsibility, risk, or expected outcome.

- __Boundary reasoning__: the act of using boundaries as reasoning objects to identify where concepts, responsibilities, decisions, systems, actors, or ownership areas should be separated.

- __Progressive understanding__: the gradual improvement of domain and system knowledge through discovery, documentation, modeling, implementation, validation, and feedback.

## Relationship between design modalities

The design modalities describe different starting points for design work.

```text
Context-First
-> start from the surrounding situation

Problem-First
-> start from a concrete tension or need

Slice-First
-> start from a small useful implementation or validation slice
```

They are not maturity levels and they are not a fixed sequence.

A team may start Context-First when the environment is unclear, Problem-First when a specific tension is visible, or Slice-First when building a small piece is the safest way to learn.

The important part is choosing the modality that matches the uncertainty of the current work.
