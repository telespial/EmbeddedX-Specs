# EmbeddedX Agent Architecture

## Overview

EmbeddedX should not rely on one unbounded agent to build a project. It should operate through defined roles with explicit scope, permissions, and outputs.

This is a control system, not an improvisation system.

## Core Agent Roles

### Project Bootstrap Agent

Creates the initial project workspace, required files, and project state folders.

### Vendor Intake Agent

Understands the selected vendor, development environment, and reusable vendor assets.

### Development Kit Intake Agent

Loads board-specific manifests, documentation, sample code, and references.

### Component Normalization Agent

Classifies components by type and associates them with reusable library assets.

### Specification Synthesis Agent

Builds or links Machine Readable Datasheet (MRD), Machine Readable Connectivity (MRC), and Model Definition Package (MDP) related material.

### Runtime Integration Agent

Prepares Embedded Intelligence Layer (EIL) expectations and integration boundaries.

### AI Integrated Coding System Agent

Performs bounded code generation and modification under explicit rules.

### Validation Agent

Runs compile, structural, configuration, and project consistency checks.

### Recovery Agent

Controls restore points, rollback behavior, and state promotion.
