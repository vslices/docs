# VSlices Docs Standard glossary

This glossary defines concepts used by VSlices Docs Standard.

VSlices Docs Standard focuses on preserving useful knowledge through living documentation structures.

This glossary does not redefine every document type. Specific document types are explained in the Docs Standard taxonomy and in their own pages.

These terms help describe what kind of knowledge should be documented, why it matters, and how documents can remain connected to real work.

## Documentation concepts

- __Living documentation__: documentation that evolves together with the system, decisions, domain understanding, implementation, validation, and feedback.

- __Document structure__: the expected shape of a document, including its purpose, sections, relationships, and intended use.

- __Document type__: a reusable documentation form used to preserve a specific kind of knowledge, such as context, process, behavior, capability, decision, or validation.

- __Knowledge artifact__: a preserved piece of knowledge that future work may depend on, such as a document, note, diagram, decision, example, or validation result.

- __Documentation boundary__: the limit that defines what a document should explain and what should be left to another document.

## Relationship concepts

- __Document relationship__: a connection between documents that helps preserve traceability between context, decisions, processes, behaviors, capabilities, validation, and implementation.

- __Reference__: an explicit link from one document to another document, concept, decision, behavior, or artifact.

- __Traceability__: the ability to follow how knowledge moves between discovery, documentation, design, architecture, implementation, validation, and evolution.

- __Document stage__: the level of maturity, stability, or confidence a document currently represents.

- __Document affinity__: the natural relationship between a document type and the kind of work, knowledge, uncertainty, or lifecycle stage it best supports.

## Knowledge quality concepts

- __Useful knowledge__: knowledge that helps future work understand, decide, implement, validate, maintain, or evolve something more safely.

- __Preserved intent__: the reasoning, meaning, purpose, and constraints that should remain understandable after the original discussion or decision has passed.

- __Documentation drift__: the distance that appears when documentation and real system behavior evolve separately.

- __Outdated knowledge__: documented knowledge that no longer reflects the current understanding, behavior, decision, or implementation.

- __Documentation debt__: accumulated documentation gaps, outdated explanations, missing decisions, or disconnected knowledge that make future work harder.

## Relationship between the terms

VSlices Docs Standard helps teams preserve knowledge using the smallest useful document structure.

```text
Useful knowledge
-> Document type
-> Document structure
-> Document relationship
-> Traceability
-> Living documentation
```

This is not a requirement to document everything. A team should document the knowledge that future work depends on, using the smallest structure that preserves enough meaning, context, and intent.

The goal is not more documentation. The goal is less knowledge loss.
