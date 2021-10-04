# OO Design

## Don't repeat yourself 

The DRY principle is stated as "Every piece of knowledge must have a single, unambiguous, authoritative representation within a system". The principle has been formulated by Andy Hunt and Dave Thomas in their book The Pragmatic Programmer. They apply it quite broadly to include "database schemas, test plans, the build system, even documentation". When the DRY principle is applied successfully, a modification of any single element of a system does not require a change in other logically unrelated elements. Additionally, elements that are logically related all change predictably and uniformly, and are thus kept in sync. Besides using methods and subroutines in their code, Thomas and Hunt rely on code generators, automatic build systems, and scripting languages to observe the DRY principle across layers.


## Rule of three (computer programming)

Rule of three ("Three strikes and you refactor") is a code refactoring rule of thumb to decide when similar pieces of code should be refactored to avoid duplication. It states that two instances of similar code do not require refactoring, but when similar code is used three times, it should be extracted into a new procedure. The rule was popularised by Martin Fowler in Refactoring[1] and attributed to Don Roberts.

Duplication is considered a bad practice in programming because it makes the code harder to maintain. When the rule encoded in a replicated piece of code changes, whoever maintains the code will have to change it in all places correctly.

However, choosing an appropriate design to avoid duplication might benefit from more examples to see patterns in. Attempting premature refactoring risks selecting a wrong abstraction, which can result in worse code as new requirements emerge and will eventually need to be refactored again.

The rule implies that the cost of maintenance certainly outweighs the cost of refactoring and potential bad design when there are three copies, and may or may not if there are only two copies.


## Minimum viable product

A minimum viable product (MVP) is a version of a product with just enough features to be usable by early customers who can then provide feedback for future product development.

A focus on releasing an MVP means that developers potentially avoid lengthy and (ultimately) unnecessary work. Instead, they iterate on working versions and respond to feedback, challenging and validating assumptions about a product's requirements. The term was coined and defined in 2001 by Frank Robinson and then popularized by Steve Blank and Eric Ries. It may also involve carrying out market analysis beforehand. The MVP is analogous to experimentation in the scientific method applied in the context of validating business hypotheses. It is utilized so that prospective entrepreneurs would know whether a given business idea would actually be viable and profitable by testing the assumptions behind a product or business idea. The concept can be used to validate a market need for a product and for incremental developments of an existing product. As it tests a potential business model to customers to see how the market would react, it is especially useful for new/startup companies who are more concerned with finding out where potential business opportunities exist rather than executing a prefabricated, isolated business model.