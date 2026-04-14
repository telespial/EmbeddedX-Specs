# EmbeddedX Project Framework

## Overview

The EmbeddedX Project Framework defines how embedded projects are created, structured, and controlled within the EmbeddedX system.

The goal is to ensure that all projects:

* maintain deterministic system behavior
* support safe integration of intelligence layers
* remain structured and reproducible
* reduce integration risk
* accelerate development cycles

This framework separates reusable system knowledge from project-specific implementation.

## Shared Library vs Project Workspace

### Shared Library

The shared library contains reusable assets across all projects.

Examples:

* vendor hubs
* development kits
* component libraries
* reusable specifications
* reusable sample code
* Software Development Kit references
* debug references
* reusable documents and manifests

### Project Workspace

Each project contains only project-specific data, configuration, references, outputs, validation artifacts, and restore states.

No global assets should be duplicated unless a project-specific fork or snapshot is required.

## Project Creation Flow

When a new project is created:

1. a project workspace is initialized
2. `start_here.md` is generated
3. `project.manifest.json` is created
4. `project.rules.md` is created
5. references to shared library assets are established
6. initial state folders are created
7. bounded system agents begin controlled analysis and setup

## Required Project Files

### `start_here.md`

Defines:

* project intent
* target hardware
* vendor and board
* current inputs available
* missing critical assets
* current project state
* immediate next step

### `project.manifest.json`

Defines:

* project identity
* selected vendor and hardware
* referenced library assets
* active specifications
* enabled agents
* validation requirements
* state locations
* package and deployment targets

### `project.rules.md`

Defines:

* allowed operations
* restricted modifications
* read-only areas
* validation requirements
* promotion conditions
* rollback rules
* project-specific constraints
