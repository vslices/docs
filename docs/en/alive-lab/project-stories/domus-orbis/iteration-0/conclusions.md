# Conclusions from Iteration 0

## Purpose

This document summarizes the learnings obtained during Iteration 0 of Domus Orbis and explains how those learnings can influence the evolution of VSlices.

It does not aim to repeat the step-by-step story of the iteration. Its objective is to extract methodological, documentation, design, and tooling conclusions from a real case.

## Use of AI during the iteration

AI was used as a working counterpart.

It helped to:

* organize the problem;
* detect overscope;
* propose documents;
* draft initial versions;
* review whether a solution belonged to Iteration 0 or to a future evolution;
* transform conversation into documentation;
* maintain focus on the current need.

AI did not replace domain observation. The real need came from the everyday use of the home.

In this case, AI worked as support for preserving continuity, not as an automatic source of truth.

### Open questions

* How could we generate an AI agent that directly supports the application of Method?
* Would it be possible to generate an AI agent that helps observe which things can extend our products?

## What was discovered

Iteration 0 left several learnings.

First, the real problem was not automating purchases. It was that the monthly list had to exist before payment.

Second, a small solution could provide value without becoming an application yet.

Third, the documentation had to live close to the project because its objective was to help resume the work later.

Fourth, the necessary documents depended on the scope. Not every phase needed the same number of documents.

Fifth, the initial *artifact* had to be small, but not disposable. Even if tools, integrations, or automation appear later, the centralized list remains a useful piece.

## What could be done differently depending on context

This case was small, personal, and urgent.

That is why some documents were lightweight notes and some *artifacts* were enough without a formal usage guide. In another context, this could change.

A project with more people could need:

* explicit decisions
* usage guides
* more formal validations
* additional diagrams
* stakeholder review
* stricter acceptance criteria

A project with more technical risk could need:

* integration tests
* technical spikes
* architecture decisions
* external provider validation
* rollback strategy

A project with greater economic impact could require:

* authorization controls
* auditability
* traceability
* human confirmations
* operational limits

Domus Orbis does not define a universal recipe. It shows how the minimum useful document set was selected for this scope.

### Open questions

* How does economic impact affect VSlices products?
* How does technical risk affect them?
* How does team size affect them?
* How does project timeline affect them?

## Document selection

One of the most important observed rules was:

> No phase of VSlices Method has a fixed number of documents.

Documents are selected according to the scope, risk, uncertainty, and responsibility of the phase.

In Domus Orbis, given its more casual and personal nature, a single person fulfilled several roles at the same time. That context did not require documenting boundaries constantly.

This is mentioned because another project may require greater emphasis on boundaries if it has more people involved, more concepts in play, or a less casual and more formal profile.

### Open questions

* Which project characteristics affect which parts of the documentation?

## Use of the methodology

Domus Orbis showed that Slice-First can start from an everyday and small problem without losing methodological value.

The central learning was:

> The first slice should not imitate a miniature version of the future system. It should protect the current need with the smallest sufficient amount of context.

In this case, the future system could include automation, markets, payments, or inventory. But the first need was much smaller:

> The monthly list must exist before payment.

That was the starting point.

## Diagrams according to responsibility

Diagrams were used where they helped fulfill the responsibility of the document.

The process document used a flow diagram because it needed to show steps and friction.

The solution proposal used a modified version of the flow to show the minimum proposed intervention.

This led to a future rule for VSlices Docs Standard:

> Each document can define the views or diagrams it needs according to the question it must answer.

Diagrams are not mandatory by default, but they are not decoration either when they help understanding happen faster.

### Open questions

* How will diagrams evolve VSlices Docs Standard, considering its current and future responsibilities?

## Colocated documentation

The documentation of Domus Orbis lives inside the [same project](https://github.com/HernanFAR/DomumOrbis), under a [Docs](https://github.com/HernanFAR/DomumOrbis/tree/master/Docs) folder.

This was intentional. When documentation is close to implementation, it becomes easier to preserve continuity between:

* context
* scope
* vocabulary
* processes
* proposals
* *artifacts*
* validations
* future code

### Open questions

* How does this facilitate integration with the future CLI and other product iterations?

## Which VSlices products can evolve

### VSlices Method

This case reinforces that Iteration 0 can be used to document the current reality before defining the first Slice-First.

It also reinforces that no phase has a fixed document set. Phases guide the reasoning, but *artifacts* and documentation depend on context.

### VSlices Docs Standard

#### Confirmations of idea usefulness

This case confirms the usefulness of several ideas:

* naming convention with segments such as `context.scenario.md`, using a form close to `<type>.<short-name>`;
* selective vocabulary, without filling every slot when it does not add value.

#### New taxonomy: Diagrams

This case confirms the need for VSlices Docs Standard to consider a new taxonomy for diagrams.

| Context                       | Related diagram                  |
| ----------------------------- | -------------------------------- |
| Defining scenario scope       | Use case diagram                 |
| Defining iteration scope      | Use case diagram                 |
| Writing a process document    | Flow diagram, swimlane diagram   |
| Writing a use case document   | Flow, behavior, or state diagram |
| Writing a capability document | Dependency map                   |
| Writing domain vocabulary     | Flow diagram                     |

If we open a Diagrams line, we need to consider:

* what meaning we will give to each piece or container;
* when we recommend using these diagrams according to context;
* how these diagrams relate to a specific document.

#### New documents

This iteration opened an important point: Support Notes, as such, can work as primitive versions of more specific documents.

Many of these more specific documents still do not have a direct equivalent inside VSlices Docs Standard.

For example:

| Document                                                                                                                             | Possible derivative                |
| ------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------- |
| [improvement.solution](https://github.com/HernanFAR/DomumOrbis/blob/master/Docs/Iteraci%C3%B3n%200/planning/improvement.solution.md) | L0 Continuous Improvement Document |
| [proposal.solution](https://github.com/HernanFAR/DomumOrbis/blob/master/Docs/Iteraci%C3%B3n%200/planning/proposal.solution.md)       | L0 Proposal Document               |
| [scope.iteration](https://github.com/HernanFAR/DomumOrbis/blob/master/Docs/Iteraci%C3%B3n%200/understanding/scope.iteration.md)      | L0 Scope Document                  |

Each document would have a specific responsibility, differentiated from other documents.

#### Use of Support Note

The concept of Support Note has proven very useful for defining more complex documents in a simple way.

However, it has also proven too generic to function as a 1:1 equivalent of specific L0 versions.

This means we should consider the option of generating an L0 version of each document within the templates.

This is not far-fetched, since the nature of Support Notes forces us to add new paragraphs or segments when they are used to represent more specific documents, such as an L0 Context Document.

For Support Notes, this means they no longer necessarily represent an L0 document. They represent a general idea of something, which may or may not be official, and which may or may not become an L0 document with new default segments in a future delivery.

### VSlices Design

This case helps teach separation between:

* current need
* current process
* proposed solution
* initial *artifact*
* future improvement
* premature automation

It also shows how an everyday problem can reveal important domain boundaries.

### VSlices Framework

This case reinforces that colocated documentation can be important for future tooling.

If documents live close to the project, a CLI could discover *artifacts*, validate relationships, generate scaffolding, or review continuity between documentation and implementation.

#### Open questions

* How would code autogeneration tooling work with VSlices Docs Standard?
