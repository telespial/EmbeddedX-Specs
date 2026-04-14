# Project Rules

## Read-Only Areas

* /refs
* imported shared library manifests
* approved golden state snapshots

## Allowed Generated Areas

* /generated
* /validation
* /logs
* /states/candidate

## Validation Requirements

* structural checks
* reference consistency checks
* state transition checks

## Promotion Rule

No candidate may be promoted to golden without required validation and explicit approval.

## Rollback Rule

Failsafe and recovery states must remain restorable.
