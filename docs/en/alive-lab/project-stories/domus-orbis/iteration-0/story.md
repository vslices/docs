# Iteration 0

*Documenting the current reality before defining the first Slice-First*

## Purpose

This iteration documents how Domus Orbis approached a real monthly shopping problem using VSlices Method.

The objective was not to immediately build an application, automate a store, or solve payments. The objective was to understand the current reality, delimit the scope, and produce a small solution that reduced friction without introducing complexity too early.

Iteration 0 existed to answer a question before implementation:

> What current reality do we need to preserve before defining the first stable behavior?

## Observed scenario

The problem appeared in the household's monthly shopping.

The purchase usually repeats month after month, but currently requires manually reconstructing the list inside a market application. If that list is not ready by the time payment is received, the purchase can be postponed.

When the purchase is postponed, the money intended for pantry supplies can disperse into other expenses, emergencies, or day-to-day decisions.

The problem was not just buying. The problem was that the monthly shopping intention did not exist before the critical moment.

## 1. Understanding

The first phase was Understanding.

Instead of starting by designing a solution, the scenario where the need appeared was documented.

| Document type                                                                            | Specific name                                                                                                                     | Utility                                                                                                                                                                              |
| ---------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| [L0 Context Document](../../../../products/docs-standard/taxonomy/context-document.md)   | [context.scenario](https://github.com/HernanFAR/DomumOrbis/blob/master/Docs/Iteraci%C3%B3n%200/understanding/context.scenario.md) | Explained the real context: monthly shopping, available money, executive load, limited time, and risk of money dispersion.                                                           |
| [Support Note](../../../../products/docs-standard/taxonomy/support-note.md)              | [scope.iteration](https://github.com/HernanFAR/DomumOrbis/blob/master/Docs/Iteraci%C3%B3n%200/understanding/scope.iteration.md)   | Delimited which part of the scenario would be analyzed. This avoided expanding the iteration toward full inventory, payment automation, multiple markets, or a complete application. |
| [L1 Domain Vocabulary](../../../../products/docs-standard/taxonomy/domain-vocabulary.md) | [vocabulary.domain](https://github.com/HernanFAR/DomumOrbis/blob/master/Docs/Iteraci%C3%B3n%200/vocabulary.domain.md)             | Preserved important terms such as monthly shopping list, prepared list, market, cart, payday, money dispersion, and executive load.                                                  |

The vocabulary was worked on in parallel with the context and scope documents. It was not necessary to wait until the scenario was completely closed before starting to capture terms.

## 2. Contextualizing

After understanding the scenario, the current process was documented.

| Document type                                                                       | Specific name                                                                                                                                           | Utility                                      |
| ----------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------- |
| [Process Document](../../../../products/docs-standard/taxonomy/process-document.md) | [process.household-shopping](https://github.com/HernanFAR/DomumOrbis/blob/master/Docs/Iteraci%C3%B3n%200/contextualizing/process.household-shopping.md) | Showed how household shopping happens today. |

The identified flow was:

* the monthly payment is received;
* it is evaluated whether there is time, energy, and focus;
* if there is, the market application is opened;
* the list is manually reconstructed in the cart;
* the purchase is made;
* if there is not, the purchase is postponed;
* during the postponement, the money can disperse.

The process was represented with a flow diagram because the problem depended on sequence, timing, and friction.

This made it possible to see that the fragile point was not at the end of the process, but before it: the list did not exist as a prepared intention before payment.

## 3. Planning

With the scenario and process clear, the work moved to Planning.

| Document type | Specific name                                                                                                                        | Utility                                                                             |
| ------------- | ------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------- |
| Support Note  | [proposal.solution](https://github.com/HernanFAR/DomumOrbis/blob/master/Docs/Iteraci%C3%B3n%200/planning/proposal.solution.md)       | Defined the solution, where it takes place, what it will do, and how it will do it. |
| Support Note  | [improvement.solution](https://github.com/HernanFAR/DomumOrbis/blob/master/Docs/Iteraci%C3%B3n%200/planning/improvement.solution.md) | Defined how the solution could evolve.                                              |

The proposed solution was intentionally small.

It did not propose building all of Domus Orbis. It did not propose automating payment. It did not propose integrating a store in a definitive way.

The chosen solution was to create a centralized YAML file to register the monthly shopping list.

The initial format had to allow registering:

* format version;
* list name;
* markets;
* market base URL;
* products;
* product name;
* product URL;
* quantity or weight.

The idea was for the list to exist outside the cart of a specific store. That way, it could be prepared before payment and used as a starting point to reconstruct the purchase with less friction.

Among the future improvements were:

* validate the YAML;
* add weight unit;
* add product notes;
* mark essential products;
* generate a human-readable view of the list;
* prepare the cart in an assisted way;
* automate cart preparation;
* support multiple markets more explicitly;
* register a list as paid;
* pay a list.

This allowed ideas to be preserved without turning the iteration into something larger than necessary.

## 4. Building

The Building phase produced the minimum useful artifact.

| Document type | Specific name                                                                                                                                              | Utility                                       |
| ------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------- |
| Artifact      | [artifact.monthly-shopping-list](https://github.com/HernanFAR/DomumOrbis/blob/master/Docs/Iteraci%C3%B3n%200/building/artifact.monthly-shopping-list.yaml) | YAML container used to define shopping lists. |

In this case, no formal usage guide was created because the user, the client, and the domain expert were the same person.

The delivery was simply the YAML.

This left an important learning:

> Building does not always imply code. Sometimes the first useful artifact is a file, a template, a configuration, or a persisted structure.

For this context, building an application would have been too much. The YAML file was enough to validate whether a centralized list reduced real friction.

## 5. Validating

The Validating phase was approached as a personal feedback note.

| Document type   | Specific name                                                                                                               | Utility                                                      |
| --------------- | --------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------ |
| Validation Note | [validation.iteration](https://github.com/HernanFAR/DomumOrbis/blob/master/Docs/Iteraci%C3%B3n%200/validation.iteration.md) | Provided risks and feedback based on the completed solution. |

The validation method was user feedback and domain expert review.

Since the real user was also the domain expert, no formal ceremony was needed. It was enough to observe whether the artifact helped during real use.

The first relevant observation was:

> A centralized list can be common, but each market has its own way of turning that list into a purchase.

This learning suggests that the monthly list domain should be separated from market adapters.

The list can be stable. The way the cart is prepared can change depending on the market.

## Conclusion

Iteration 0 of Domus Orbis showed that a Slice-First can begin before code.

The iteration did not produce an application. It produced understanding, scope, vocabulary, process, proposal, future improvement, artifact, and documented validation.

The result was small, but useful. The main conclusion was:

> The first slice should not be a miniature version of the future system. It should protect the current need with the smallest sufficient amount of context.

In Domus Orbis, the current need was clear:

> The monthly list must exist before payment.

That was the foundation for continuing toward Iteration 1.
