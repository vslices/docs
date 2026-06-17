# VSlices and Development Methodologies

## Purpose

This document explains how VSlices relates to software development methodologies, practices, and delivery approaches.

VSlices is not an agile methodology, a project management framework, a fixed architecture, or a replacement for existing engineering practices.

It is a continuity-oriented software engineering suite. Its main concern is preserving alignment between domain understanding, documentation, design reasoning, architecture, implementation, and system evolution.

## The core difference

Most development methodologies and delivery approaches have a specific center of gravity.

- Agile focuses on adapting delivery.
- Scrum focuses on organizing teamwork.
- Extreme Programming focuses on technical feedback and engineering quality.
- Lean focuses on reducing waste and improving flow.
- Domain-Driven Design focuses on understanding and modeling the domain.

VSlices focuses on continuity between those concerns.

Its central questions are not only:

* How do we deliver software?
* How do we organize code?

!!! note "Central question for VSlices"

    How do we preserve domain intent, architectural meaning, documented knowledge, and executable behavior as the system evolves?

## Scope

| This document covers | This document does not cover |
| --- | --- |
| How VSlices relates to development methodologies and delivery-oriented approaches. | How VSlices relates to architectural styles or implementation patterns. |

Architectural approaches such as Clean Architecture, Hexagonal Architecture, CQRS, Event Sourcing, microservices, modular monoliths, or Vertical Slice Architecture should be discussed separately.

## VSlices and other methodologies

VSlices can be compared with different methodologies and delivery approaches. Each comparison keeps the same focus: what the other approach optimizes for, how it relates to VSlices, and what VSlices adds through continuity.


=== "Agile"

    **Relationship:** Highly compatible.
    
    **Shared concerns:**

    * incremental evolution
    * adaptability
    * feedback
    * simplicity
    * avoiding unnecessary upfront complexity

    **Difference:** Agile focuses on adapting delivery. VSlices focuses on preserving continuity while delivery happens.

    !!! note "VSlices question"

        How do we respond to change without losing the meaning of the system?
        

=== "Scrum"

    **Relationship:** Complementary.

    **Scrum defines:**

    * sprints
    * product owners
    * scrum masters
    * sprint reviews
    * backlog management rules

    **Difference:** Scrum helps organize work. VSlices helps preserve the meaning of the work.

    !!! note "VSlices question"

        How do we preserve continuity between product discovery, documentation, architecture, and implementation?

=== "Extreme Programming"

    **Relationship:** Strongly aligned.

    **Shared concerns:**

    * simplicity
    * feedback
    * continuous improvement
    * technical quality
    * refactoring
    * sustainable engineering practices

    **Difference:** Extreme Programming focuses on building software safely and incrementally. VSlices extends that concern toward continuity between code and the knowledge that justifies the code.

    !!! note "VSlices question"

        How do we keep technical quality connected to domain intent, documented decisions, and architectural evolution?


=== "Lean Software Development"

    **Relationship:** Strongly aligned.

    **Shared concerns:**

    * reducing waste
    * delaying unnecessary decisions
    * amplifying learning
    * avoiding overproduction
    * improving flow

    **Difference:** Lean focuses on reducing waste and improving learning. VSlices applies that concern to software knowledge continuity, treating fragmented knowledge, outdated documentation, unclear decisions, and architecture detached from domain needs as forms of waste.

    !!! note "VSlices question"

        How do we reduce waste caused by fragmented knowledge and lost architectural intent?


=== "Domain-Driven Design"

    **Relationship:** Deeply compatible.

    **Shared concerns:**

    * domain language
    * domain boundaries
    * business meaning
    * explicit models
    * software shaped by real business needs

    **Difference:** Domain-Driven Design helps teams discover, understand, and model the domain. VSlices attempts to preserve that understanding across documentation, design, architecture, implementation, and evolution.

    !!! note "VSlices question"

        How do we keep the domain model, documented knowledge, architectural structure, and executable behavior aligned over time?


=== "Waterfall"

    **Relationship:** Low alignment with traditional sequential Waterfall.

    **Difference:** Waterfall treats discovery, documentation, design, implementation, and validation as a sequence that happens in a fixed order. VSlices treats them as evolving sources of knowledge.

    !!! note "VSlices question"

        What knowledge must remain visible and evolvable while the system changes?


## Comparative summary

The table below summarizes the main relationship between each approach and VSlices.

| Approach | Main concern | VSlices relationship |
| --- | --- | --- |
| Agile | Adaptive delivery | Compatible; adds continuity between knowledge, documentation, and implementation. |
| Scrum | Team coordination | Complementary; does not replace it. |
| Extreme Programming | Technical quality and feedback | Strongly aligned; extends continuity beyond code. |
| Lean | Waste reduction and learning | Strongly aligned; treats fragmented knowledge as waste. |
| Domain-Driven Design | Domain modeling | Deeply compatible; preserves domain intent across the lifecycle. |
| Waterfall | Sequential specification and delivery | Low alignment; VSlices prefers living continuity. |

## The VSlices position

VSlices is not a universal replacement for existing methodologies. It is a continuity layer for software engineering.

It helps teams ask:

!!! note "Continuity question"

    Are our domain understanding, documents, decisions, architecture, and implementation still describing the same system?

When the answer is no, the system may still work, but its meaning has started to fragment.

VSlices exists to reduce that fragmentation.

## Conclusion

VSlices can work with agile teams, disciplined engineering teams, domain-driven teams, and teams using different architectural styles.

Its differentiation is not in replacing those approaches. It is in preserving continuity between business understanding, documentation, design, implementation, and software evolution.

That continuity is the center of VSlices.
