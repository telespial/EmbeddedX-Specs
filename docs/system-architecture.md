# EmbeddedX System Architecture

## A Framework-First Architecture for Building Embedded Products with Integrated Intelligence

EmbeddedX is structured as a framework-first system:

```text
EmbeddedX Framework / Platform
        ├── Machine Readable Datasheet (MRD)
        ├── Machine Readable Connectivity (MRC)
        ├── Model Definition Package (MDP)
        ├── Embedded Intelligence Layer (EIL)
        ├── AI Integrated Coding System (AICS)
        └── Embedded Intelligence Package (EIP)
                 ↓
      Generated / Integrated Firmware
                 ↓
          Physical Hardware
```

The framework also establishes a shared library and controlled project workspace model so projects can be created, validated, recovered, and scaled consistently.

## Architectural Rules

### Rule 1

The framework comes first. EmbeddedX defines the system-level rules that coordinate the specification family.

### Rule 2

MRD, MRC, MDP, EIL, AICS, and EIP are sibling specification layers under the EmbeddedX framework.

### Rule 3

Generated firmware should be constrained by the combined effect of those layers.

### Rule 4

Project creation, state control, recovery, and validation are part of the architecture, not optional add-ons.

### Rule 5

Reusable knowledge belongs in the shared library. Project-specific state belongs in project workspaces.
