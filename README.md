# DDD Reference

*Opinionated reference guide DDD concepts and principles by [@_RobsonRamos](//twitter.com/_RobsonRamos)*

## Table of Contents

1. [Anticorruption Layer](#anticorruption-layer)
1. [Shared Kernel](#shared-kernel)


## Anticorruption Layer

The anticorruption layer protects your model from external influences managing the transformation of one context's model to another because it's important not to compromise the integrity of your bounded context to match the API of another.

When to use?
- Wrap commutication with legacy or third-party code
- If you communicate with other subsystems

**[Back to top](#table-of-contents)**

## Shared Kernel

The shared kernel allow share models or domain logics between contexts. It's a shared code dependency so it can be more risky due to coupling, for example: one team can break another team's functionality.

So it's important to have integrated tests that verifies the behavior of both models.



