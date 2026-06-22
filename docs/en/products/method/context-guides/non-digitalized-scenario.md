# Scenario "Not digitized"

A "Not digitized" scenario is a work context where important work is not yet represented by software.

The work may happen through conversations, spreadsheets, paper documents, messages, meetings, manual coordination, or informal routines.

This does not mean the work is simple. It means the knowledge needed to support it may still be implicit, distributed, or unstable.

## Core idea

!!! principle "Continuity Principle"

    In a not digitized scenario, VSlices Method helps the team understand how the work currently happens before deciding what should become software.


The goal is not to document everything. It is to discover enough domain, process, and decision context to avoid automating a misunderstood reality.

## When this guide applies

Use this guide when:

* no software currently supports the work
* the existing software is not related to the work being studied
* the work is coordinated manually
* knowledge lives mainly in people, documents, or habits
* workflows are informal or inconsistent
* different people explain the same work in different ways
* the team is asked to create a new system, module, or capability from scratch

This guide can apply to a complete project, a work line, or a single area of business behavior.

## Main risk

The main risk is automating a process the team does not yet understand.

A not digitized scenario may contain:

* implicit rules
* informal responsibilities
* exceptions handled from memory
* language that changes between people
* decisions hidden in habits
* manual validations
* workarounds that reveal real constraints
* process steps that exist only because there is no better support

!!! risk "Risk to avoid"

    If the team starts designing software too early, it may turn temporary habits into permanent system behavior.
  

## Useful initial modality

A not digitized scenario usually starts with [**Context-First**](../../design/modalities/context-first/index.md), because the team still needs to understand how the work happens before deciding what should become software.

| Situation                                                    | Useful modality                                                     | Reason                                                                         |
| ------------------------------------------------------------ | ------------------------------------------------------------------- | ------------------------------------------------------------------------------ |
| The team does not understand how the work currently happens. | **Context-First**                                                   | The next decision needs a broader understanding of the domain and process.     |
| There is a clear pain inside the manual work.                | [**Problem-First**](../../design/modalities/problem-first/index.md) | The team can focus on understanding the problem without assuming the solution. |
| A small experiment can reveal how people react to support.   | [**Slice-First**](../../design/modalities/slice-first/index.md)     | The team can learn through a bounded prototype or a vertical slice.            |

!!! risk "Risk to avoid"

    Slice-First should be used carefully in this scenario.

    A small slice is useful only when it helps the team learn without pretending that the whole context is already understood.


## What to observe first

Before designing software, observe how people currently perform the work.

| Observe                                                     | To understand                                                             |
| ----------------------------------------------------------- | ------------------------------------------------------------------------- |
| Who participates in the work                                | Which roles, people, or areas sustain the process.                        |
| What activates the work                                     | Which event, need, or decision starts the process.                        |
| What result is expected                                     | What it means for the work to be completed correctly.                     |
| Which steps repeat                                          | Which behavior may need stable structure.                                 |
| What changes from one case to another                       | Which variations should not be lost when digitizing.                      |
| Which terms people use                                      | Which domain language should be preserved.                                |
| Where delays, errors, or misunderstandings happen           | Which frictions reveal real risks.                                        |
| Which decisions are made during the work                    | Which knowledge should not remain implicit.                               |
| Which validations are performed manually                    | Which rules may need to become explicit.                                  |
| Which exceptions are common                                 | Which special cases should be understood early.                           |
| Which information is created, transformed, or shared        | Which data sustains the work.                                             |
| Which parts exist only because there is no software support | Which habits may be temporary and should not be automated without review. |

The goal is not to model the process perfectly. It is to find enough structure to make the next decision with more confidence.

## Knowledge to preserve

Preserve knowledge when it affects what should be built, avoided, or investigated later.

Useful knowledge may include:

* domain terms and conflicting meanings
* actors and responsibilities
* current workflows
* recurring problems
* manual decisions
* validations and expected errors
* important exceptions
* business rules hidden in the routine
* documents, spreadsheets, or messages used as coordination tools
* open questions and uncertainty

!!! principle "Continuity Principle"

    Do not keep every observation.

    Preserve what future work should not have to rediscover.


## Documentation support

Documents can help make implicit work visible.

| Knowledge need                                            | Useful document                                                                                                                                                                         |
| --------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| People use terms inconsistently.                          | Domain Vocabulary — [Taxonomy](../../docs-standard/taxonomy/domain-vocabulary.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/domain-vocabulary.md)       |
| The surrounding scenario needs to be understood.          | Context Document — [Taxonomy](../../docs-standard/taxonomy/context-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/context-document.md)          |
| The work depends on steps, handoffs, or responsibilities. | Process Document — [Taxonomy](../../docs-standard/taxonomy/process-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/process-document.md)          |
| A behavior should be supported by software.               | Use Case Document — [Taxonomy](../../docs-standard/taxonomy/use-case-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/use-case-document.md)       |
| A stable business ability is emerging.                    | Capability Document — [Taxonomy](../../docs-standard/taxonomy/capability-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/capability-document.md) |
| A direction must be chosen under tradeoffs.               | Decision Record — [Taxonomy](../../docs-standard/taxonomy/decision-record.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/decision-record.md)             |
| Early evidence changes what the team believes.            | Validation Note — [Taxonomy](../../docs-standard/taxonomy/validation-note.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/validation-note.md)             |
| Observations are still uncertain, local, or temporary.    | Support Note — [Taxonomy](../../docs-standard/taxonomy/support-note.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/support-note.md)                      |

Use documents to preserve understanding, not to formalize everything too early.

{% include-markdown "shared/readings/document-stage-affinity-admonition.md" %}

## Suggested approach

Start by choosing one area of work to understand.

Do not try to model the whole organization first. A useful approach is to:

1. Identify the scenario or work line being explored.
2. Observe how the work happens today.
3. Capture language, actors, workflows, decisions, and uncertainty.
4. Identify recurring pains, risks, or opportunities.
5. Keep only the knowledge needed for the next responsible decision.
6. Decide the next useful modality: keep understanding the context, clarify a problem, or build a small slice.
7. Use feedback to update the shared context.

The team should move gradually from observation toward decision.

## Common mistakes

Not digitized scenarios often fail when teams jump from conversation to solution.

Common mistakes include:

* designing screens before understanding the work
* treating one person's explanation as if it were the whole process
* ignoring exceptions because they seem rare
* automating manual habits that should be improved instead of copied
* assuming informal work has no structure
* documenting everything before deciding anything
* building a complete system before validating a small part
* using software concepts before the domain language is clear

!!! risk "Do not confuse evidence with design"

    Manual work shows how the current reality operates.

    It does not mean that reality should be copied into software as-is.


## Guiding principle

!!! principle "Continuity principle"

    Understand the work before representing it.

    Preserve enough context, language, process, and decision knowledge to avoid turning temporary habits into permanent software.

Build only when the team can explain which reality the software should support or improve.
