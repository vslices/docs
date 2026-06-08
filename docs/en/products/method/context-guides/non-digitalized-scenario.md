# Non-Digitalized Scenario

A non-digitalized scenario is a working context where important work is not yet represented by software.

The work may happen through conversations, spreadsheets, paper documents, messages, meetings, manual coordination or informal routines.

This does not mean the work is simple. It means the knowledge needed to support it may still be implicit, distributed or unstable.

## Core idea

In a non-digitalized scenario, VSlices Method helps the team understand how work currently happens before deciding what should become software.

The goal is not to document everything. It is to discover enough domain, process and decision context to avoid automating a misunderstood reality.

## When this guide applies

Use this guide when:

* no software currently supports the work
* existing software is unrelated to the work being studied
* work is coordinated manually
* knowledge lives mostly in people, documents or habits
* workflows are informal or inconsistent
* different people explain the same work differently
* the team is asked to create a new system, module or capability from scratch

This guide can apply to a full project, a work line or a single area of business behavior.

## Main risk

The main risk is automating a process the team does not understand. A non-digitalized scenario may contain:

* implicit rules
* informal responsibilities
* exceptions handled by memory
* language that changes between people
* decisions hidden in habits
* manual validations
* workarounds that reveal real constraints
* process steps that exist only because no better support exists

If the team starts by designing software too early, it may turn temporary habits into permanent system behavior.

## Useful starting modality

A non-digitalized scenario usually starts with **Context-First**.

| Situation                                                         | Modality   | Reason                                                                         |
| ----------------------------------------------------------------- | ----------------- | ------------------------------------------------------------------------------ |
| The team does not understand how work<br/>currently happens.          | [**Context-First**](../../design/modalities/context-first/index.md) | The next decision needs broader<br/>domain and process understanding.              |
| A clear pain exists inside the manual<br/>work.                       | [**Problem-First**](../../design/modalities/problem-first/index.md) | The team can focus on understanding<br/>the problem without assuming the<br/>solution. |
| A small experiment can safely reveal how<br/>people react to support. | [**Slice-First**](../../design/modalities/slice-first/index.md)   | The team can learn through a narrow<br/>prototype or vertical slice.               |

Slice-First should be used carefully. A small slice is useful only when it helps learning without pretending the whole context is understood.

## What to observe first

Before designing software, observe how people currently perform the work. Useful questions include:

* Who participates in the work?
* What triggers the work?
* What result is expected?
* What steps are repeated?
* What changes from case to case?
* What terms do people use?
* Where do delays, mistakes or misunderstandings happen?
* What decisions are made during the work?
* What validations are performed manually?
* What exceptions are common?
* What information is created, transformed or shared?
* Which parts of the work exist only because there is no software support?

The objective is not perfect process modeling. Is finding enough structure to make the next decision safer.

## Knowledge to preserve

Preserve knowledge when it affects what should be built, avoided or investigated next. Useful knowledge may include:

* domain terms and conflicting meanings
* actors and responsibilities
* current workflows
* repeated problems
* manual decisions
* validations and expected errors
* important exceptions
* business rules hidden in routine
* documents, spreadsheets or messages used as coordination tools
* open questions and uncertainty

Do not preserve every observation. Preserve what future work should not have to rediscover.

## Document support

Documents may help make implicit work visible.

| Knowledge need                                        | Useful document         |
| ----------------------------------------------------- | ----------------------- |
| People use terms inconsistently.                      | [Domain Vocabulary](../../docs-standard/taxonomy/domain-vocabulary.md)   |
| The surrounding scenario needs to be understood.      | [Context Document](../../docs-standard/taxonomy/context-document.md)    |
| Work depends on steps, handoffs or responsibilities.  | [Process Document](../../docs-standard/taxonomy/process-document.md)    |
| A behavior should be supported by software.           | [Use Case Document](../../docs-standard/taxonomy/use-case-document.md)   |
| A stable business ability is emerging.                | [Capability Document](../../docs-standard/taxonomy/capability-document.md) |
| A direction must be chosen under tradeoffs.           | [Decision Record](../../docs-standard/taxonomy/decision-record.md)     |
| Early evidence changes what the team believes.        | [Validation Note](../../docs-standard/taxonomy/validation-note.md)     |
| Observations are still uncertain, local or temporary. | [Support Note](../../docs-standard/taxonomy/support-note.md)        |

Use documents to preserve understanding, not to formalize everything too early.

> Document affinity by iteration stage is described in the [Document-Stage affinity](../document-stage-affinity.md) page.

## Suggested approach

Start by choosing one area of work to understand.

Do not try to model the whole organization first. A useful approach is:

1. Identify the scenario or work line being explored.
2. Observe how work happens today.
3. Capture language, actors, workflows, decisions and uncertainty.
4. Identify repeated pain, risk or opportunity.
5. Preserve only the knowledge needed for the next responsible decision.
6. Choose whether to continue understanding, clarify a problem or build a small slice.
7. Use feedback to update the shared context.

The team should move gradually from observation to decision.

## Common mistakes

Non-digitalized scenarios commonly fail when teams rush from conversation to solution. Common mistakes include:

* designing screens before understanding work
* treating one person's explanation as the whole process
* ignoring exceptions because they seem rare
* automating manual habits that should be improved instead
* assuming informal work has no structure
* documenting everything before deciding anything
* building a full system before validating a small part
* using software concepts before domain language is clear

Manual work should be respected as evidence. It should not be copied blindly into software.

## Guiding principle

Understand the work before representing it.

Preserve enough context, language, process and decision knowledge to avoid turning temporary habits into permanent software.

Build only when the team can explain what reality the software is meant to support or improve.
