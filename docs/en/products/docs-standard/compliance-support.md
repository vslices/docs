# Compliance support

VSlices Docs Standard prioritizes knowledge continuity over formal compliance.

It is not a certified implementation of any external standard and does not declare conformity with specific frameworks, standards, audits, or regulations. It can help prepare documentation that is easier to map to established standards, internal policies, audits, or compliance-oriented reviews.

!!! principle "Compliance principle"

    Preserve engineering knowledge first. Add compliance controls when the context requires them.


Teams that need formal compliance should use VSlices Docs Standard as a continuity layer and then add the artifacts, controls, reviews, evidence, and approval mechanisms required by their target standard.

## Position

VSlices Docs Standard is influenced by existing documentation, architecture, and traceability practices.

It does not implement them directly.

This page helps distinguish:

* **what VSlices can support**: areas where VSlices documentation already provides a useful structure
* **what VSlices can partially support**: areas where VSlices preserves related knowledge, but not the full required form
* **what needs to be added**: areas that require specific artifacts, controls, approvals, or evidence

## Support summary

The following table does not declare conformity.

It only shows areas where VSlices documents can serve as a basis for preparing, mapping, or complementing documentation required by external references.

!!! risk "Risk to avoid"

    Do not use this table as automatic evidence of formal compliance.


| External reference | Can support                                                                    | Can partially support                                                 | Needs to add                                                            |
| ------------------ | ------------------------------------------------------------------------------ | --------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| ISO/IEC/IEEE 42010 | Context, concerns, rationale, decisions, and documentary relationships.        | Viewpoints, views, correspondences, and architecture descriptions.    | Conformant architecture description framework.                          |
| ISO/IEC/IEEE 29148 | Expected behavior, assumptions, expected errors, and lightweight traceability. | Quality attributes, verification, and formal requirements management. | Formal process for specification, review, verification, and management. |
| arc42              | Context, decisions, risks, glossary, and documentary continuity.               | Runtime, deployment, and building block views.                        | Complete arc42 structure.                                               |
| C4 Model           | System context and boundary awareness.                                         | Container, component, and code views.                                 | Complete C4 notation, visual hierarchy, and conventions.                |
| ADR                | Decision rationale, tradeoffs, and consequences.                               | Formal lifecycle for architecture decisions.                          | Strict ADR template, governance, or approval process.                   |
| 4+1 Model          | Scenarios and use case-oriented reasoning.                                     | Logical, process, development, and physical views.                    | Complete 4+1 architectural view model.                                  |

## How to use this

Use this document to understand how VSlices Docs Standard can support alignment with external standards, architecture templates, client policies, audit expectations, or regulatory requirements.

VSlices can preserve knowledge that those external requirements may also need, but it does not make that knowledge conformant by itself.

When a team needs to align with an external requirement:

1. **Start with VSlices Docs Standard**
   Preserve the real engineering knowledge first: context, processes, behavior, capabilities, decisions, validation, and evolution.

2. **Identify the target requirement**
   Clarify which standard, framework, client policy, audit expectation, or regulatory requirement must be satisfied.

3. **Map existing documents**
   Connect VSlices documents with the artifacts requested by the target requirement.

4. **Identify missing evidence or controls**
   Find what the target requirement needs and VSlices does not provide by default, such as approvals, review cycles, formal traceability, required diagrams, audit evidence, or specific formats.

5. **Extend without disconnecting**
   Add the required compliance material while keeping it linked to the original engineering knowledge.

## What this page should not do

This page should not be used to claim that VSlices Docs Standard complies with an external standard.

It also does not replace:

* legal review
* compliance review
* formal audit
* architecture approval
* organizational controls
* specific regulatory evidence
* mandatory templates from a client or industry

Its purpose is to show how VSlices documentation can serve as a continuity basis for preparing that work.

## Usage rule

!!! principle "Compliance principle"

    Do not use it as a substitute for review, evidence, approval, or formal conformity.


Use VSlices Docs Standard to preserve engineering knowledge that can support compliance work.
