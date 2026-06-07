# Design Patterns

Design Patterns documents the architectural and engineering patterns used throughout VSlices Framework.

The purpose of this section is not only to explain how to use framework features, but also is also to explain:

- the engineering problems behind each pattern
- the tradeoffs involved
- the architectural reasoning
- the underlying implementation concepts
- and the alternatives available outside the framework

VSlices does not aim to hide engineering concepts behind abstractions. Instead, it attempts to organize, standardize, and progressively compose ideas that can also be implemented using LanguageExt or plain .NET.

## Pattern structure

Every pattern should explain:

1. The problem it addresses.
2. The proposed solution.
3. The benefits it provides.
4. The tradeoffs it introduces.
5. How it looks in VSlices.
6. How it relates to LanguageExt.
7. How it can be implemented using plain .NET.
8. Related patterns and concepts.

This structure helps preserve continuity between the framework abstractions and the engineering ideas behind them.

## The three-level model

VSlices patterns are explained through three progressively deeper levels.

### Level 1 — VSlices

The first level focuses on the framework experience, focusing on DX and framework usage. It explains:

- what the pattern does
- what problem it solves
- how it is used
- why it improves ergonomics or continuity

### Level 2 — LanguageExt Equivalent

The second level focuses on architectural mechanics. It explains:

- which LanguageExt primitives are involved
- which effects are being composed
- how execution works internally
- how errors and dependencies are modeled

### Level 3 — Plain .NET Equivalent

The third level focuses on demystification, explaining the same idea but only using plain .NET. The objective is to demonstrate that:

- the concept is universal
- the framework is optional
- the architectural value exists independently from VSlices
