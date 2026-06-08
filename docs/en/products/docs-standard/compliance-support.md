# Compliance Support

VSlices Docs Standard prioritizes knowledge continuity over formal compliance. It is not a certified implementation of any external standard.

It can, however, help teams prepare documentation that is easier to map toward established standards, architecture documentation practices, and compliance-oriented reviews.

Teams that require formal compliance should use VSlices Docs Standard as a continuity layer, then add the specific artifacts, controls, reviews, evidence, and approval mechanisms required by their target standard.

## Position

VSlices Docs Standard is influenced by existing documentation and architecture practices.

It does not directly implement them. It is to be honest about:

* **what VSlices supports**: areas where VSlices documents already provide useful structure.
* **what VSlices partially supports**: areas where VSlices provides related knowledge, but not the full required form.
* **what VSlices does not provide**: areas that require additional compliance-specific artifacts or controls.

## Standard/Practice support overview

| Standard               | Supports                                                                                                       | Partially supports                                            | Does not provide                                       |
| ---------------------- | -------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------ |
| ISO/IEC/IEEE<br/>42010 | <ul><li>Context</li><li>Concerns</li><li>Rationale</li><li>Decisions</li><li>Relationships</li></ul>           | <ul><li>Viewpoints</li><li>Views</li><li>Correspondences</li><li>Architecture<br/>descriptions</li><ul> | Full conforming architecture<br/>description framework     |
| ISO/IEC/IEEE<br/>29148 | <ul><li>Behavior</li><li>Validation</li><li>Assumptions</li><li>Expected errors</li><li>Traceability</li></ul> | <ul><li>Requirement quality<br/>attributes</li><li>Verification links</li><ul>         | Full requirements specification<br/>and management process |

| Principio           | Supports                                                                                     | Partially supports                                                                  | Does not provide                               |
| ------------------ | -------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------- |
| arc42              | <ul><li>Context</li><li>Decisions</li><li>Risks</li><li>Glossary</li><li>Continuity</li><ul> | <ul><li>Runtime</li><li>Deployment</li><li>Building block views</li><ul>            | Complete arc42 structure<br/>by default         |
| C4 Model           | <ul><li>Context-level thinking</li><li>Boundary awareness</li></ul>                          | <ul><li>Container</li><li>Component</li><li>Code views</li></ul>                    | Diagram notation and visual<br/>model hierarchy |
| ADR                | <ul><li>Decision reasoning</li><li>Tradeoffs</li><li>Consequences</li></ul>                  | <ul><li>Architecture-specific<br/>decision lifecycle</li><ul>                       | A strict ADR template or<br/>governance process |
| 4+1 View<br/>Model | <ul><li>Scenarios</li><li>Use-case<br/>oriented thinking</li><ul>                            | <ul><li>Logical</li><li>Process</li><li>Development</li><li>Physical views</li><ul> | Complete 4+1 architecture<br/>view model        |

## How to use this

Use this document as a mapping aid. Do not treat it as proof of compliance. For compliance-oriented work:

* **start with VSlices Docs Standard**: preserve continuity between domain, documentation, decisions, implementation, and validation.
* **identify the target standard**: clarify which external standard, framework, customer requirement, or regulatory expectation applies.
* **map VSlices documents to required artifacts**: reuse existing knowledge instead of rewriting everything from scratch.
* **add missing controls**: include required approvals, traceability, evidence, review cycles, formats, or diagrams.
* **keep continuity visible**: avoid producing compliance artifacts that become disconnected from real engineering knowledge.

## Principle

VSlices Docs Standard should help teams become more prepared for compliance. It should not pretend to replace compliance.

> Preserve knowledge first. Add compliance controls when the context requires them.
