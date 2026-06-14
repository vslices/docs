# VSlices and Development Methodologies

## Purpose

This document explains how VSlices relates to other software development methodologies, practices, and architectural approaches.

VSlices is not primarily:

* an agile methodology
* a project management framework
* a fixed architecture
* a replacement for existing engineering practices

VSlices is a continuity-oriented software engineering suite. Its main concern is preserving alignment between:

* domain understanding
* documentation
* design reasoning
* architecture
* implementation
* system evolution

## The core difference

Most development methodologies and delivery approaches have a specific center of gravity.

- Agile focuses on adapting delivery.
- Scrum focuses on organizing teamwork.
- Extreme Programming focuses on technical feedback and engineering quality.
- Lean focuses on reducing waste and improving flow.
- Domain-Driven Design focuses on understanding and modeling the domain.

VSlices focuses on continuity. The central questions are not only:

> How do we deliver software? 
> How do we organize code?

The central question is:

> How do we preserve domain intent, architectural meaning, documented knowledge, and executable behavior as the system evolves?

## Scope

This document compares VSlices with development methodologies and delivery-oriented approaches.

It does not compare VSlices with architectural styles or implementation patterns.

Architectural approaches such as Clean Architecture, Hexagonal Architecture, CQRS, Event Sourcing, microservices, modular monoliths, or Vertical Slice Architecture should be discussed separately.

## VSlices and Agile

VSlices is highly compatible with Agile principles. Both value:

* incremental evolution
* adaptability
* feedback
* simplicity
* avoiding unnecessary upfront complexity

However, Agile mainly addresses how teams adapt and deliver value over time.

VSlices addresses how knowledge, decisions, boundaries, behaviors, and implementation remain connected while that delivery happens. 

While Agile asks: _How do we respond to change?_, VSlices asks: _How do we respond to change without losing the meaning of the system?_.

## VSlices and Scrum

Scrum provides a structure for team coordination through roles, events, artifacts, and iterations.

And VSlices does not try to replace Scrum, because it does not define:

* sprints
* product owners
* scrum masters
* sprint reviews
* backlog management rules

A team using Scrum could still use VSlices to preserve continuity between product discovery, documentation, architecture, and implementation.

Scrum helps organize work. VSlices helps preserve the meaning of the work.

## VSlices and Extreme Programming

VSlices is strongly aligned with Extreme Programming. Both value:

* simplicity
* feedback
* continuous improvement
* technical quality
* refactoring
* sustainable engineering practices

Extreme Programming focuses deeply on how software is built safely and incrementally. VSlices extends this concern toward continuity between the code and the knowledge that justifies the code.

While XP asks: _How do we build software with high technical quality and fast feedback?_, VSlices asks: _How do we keep that technical quality connected to domain intent, documented decisions, and architectural evolution?_.

## VSlices and Lean Software Development

VSlices is highly aligned with Lean thinking. Both care about:

* reducing waste
* delaying unnecessary decisions
* amplifying learning
* avoiding overproduction
* improving flow

VSlices applies this thinking to software knowledge continuity. From a VSlices perspective, unnecessary abstractions, outdated documentation, disconnected tickets, unclear decisions, and architecture detached from domain needs are forms of waste. 

While Lean asks: _How do we reduce waste and improve learning?_, VSlices asks: _How do we reduce waste caused by fragmented knowledge and lost architectural intent?_.

## VSlices and Domain-Driven Design

VSlices is deeply compatible with Domain-Driven Design. Both care about:

* domain language
* domain boundaries
* business meaning
* explicit models
* software shaped by real business needs

Domain-Driven Design helps teams discover, understand, and model the domain. VSlices attempts to preserve that understanding across documentation, design, architecture, implementation, and evolution.

While DDD asks: _How do we model software around the domain?_, VSlices asks: How do we keep the domain model, documented knowledge, architectural structure, and executable behavior aligned over time?

## VSlices and Waterfall

VSlices is not aligned with traditional Waterfall as a sequential lifecycle model. VSlices does not assume that discovery, documentation, design, implementation, and validation happen once in a fixed order.

However, VSlices does not reject documentation or upfront thinking. The problem is not documentation. It is treating documentation as frozen knowledge.

VSlices prefers living documentation that evolves with implementation and preserves architectural meaning over time. 

Waterfall tends to ask: _What should be specified before implementation begins?_, VSlices asks: _What knowledge must remain visible and evolvable while the system changes?_.

## Comparative summary

| Approach                    | Main concern                          | VSlices relationship                                        |
| --------------------------- | ------------------------------------- | ----------------------------------------------------------- |
| Agile                       | Adaptive delivery                     | Compatible, adds continuity between: <ul><li>Knowledge</li><li>Documentation</li><li>Implementation</li></ul> |
| Scrum                       | Team coordination                     | Complementary, does not replace it                          |
| Extreme<br/>Programming         | Technical quality<br/>and feedback        | Strongly aligned, extends continuity beyond code            |
| Lean                        | Waste reduction<br/>and learning          | Strongly aligned, treats fragmented knowledge as waste      |
| Domain-Driven<br/>Design        | Domain modeling                       | Deeply compatible, preserves domain intent across lifecycle |
| Waterfall                   | Sequential<br/>specification and<br/>delivery | Low alignment, VSlices prefers living continuity            |

## The VSlices position

VSlices is not a universal replacement for existing methodologies. It is a continuity layer for software engineering. It helps teams ask:

> Are our domain understanding, documents, decisions, architecture, and implementation still describing the same system?

When the answer is no, the system may still work, but its meaning has started to fragment.

VSlices exists to reduce that fragmentation.

## Conclusion

VSlices can work with agile teams, disciplined engineering teams, domain-driven teams, and teams using different architectural styles.

Its differentiation is not in replacing those approaches. It is in preserving continuity between them.

VSlices is concerned with what often gets lost between:

* understanding the business
* documenting the system
* designing the solution
* implementing the behavior
* and evolving the software over time

That continuity is the center of VSlices.
