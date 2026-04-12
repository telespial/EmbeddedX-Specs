# EmbeddedX Interoperability

## Cross-Repository Alignment for the EmbeddedX Platform

Proposed by: Richard Haberkern  
Contact: rmhaberkern@gmail.com  

Free for evaluation. Commercial use requires permission. See license.md for more information.

* * *

## Abstract

EmbeddedX depends on multiple repositories working together without collapsing into duplication. This document establishes the platform-level interoperability rules that keep the ecosystem coherent.

* * *

## 1. Recommended Dependency Direction

The recommended conceptual direction is:

* MRD → MDF → EIL → AICS

In practice:

* MRD establishes hardware-visible reality
* MDF establishes model-visible structure
* EIL establishes runtime intelligence integration
* AICS constrains how AI systems create or modify code around that stack

* * *

## 2. Interoperability Rules

* Use stable naming across repositories
* Avoid copying full sibling documents into another repository
* Reference sibling repositories explicitly
* Keep terminology aligned
* Make higher layers respect lower-layer definitions
* Keep platform-level guidance separate from implementation-specific behavior

* * *

## 3. Cross-Reference Guidance

Specifications should reference one another through:

* stable names
* versioned releases where practical
* explicit identifiers where available
* human-readable repository links
* machine-readable schema identifiers when applicable

* * *

## 4. Compatibility Expectation

A repository is platform-compatible when it:

* uses EmbeddedX terminology consistently
* clearly identifies its boundaries
* supports machine-assisted use where appropriate
* preserves human inspectability where relevant
* does not contradict platform-level principles

* * *

## 5. Practical Result

The goal is a platform where tools, validators, and engineers can move across repositories without losing meaning.
