# EmbeddedX Rules and Control

## Overview

EmbeddedX relies on explicit rules to prevent uncontrolled generation, accidental overwrites, and state drift.

The platform should make it clear:

* what may be generated
* what may be modified
* what must remain read-only
* when validation is required
* when promotion is allowed
* how rollback is handled

## Rule Sources

Rules may come from:

* platform-level constraints
* project rules
* selected vendor constraints
* selected board constraints
* specification-layer compatibility requirements
* deployment requirements

## Operating Principle

If a system action could increase engineering risk, it should be bounded by explicit rules first.
